**Malpractice Coverage**

[Back to Practitioner Credentialing](https://github.com/alpivonka/PractitionerCredentialing/blob/main/README.md)



| **CR Object**        | **CR Attribute** | **CR Description**                        | **FHIR Resource** | **FHIR Attribute**                      |
|----------------------|------------------|-------------------------------------------|-------------------|-----------------------------------------|
| Malpractice Coverage | Id               | Identifier of Malpractice Insurance Proof | Coverage          | Identifier                              |
| Malpractice Coverage | Practitioner     | The entity the insurance covers           | Coverage          | beneficiary (Practitioner/Organization) |
| Malpractice Coverage | PolicyNumber     | x                                         | Coverage          | Identifier                              |
| Malpractice Coverage | Provider         | Insurance Provider                        | Coverage          | policyHolder (Organization)             |
| Malpractice Coverage | Type             | Type of coverage                          | Coverage          | type                                    |
| Malpractice Coverage | status           | status of coverage                        | Coverage          | status                                  |
| Malpractice Coverage | Issue Date       | x                                         | Coverage          | period.start                            |
| Malpractice Coverage | Experation Date  | x                                         | Coverage          | period.end                              |
