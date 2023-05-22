

# Data Warehouse Project - Olist E-Commerce Store

This project implements a data warehouse solution using the Olist E-Commerce store dataset. The data is extracted from the source system, transformed using SSIS (SQL Server Integration Services), and loaded into the destination database. The project involves the creation of six dimensions and three fact tables in the destination database.

## Project Structure

The project repository contains the following files and directories:

- `README.md`: Provides an overview and instructions for the project.
- `Olist_Data_Warehouse_Project.docx`: Word document with detailed step-by-step explanations and screenshots.
- `SSIS_Packages`: Directory containing SSIS packages used for data extraction, transformation, and loading.
- `SQL_Scripts`: Directory containing SQL scripts for creating the destination database, dimensions, and fact tables.
- `Data_Model`: Directory containing the data model diagram.

## Getting Started

To get started with the project, follow these steps:

1. Clone the project repository to your local machine:

   ```
   git clone https://github.com/safamahmoud71/DWH_Project.git
   ```

2. Review the `Olist_Data_Warehouse_Project.docx` document for detailed instructions and explanations.

3. Set up the destination database by executing the SQL scripts in the `SQL_Scripts` directory in the following order:
   - `create_database.sql`: Creates the destination database.
   - `create_dimensions.sql`: Creates the dimension tables.
   - `create_facts.sql`: Creates the fact tables.

4. Open SQL Server Integration Services (SSIS) and import the packages from the `SSIS_Packages` directory.
   - SourceToSTG.dtsx: Extracts data from the source system and loads it into the staging area.
   - STGToDestination.dtsx: Transforms the data from the staging area and loads it into the destination database.

5. Modify the connection strings in the SSIS packages to point to your source and destination databases.

6. Execute the SSIS packages in the following order:
   1. Run the SourceToSTG.dtsx package to extract and load data into the staging area.
   2. Run the STGToDestination.dtsx package to transform and load data into the destination database.

7. Verify that the data has been successfully loaded into the destination database.

8. Refer to the data model diagram in the `Data_Model` directory for an overview of the created dimensions and fact tables.

## Additional Resources

For more detailed instructions, screenshots, and explanations, please refer to the `phase2_Alaa Adel_.docx` document in the repository.



Feel free to contribute to the project by submitting pull requests or reporting issues.



Please note that the Olist E-Commerce store dataset used in this project has its own terms and conditions. Make sure to comply with the dataset's license and usage guidelines.

## Acknowledgments

Special thanks to Olist for providing the E-Commerce store dataset.


---

This is just a template for your README.md file. Feel free to modify and customize it according to your project's requirements and specifications.
