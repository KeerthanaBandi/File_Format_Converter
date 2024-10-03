# CSV to JSON File Format Converter

## Overview

This project is a Python-based tool designed to convert CSV files to JSON format. It includes schema-based column mapping to ensure accurate data transformation and supports batch processing of files in specified directories.

## Features

- Convert CSV files to JSON with customizable schema-based column mapping.
- Batch processing of multiple CSV files in a directory.
- Schema validation to ensure proper conversion.
- Support for reading and applying schemas from a JSON file.
- Handles large datasets with efficient processing using `pandas`.

## Requirements

- Python 3.x
- pandas
- glob
- json
- re

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/csv-to-json-converter.git
    ```

2. Navigate to the project directory:

    ```bash
    cd csv-to-json-converter
    ```

3. Install dependencies:

    ```bash
    pip install pandas
    ```

## Usage

1. Prepare your schemas: Make sure you have a `schemas.json` file that defines the structure of the columns in your CSV files.

2. Set environment variables for your source and target directories:

    ```bash
    export SRC_BASE_DIR=path_to_your_csv_files
    export TGT_BASE_DIR=path_to_your_output_json
    ```

3. Run the script:

    - To convert all datasets based on schemas:

    ```bash
    python app.py
    ```

    - To convert specific datasets:

    ```bash
    python app.py '["dataset1", "dataset2"]'
    ```

## Project Structure

