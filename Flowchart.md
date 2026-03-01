# 3D Model Generation Pipeline (PDF → Digital Twin)

## Overview

This pipeline automates the process of generating 3D models from PDF
files for Digital Twin creation.

------------------------------------------------------------------------

## Flowchart

``` mermaid
flowchart TD
    A[Input: PDF File] --> B[Parse Entire PDF]
    B --> C[Extract Required Pages]
    C --> D[Extract Essential Data]
    D --> E[Convert Data to JSON]
    E --> F[Pass JSON to AutoLISP Script]
    F --> G[Use Pre-made CAD Blocks]
    G --> H[Generate 3D Model]
```

------------------------------------------------------------------------

## Step-by-Step Process

1.  **Input PDF**\
    The system receives a PDF containing design or structural data.

2.  **PDF Parsing**\
    The entire PDF is parsed to identify and extract relevant pages.

3.  **Data Extraction**\
    Essential structured data is extracted from the selected pages.

4.  **JSON Conversion**\
    Extracted data is converted into a structured JSON format.

5.  **AutoLISP Execution**\
    The JSON file is passed to an AutoLISP script.

6.  **Block-Based Model Creation**\
    Pre-made CAD blocks are programmatically arranged and generated.

7.  **3D Model Output**\
    Final 3D model is generated and ready for Digital Twin integration.
