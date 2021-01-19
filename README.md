# InvoiceParser

## Overview

This project is to download the scanned pdf files from the AWS S3 bucket, extract the necessary information from them, 
and upload it to S3 bucket again.
The main part of this project is to extract the necessary information from the whole text with the OCR technology
including the Tesseract framework and AWS Textract. Also, the image processing technology
by the OpenCV framework is applied for the detection of tables in the scanned pdf document.

## Structure

- src

    The main source code for OCR, downloading and uploading, and image processing

- app

    The main execution file

- requirements

    All the dependencies for this project
    
- settings

    Several settings including files path and static values

## Installation

- Environment
    
    Ubuntu 18.04, Windows 10, Python 3.6

- Dependency Installation

    Please run the following command in this project directory in the terminal.
    ```
    pip3 install -r requirements.txt
    ```

## Configuration

- Please set some configurations in config.cfg file.

    * Please set the access key id and secret access key of your S3 bucket into the access_key_id and secret_access_key 
    variable of the config file.
    
    * Please set the S3 bucket name into the s3_bucket_name variable of the config file and the full path of the scanned
    pdf document folder in the S3 bucket into the pdf_folder_object variable of the config file. 
    
## Execution

- Please run the following command in the terminal.

    ```
    python3 app.py
    ```

