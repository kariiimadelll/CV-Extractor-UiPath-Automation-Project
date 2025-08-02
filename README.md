# 📄 CV Extractor – UiPath Automation Project

A UiPath bot that reads all CVs (PDF files) from a folder, extracts key candidate information, and writes the results into an Excel file for easy review and analysis.

---

## 🔍 What It Does

- Loops through all PDF CVs in a given folder
- Extracts structured data such as:
  - Full Name
  - Email Address
  - Phone Number
  - Job Title
  - Address (if available)
- Saves all extracted data into an Excel sheet (`Output.xlsx`)

---

## 🧠 Use Cases

- HR automation to filter and manage CVs
- Resume parsing for recruitment systems
- Any scenario requiring structured CV data collection

---

## 🗂 Project Structure

| File/Folder                          | Description |
|-------------------------------------|-------------|
| `main.xaml`                         | Main entry point that calls sub-workflows |
| `CvProject_DataExtraction.xaml`     | Extracts Name, Email, Phone, etc. from each PDF |
| `CvProject_BuildDataTable.xaml`     | Creates a structured DataTable to hold extracted data |
| `CvProject_AddingToExcel.xaml`      | Writes the DataTable into `Resume.xlsx` |
| `CVs/`                   | Folder containing input CVs in PDF format |
| `Output/Resume.xlsx`                  | Excel file generated with extracted results |
| `.gitignore`                        | Excludes temp/system files from version control |

---

## ⚙️ Dependencies

- UiPath.PDF.Activities
- UiPath.Excel.Activities
- UiPath.System.Activities
- UiPath.IntegrationService.Activities = 1.15.0
- UiPath.IntelligentOCR.Activities = 6.25.1-preview
Make sure these packages are installed from **Manage Packages** in UiPath Studio.

---

## 🚀 How to Run

1. Place sample CVs in the `CVs/` folder
2. Open the project in UiPath Studio
3. Run `main.xaml`
4. Check the `Data/ٌResume.xlsx` file for extracted data

---

## 👤 Author

Created by [Karim Adel]  
A project to automate candidate data extraction from CVs using UiPath.

---

## 🏷 Tags

`UiPath` • `RPA` • `PDF Extraction` • `Excel Automation` • `CV Parser`
