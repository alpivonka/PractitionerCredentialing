**DEA-Certification**

A certification granted by the U.S. Drug Enforcement Administration (DEA) to a healthcare professional who is authorized to prescribe controlled substances.

[Back to Practitioner Credentialing](https://github.com/alpivonka/PractitionerCredentialing/blob/main/README.md)


| **CR Object** | **CR Attribute**   | **CR Description**                                                                                                                                      | **FHIR Resource** | **FHIR Attribute**                                        |
|---------------|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|-----------------------------------------------------------|
| DEA           | RegistrationNumber | DEA Registration Number Issued by the DEA                                                                                                               | Practitioner      | "Qualification.Identifier.value                           |
|               |                    |                                                                                                                                                         |                   | Qualification.Identifier.period                           |
|               |                    |                                                                                                                                                         |                   | Qualification.Identifier.assigner (Organization)          |
|               |                    |                                                                                                                                                         |                   | Qualification.identifier.type"                            |
| DEA           | Schedules          | As list of Controled Substances by Schedule number.                                                                                                     | Practitioner      | Qualification.extension.schedule.code                     |
| DEA           | Business Address   | "The specific type of activity a registrant is authorized to conduct with controlled substances. **Must obtain list of DEA Activities for Code System** | Practitioner      |  ????                                                     |
| DEA           | Period             | Registration Issue and Experation Dates                                                                                                                 | Practitioner      | Qualification.period (Start/End date)                     |
| DEA           | Practitioner       | Who the Cerfication was issued to, responsible party                                                                                                    | Practitioner      | Practitioner which contains the Qualification             |
| DEA           | Address            | the physical location where the controlled substances are manufactured, distributed, imported, exported, or dispensed.                                  | Practitioner      | Qualification.extension.dea.address                       |
| DEA           | Type               | Type of cerfication                                                                                                                                     | Practitioner      | Qualification.code                                        |
| DEA           | Status             | Status of Certification                                                                                                                                 | Practitioner      | Qualification.extension.practitioner-qualification.status |
