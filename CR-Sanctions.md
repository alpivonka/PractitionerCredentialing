**Sanctions**

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
