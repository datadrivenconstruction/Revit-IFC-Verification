# Revit and IFC Validation Tool

## Overview
This Excel data validation tool is designed to automate the process of validating data records from Revit and IFC project data against specified criteria, converting data formats and exporting the results with detailed validation reports - which describe the percentage of parameter completion and their unique values. 


![enter image description here](https://datadrivenconstruction.io/wp-content/uploads/2024/07/DDC-Validation-Revit-and-IFC-.jpg.jpg)


## Features
- **Group Parameter Customization:** Ensures that the specified parameters exist for the groups specified in the tables.
- **Report:** Generates a report indicating the results of the validation, including whether the parameters for groups exist and are populated, and their unique values.
- **Customizable Validation Rules:** Users can define custom validation rules and criteria through the Excel interface.
- **Automation:** Accelerates repetitive tasks by automating data validation for both Revit and IFC projects.

## Additional Resources

-   **DDC RVT&IFC Converter:** https://datadrivenconstruction.io/index.php/convertors/ necessary free libraries for data conversion from Revit 2015-2023 and IFC2x3.


## Prerequisites

1. **Install Python:**
   - Download and install Python from the official website: [Python.org](https://www.python.org/downloads/).
   - Make sure to add Python to your system's PATH during installation.

2. **Verify Python Installation:**
   - Open Command Prompt (CMD) and run the following command to check the Python version:
     ```sh
     python --version
     ```
   - You should see an output similar to `Python 3.x.x`.

3. **Install Required Libraries:**
   - You can install the necessary Python libraries using pip:
     ```sh
     pip install pandas openpyxl
     ```

## Setup Configuration

1. **Open the `DDC Revit and IFC Validation.xlsx` file:**
   - This file contains all the necessary parameters and settings for the validation process.
   - In the Excel document, specify the path to the Revit (IFC, DWG, DGN) file.
   - On the next line, specify the path to the corresponding converter for Revit (IFC, DWG, DGN).
     - This path must end with the folder "datadrivenlibs".

2. **Update the File Path in the Script:**
   - Open the `Revit and IFC Validation.py` script.
   - Locate the variable `file_path_excel` in the script.
   - Update this variable to the path where the `DDC Revit and IFC Validation.xlsx` file is located.
     ```python
     file_path_excel = r'C:\Validation\DDC IFC Validation.xlsx'
     ```

3. **Specify Paths for Converter Libraries and Define Data Types to Validate:**
   - Ensure that all paths to the converter libraries are correctly specified in the Excel file.
   - Define the data types to validate as required.

## How to Use the Tool

1. In the Excel table, write the group of elements (e.g., walls, windows, etc.) you want to validate.
2. For each category, specify the parameters you want to check for presence and completeness in the project.

## Run the Tool

1. Execute the script from your terminal or command prompt:
   ```sh
   python Revit and IFC Validation.py
   ```

## Review Reports

1. Open the generated report Excel file to review the validation results.
   - The report will include details such as data compliance rates, identified issues, and suggestions for corrections.

## Adjust Settings (Optional)

1. Adjust validation settings in the Excel file if needed to fine-tune the results based on the initial output.
2. Rerun the tool to apply the new settings.

---


## Contributing
Contributions to this project are welcome! Here's how you can contribute:
- **Fork the Repository:** Click on the 'Fork' button at the top right corner of this repository.
- **Clone the Repository:** Clone the forked repository to your local machine.
- **Create a New Branch:** Create a new branch for your modifications.
- **Make Changes and Commit:** Make your changes in the new branch and commit them.
- **Push to the Branch:** Push your branch to your GitHub fork.
- **Create a Pull Request:** Open a pull request from your forked repository and we'll review your changes.

## Support
If you encounter any issues or have questions, please file an issue on the GitHub repository.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
