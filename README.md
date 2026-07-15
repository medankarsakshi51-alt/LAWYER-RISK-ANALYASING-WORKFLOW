# 🚀 Automated PDF Data Extraction Pipeline using Google Gemini & JavaScript

This repository contains an automated workflow that extracts structured information from uploaded PDFs and processes it seamlessly into multiple rows and data formats.

## 📋 Workflow Overview

The entire pipeline is triggered automatically upon form submission. Here is how the data flows:

* **Trigger**: A form submission initiates the process.
* **Extraction**: Text is extracted from the uploaded PDF file.
* **Initialization**: The system initializes three distinct database rows (`row`, `row1`, `row2`).
* **AI Analysis**: The extracted text is processed by **Google Gemini Chat Model** via an Information Extractor.
* **Data Splitting**: The AI output is split into individual line items (resulting in 6 distinct items).
* **Row Creation**: A new database row (`row3`) is generated for each of the 6 items.
* **Transformation**: Custom **JavaScript code** formats, cleans, or validates the processed data.
* **Completion**: The final structured dataset is outputted to an ending form or confirmation layout.

## 🛠️ Key Technologies Used

* **Google Gemini API**: For intelligent entity and information extraction.
* **JavaScript**: For custom post-processing, data manipulation, and cleaning.
* **Automation Platform**: Visual node workflow automation.

## 🚀 How to Use

1. Import the `workflow.json` file into your automation platform.
2. Connect your Google Gemini API credentials to the **Information Extractor** node.
3. Configure your database destinations for the row creation steps.
4. Publish and trigger the workflow with a PDF upload form!
