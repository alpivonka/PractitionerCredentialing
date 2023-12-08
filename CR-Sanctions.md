**Sanctions**

Medical practitioner sanctions are disciplinary actions taken against a healthcare professional by a licensing board or regulatory body. These actions are imposed when a practitioner is found to have violated professional standards, laws, or regulations governing their practice.

[Back to Practitioner Credentialing](https://github.com/alpivonka/PractitionerCredentialing/blob/main/README.md)



| **CR Object** | **CR Attribute** | **CR Description**                  | **FHIR Resource** | **FHIR Attribute**                                               |
|------------------|------------------|-------------------------------------|-------------------|------------------------------------------------------------------|
| Sanction         | Id               | Flag                                | Identifier        |                                                                  |
| Sanction         | Type             | license suspension, fine, probation | Flag              | code                                                             |
| Sanction         | reason           | reason for                          | Flag              | supportingInfo                                                   |
| Sanction         | issuer           | issuer for                          | Flag              | author                                                           |
| Sanction         | start date       | start date                          | Flag              | period.start                                                     |
| Sanction         | end date         | end date                            | Flag              | period.end                                                       |
| Sanction         | status           | status of                           | Flag              | status                                                           |
| Sanction         | subject          | subject of                          | Flag              | subject (Practitioner, Organization, Location, PractitionerRole) |
