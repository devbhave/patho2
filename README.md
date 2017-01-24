# Patho2 : Pathology Reporting Tool #
Patho2 is the minimalistic tool for generating reports from the database. It uses SQLite database. Latex is used for report generation.

## Database Structure ##
Table PathData is a map f: (Date, Patient_No) -> Hash<Field, Value>
Hash is stored as compressed text

Each field has unique 'key'.
There are following type fields.

 - Patient Information Fields: Contains fields like name, age, etc.
 - Testing Data Fields: Contains fields like cbc, bloodgroup, etc.
 - Meta Information Fields: Contains fields like  Enable_CBC_Report, etc.

## Data Validation ##
Field values are validated against set of constraints.
- Field specific constraints
- Report specific constraints
- Global constraints

