# Practitioner Credentialing
Below represents a high level mapping for the context of Practitioner Credentialing Logical Domain model.

I am working through the mapping and am needing for insights/recommendations.
1. What are some recommended ways to represent Sanctions. Currently utilizing flags, yet needing the flag to be contain both practitioner and practitionerRole so that sanctions are made more visible.
   1. Should sanctions be tied or have refrence to the specific qualification contained in the Practitioner? Flag would need to be able to reference Practitioner/PractitionerRole as its subject.
2. Is using FHIR Claim to represent Malpractice cliam appropate?
3. Is using FHIR Coverage to represent Malpractice Coverage?


| **Practitioner Credential Object** | **CR Attribute** | **CR Attribute Definition** | **FHIR Resource** | **FHIR Attribute** | **References** |
|------------------------------------|------------------|-----------------------------|-------------------|--------------------|----------------|
| Practitioner | A healthcare professional who is authorized to provide patient care. This includes physicians, nurses, pharmacists, and other allied health professionals. | Practitioner | | | |
| Practitioner | [State License](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-StateLicense.md) | A license granted by a state to a healthcare professional to practice medicine or another healthcare profession within that state. | Practitioner | Qualification | |
| Practitioner | [DEA Certification](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-DEA-Certification.md) | A certification granted by the U.S. Drug Enforcement Administration (DEA) to a healthcare professional who is authorized to prescribe controlled substances. | Practitioner | Qualification | |
| Practitioner | [CDS Certification](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-CDS-Certification.md) | A certification granted by a state to a healthcare professional who is authorized to dispense controlled substances. | Practitioner | Qualification | |
| Practitioner | [Education History](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-Education-History.md) | Education history of the Practitioner | Practitioner | Qualification | |
| Practitioner | [Work History](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-WorkHistory.md) | (Five-year window) The record of a healthcare professional's employment history, including the dates of employment, the positions held, and the duties performed. | PractitionerRole | practitioner(Practitioner) | |
| Practitioner | [Sanction](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-Sanctions.md) | State, Medicare & Medicaid Sanctions | Flag | | subject(Practitioner/PractitionerRole) |
| Practitioner | [Malpractice Claim History](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-MalpracticeClaims.md) | (Five-year window) the claims a practitioner has been involved with, the outcomes, and types of allocations. | Claim | | careteam.provider (Organization/Practitioner) |
| Practitioner | [Malpractice Coverage](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-MalpracticeCoverage.md) | Current proof malpractice insurance coverage | Coverage | | policyHolder(Practitioner) |



![image](https://github.com/alpivonka/PractitionerCredentialing/assets/4975072/3f738117-559c-4852-a75c-0db521ca61fb)



