# PractitionerCredentialing
Below represents a high level mapping for the context of Practitioner Credentialing Logical Domain model.

I am working through the mapping and am needing for insights/recommendations.
1. What are some recommended ways to represent Sanctions. Currently utilizing flags, yet needing the flag to be contain both practitioner and practitionerRole so that sanctions are made more visible.
   1. Should sanctions be tied or have refrence to the specific qualification contained in the Practitioner? Flag would need to be able to reference Practitioner/PractitionerRole as its subject.
2. Is using FHIR Claim to represent Malpractice cliam appropate?
3. Is using FHIR Coverage to represent Malpractice Coverage?


![image](https://github.com/alpivonka/PractitionerCredentialing/assets/4975072/79646c9b-1588-4212-a4b3-9a061239cbab)

![image](https://github.com/alpivonka/PractitionerCredentialing/assets/4975072/3f738117-559c-4852-a75c-0db521ca61fb)



