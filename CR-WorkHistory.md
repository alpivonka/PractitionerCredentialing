**Work History**

(Five-year window) The record of a healthcare professional's employment history, including the dates of employment, the positions held, and the duties performed.

[Back to Practitioner Credentialing](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-Practitioner.md)


| **CR Object** | **CR Attribute** | **CR Description**                                        | **FHIR Resource** | **FHIR Attribute**                         |
|---------------|------------------|-----------------------------------------------------------|-------------------|--------------------------------------------|
| Work History  | Id               | Identifier of work experience                             | PractitionerRole  | Identifier                                 |
| Work History  | Start Date       | Start date of work experience                             | PractitionerRole  | period.start                               |
| Work History  | End Date         | End date of work experience                               | PractitionerRole  | period.end                                 |
| Work History  | Employer         | The Employer                                              | PractitionerRole  | organization                               |
| Work History  | Employer Contact | Contact information for the Employer                      | PractitionerRole  | telecom (ContactPoint)                     |
| Work History  | Position         | Position of work experience                               | PractitionerRole  | role                                       |
| Work History  | specialtiy       | Specialtiy of work experience                             | PractitionerRole  | specialty                                  |
| Work History  | health Service   | Health Services performed by practitioner while employed. | PractitionerRole  | healthcareService                          |
| Work History  | Location         | Location of work experience                               | PractitionerRole  | location                                   |
| Work History  | Practitioner     | Practitioner of work experience                           | PractitionerRole  | Practitioner (Reference to a Practitioner) |
