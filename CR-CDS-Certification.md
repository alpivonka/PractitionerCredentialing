**CDS-Certification**

A certification granted by a state to a healthcare professional who is authorized to dispense controlled substances.

[Back to Practitioner Credentialing](https://github.com/alpivonka/PractitionerCredentialing/blob/main/CR-Practitioner.md)

| **CR Object** | **CR Attribute**   | **CR Description**                                                                                                     | **FHIR Resource** | **FHIR Attribute**                                        |
|---------------|--------------------|------------------------------------------------------------------------------------------------------------------------|-------------------|-----------------------------------------------------------|
| CDS           | Cerfication Number | CDS Certification Number                                                                                               | Practitioner      | Qualification.Identifier                                  |
| CDS           | Schedules          | As list of Controled Substances by Schedule number.                                                                    | Practitioner      | Qualification.extension.schedule.code                     |
| CDS           | IssueState         | USPS State                                                                                                             | Practitioner      | ????                                                      |
| CDS           | Effective Date     | Issue  Dates                                                                                                           | Practitioner      | Qualification.period (Start date)                         |
| CDS           | End Date           | Date of experation                                                                                                     | Practitioner      | Qualification.period (End date)                           |
| CDS           | Practitioner       | Who the Cerfication was issued to, responsible party                                                                   | Practitioner      | Practitioner which contains the Qualification             |
| CDS           | Address            | the physical location where the controlled substances are manufactured, distributed, imported, exported, or dispensed. | Practitioner      | Qualification.extension.dea.address                       |
| CDS           | Type               | Type of cerfication                                                                                                    | Practitioner      | Qualification.code                                        |
| CDS           | Status             | Status of Certification                                                                                                | Practitioner      | Qualification.extension.practitioner-qualification.status |
