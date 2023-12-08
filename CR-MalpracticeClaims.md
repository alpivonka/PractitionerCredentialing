Malpractice Claims History (5 Yr Window)


| **CR Object**     | **CR Attribute** | **CR Description**           | **FHIR Resource** | **FHIR Attribute**                                           |
|-------------------|------------------|------------------------------|-------------------|--------------------------------------------------------------|
| Malpractice Claim | Id               | Identifier of claim          | Claim             | Identifier                                                   |
| Malpractice Claim | Date             | Date of claim                | Claim             | event.when | type or Created                                 |
| Malpractice Claim | Author           | Author of claim              | Claim             | enterer (Practitioner/Patient/RelatedPerson)                 |
| Malpractice Claim | Patient          | Patient                      | Claim             | patient                                                      |
| Malpractice Claim | Allegation       | Claim allegations            | Claim             | item (Product or service provided), accident, supportingInfo |
| Malpractice Claim | Outcome          | Outcome of the claim         | Claim             | ???                                                          |
| Malpractice Claim | Action           | Actions imposed or taken     | Claim             | ???                                                          |
| Malpractice Claim | Practitioner     | Who the claim was made about | Claim             | careteam.provider (Organization/Practitioner)                |
| Malpractice Claim | Insurerance      | Who is the Insurer           | Claim             | insurer                                                      |