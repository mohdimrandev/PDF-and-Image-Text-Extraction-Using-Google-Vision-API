# PDF and Image Text Extraction Using Google Vision API

This project extracts text from PDF and image files using the Google Vision API and supports batch processing of multiple files.

## Table of Contents

- [Introduction](#introduction)
- [Technologies Used](#technologies-used)
- [Techniques Used](#techniques-used)
- [Setup](#setup)
- [Running the Project](#running-the-project)

## Introduction

The goal of this project is to leverage the Google Vision API to extract text from PDF and image files, demonstrating the ability to process and analyze documents programmatically. This project includes support for bulk processing of multiple documents and outputs the extracted text in a structured format.

## Technologies Used

### Languages

[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)

### Libraries

![PyMuPDF](https://img.shields.io/badge/PyMuPDF-0172ca.svg?style=for-the-badge&logo=PyMuPDF&logocolor=black)
![Pillow](https://img.shields.io/badge/Pillow-%234b4b4d.svg?style=for-the-badge&logo=Pillow&logocolor=black)
![Google Cloud Vision](https://img.shields.io/badge/Google_Cloud_Vision-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

### Tools

![Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)

## Techniques Used

### Data Extraction

- Text extraction from PDFs using PyMuPDF
- Text extraction from images using Google Vision API

### Bulk Processing

- Handling multiple document files and extracting text from each

### Data Modeling

- Storing extracted text in a structured format using Pandas DataFrame
- Exporting extracted data to CSV format

## Setup

### 1. Go to the Google Cloud Console

   - Navigate to [Google Cloud Console](https://console.cloud.google.com/).

### 2. Create a new project

   - If you haven't already created a project, you can create a new one from the project selector dropdown in the upper left corner.

### 3. Enable the Vision API

   - Navigate to `APIs & Services` > `Library`.
   - Search for "Vision API".
   - Click on `Google Cloud Vision API` in the results.
   - Click `Enable` to enable the Vision API for your project.

### 4. Create credentials

   - After enabling the Vision API, you'll be prompted to create credentials.
   - Click on `Create credentials` and select the appropriate API (Vision API) from the list.

### 5. Choose the appropriate credential type

   - After selecting the Vision API, choose `Application data` as the credential type.

### 6. Configure service account details

   - Fill in the service account details as required (e.g., service account name, role).
   - In the `Service account permissions` step, add the `Viewer` role, which allows the service account to view resources associated with your project.

### 7. Create and download the service account key JSON file
   - After configuring the service account, proceed to manage its keys:
     - Click on the three dots (options menu) next to your newly created service account.
     - Select `Manage keys`, then click `Add key` > `Create new key`.
     - Choose `JSON` as the key type and click `Create`. This will download the JSON key file to your computer.
     - **Upload this JSON key file when prompted in google colab to authenticate Google Cloud services during project execution!**

## Running the Project

Run this project in Google Colab! You can access it here: <a href="https://colab.research.google.com/github/mohdimrandev/PDF-and-Image-Text-Extraction-Using-Google-Vision-API/blob/main/PDF_and_Image_Text_Extraction_Using_Google_Vision_API.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

1. **Run all cells** in the notebook to perform the extraction and save the results.
   - Upload your Google Cloud credentials JSON file when prompted.
   - Upload the documents (PDF or image files) you want to process to Google Colab when prompted.
