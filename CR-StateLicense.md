| **CR Object** | **CR Attribute** | **CR Description**                            | **FHIR Resource** | **FHIR Attribute**                                            |
|---------------|------------------|-----------------------------------------------|-------------------|---------------------------------------------------------------|
| State License | ID               | Identifier of this specific License Instance  | Practitioner      | "Qualification.Identifier.value                               |
|               |                  |                                               |                   | Qualification.Identifier.period                               |
|               |                  |                                               |                   | Qualification.Identifier.assigner (Organization)              |
| State License | Status           | The current status of the License             | Practitioner      | Qualification.practitioner-qualification.status               |
| State License | ValidLocation    | Where the License if valid (USPS state)       | Practitioner      | Qualification.practitioner-qualification.whereValid           |
| State License | Type             | The type of License                           | Practitioner      | Qualification.code                                            |
| State License | Period           | The Issue and experation dates of the License | Practitioner      | Qualification.period (Start/End date)                         |
| State License | Authority        | The License Issueing  Authority               | Practitioner      | Qualification.issuer(Organization)                            |
| State License | Licensee         | Who holds the License (Practitioner)          | Practitioner      | Practitioner which contains the Qualification (State license) |
