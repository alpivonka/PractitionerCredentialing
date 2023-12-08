**Education History**

Education history of the Practitioner

[Back to Practitioner Credentialing](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-Practitioner.md)



| **CR Object**                                    | **CR Attribute** | **CR Description**               | **FHIR Resource** | **FHIR Attribute**                  |
|--------------------------------------------------|------------------|----------------------------------|-------------------|-------------------------------------|
| Education History                                | Id               | Unique ID from Educational Unit  | Practitioner      | "Qualification.Identifier     |
| Education History                                | type             | Type of education attained       | Practitioner      | Qualification.code                  |
| Education History                                | start date       | Start Date of education attained | Practitioner      | Qualification.period.start          |
| Education History                                | end date         | End Date of education attained   | Practitioner      | Qualification.period.end            |
| Education History                                | Issuer           | ISSUER from Educational Unit     | Practitioner      | Qualification.issuer (Organization) |
