# Excel Data Validation Tool

## Overview
This Excel data validation tool is designed to automate the process of validating data records from Revit and IFC project data against specified criteria, converting data formats and exporting the results with detailed validation reports - which describe the percentage of parameter completion and their unique values. 


![enter image description here](https://datadrivenconstruction.io/wp-content/uploads/2024/07/DDC-Validation-Revit-and-IFC-.jpg.jpg)


## Features
- **Group Parameter Customization:** Ensures that the specified parameters exist for the groups specified in the tables.
- **Report:** Generates a report indicating the results of the validation, including whether the parameters for groups exist and are populated, and their unique values.
- **Customizable Validation Rules:** Users can define custom validation rules and criteria through the Excel interface.
- **Automation:** Accelerates repetitive tasks by automating data validation for both Revit and IFC projects.

## Additional Resources

-   **DDC RVT&IFC Converter:** https://datadrivenconstruction.io/index.php/convertors/ for tools to convert between Revit and IFC and XLSX (DataFrame) format.


## Prerequisites
Before you can run this tool, ensure you have the following installed:
- Python 3.6 or higher
- pandas library
- openpyxl library


You can install the necessary Python libraries using pip:
\`\`\`bash
pip install pandas openpyxl
\`\`\`

## Usage
To use this tool, follow these steps:

1. **Setup Configuration:**
   - Open the \`DDC Revit and IFC Validation.xlsx\` file.
   - Specify the paths to the input Excel files, define the data types for validation, and set the output parameters.

2. **Run the Tool:**
   - Execute the script from your terminal or command prompt:
     \`\`\`bash
     python excel_validation_tool.py
     \`\`\`

3. **Review Reports:**
   - Open the generated report Excel file to review the validation results.
   - Reports will include details such as data compliance rates, identified issues, and suggestions for corrections.

4. **Adjust Settings (Optional):**
   - Adjust validation settings and rerun the tool if needed to fine-tune the results based on the initial output.

## Example
Here is an example of setting up a validation rule in the \`config.xlsx\` file:

| Parameter          | Value                  |
| ------------------ | ---------------------- |
| File Path (file_path_excel)            | \`C:\Validation\DDC IFC Validation.xlsx\`   



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
"""
