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
| Practitioner | State License | A license granted by a state to a healthcare professional to practice medicine or another healthcare profession within that state. | Practitioner | Qualification | |
| Practitioner | DEA Certification | A certification granted by the U.S. Drug Enforcement Administration (DEA) to a healthcare professional who is authorized to prescribe controlled substances. | Practitioner | Qualification | |
| Practitioner | DCS Certification | A certification granted by a state to a healthcare professional who is authorized to dispense controlled substances. | Practitioner | Qualification | |
| Practitioner | Education History | Education history of the Practitioner | Practitioner | Qualification | |
| Practitioner | Work History | (Five-year window) The record of a healthcare professional's employment history, including the dates of employment, the positions held, and the duties performed. | PractitionerRole | practitioner(Practitioner) | |
| Practitioner | Sanction | State, Medicare & Medicaid Sanctions | Flag | | subject(Practitioner/PractitionerRole) |
| Practitioner | Malpractice Claim History | (Five-year window) the claims a practitioner has been involved with, the outcomes, and types of allocations. | Claim | | careteam.provider (Organization/Practitioner) |
| Practitioner | Malpractice Coverage | Current proof malpractice insurance coverage | Coverage | | policyHolder(Practitioner) |



![image](https://github.com/alpivonka/PractitionerCredentialing/assets/4975072/3f738117-559c-4852-a75c-0db521ca61fb)



