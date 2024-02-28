# Java Hospital Management System

Welcome to the Java Hospital Management System, a comprehensive project for managing hospital operations. This system includes features for handling patient records, doctor information, nurse details, room assignments, and insurance patient data.

## Getting Started

### Prerequisites

- **Java Development Kit (JDK):** [Download](https://www.oracle.com/java/technologies/javase-downloads.html)
- **MySQL Database:** [Download](https://dev.mysql.com/downloads/)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/mohdwarish483/JavaProject4thsem.git
   cd JavaProject4thsem

2. **Set up the database:**

Create a new MySQL database.
Import the SQL schema from dumps/FinalOOPSdb.sql.

3. **Compile and run the application:**
  ```bash
  javac -cp ".:./lib/mysql-connector-java.jar" src/Driver/Driver.java
  java -cp ".:./lib/mysql-connector-java.jar" src.Driver.Driver

```
## File Structure

.idea: IntelliJ IDEA configuration files.
lib: External libraries, including MySQL Connector/J.
out: Compiled Java classes.
src: Source code files.
CSVfiles: Directory for CSV files.
DAOpackage: Data Access Object package.
Doctors: Package containing Doctor-related classes.
Nurse: Package containing Nurse-related classes.
Patients: Package containing Patient-related classes.
Room: Package containing Room-related classes.
dumps: SQL dump files.


## Usage

Use the following commands to perform various operations:

**Patient Operations**
Add patient:

```bash
  java -cp ".:./lib/mysql-connector-java.jar" src.Driver.Driver -add patient < Patient name > < Patient ID > < Patient age > < Gender > < Admission Date > < Blood Group> < Phone number > < Status >
```
Remove:

java -cp ".:./lib/mysql-connector-java.jar" src.Driver.Driver -remove patient < Patient id >

Display patients list:

java -cp ".:./lib/mysql-connector-java.jar" src.Driver.Driver -display patient

Upload a CSV file:

java -cp ".:./lib/mysql-connector-java.jar" src.Driver.Driver -uploadCSV patient <Absolute Path of the CSV>

Update a Patient record:

java -cp ".:./lib/mysql-connector-java.jar" src.Driver.Driver -update patient < Patient ID > < Attribute > to < new value for the Attribute >

Bulk update via CSV:

java -cp ".:./lib/mysql-connector-java.jar" src.Driver.Driver -bulkUpdate patient <Absolute Path of the CSV>

Search patient:

java -cp ".:./lib/mysql-connector-java.jar" src.Driver.Driver -search patient <column name/names separated by comma> <constraint (optional)>

## Other Operations:
Similar commands are available for insurance patients, doctors, nurses, and rooms. Replace -add patient, -remove patient, etc., with the respective commands for insurance patients, doctors, nurses, and rooms.


## author
mohd warish
9991463786
khanwarish483@gmail.com
