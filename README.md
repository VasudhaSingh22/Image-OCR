# Cheque Data Extraction using Python and Tesseract OCR

## Overview:
This project showcases a comprehensive solution for automating the extraction of essential information from a collection of cheque images. Leveraging the capabilities of Python, OpenCV, Tesseract OCR, Pandas, and Pillow, this script extracts crucial details such as the bank name, cheque date, and cheque amount from each image. The extracted data is structured, organized, and exported to an Excel file, simplifying the process of managing multiple cheques.

## Features:
- **Image Preprocessing with OpenCV**: OpenCV, a powerful computer vision library, is employed for image preprocessing. Techniques such as grayscale conversion, Gaussian blur, and thresholding are applied to enhance OCR accuracy, ensuring optimal text extraction from images.

- **Text Extraction using Tesseract OCR**: Tesseract OCR, a widely-used optical character recognition engine, is harnessed to extract textual content from the processed cheque images. This enables accurate retrieval of critical information, making data extraction efficient and reliable.

- **Data Structuring with Pandas**: Extracted data, including bank names, cheque dates, and cheque amounts, is organized into a structured format using the Pandas library. This structured data is presented in a DataFrame, allowing for seamless manipulation, analysis, and export to various formats.

- **Image Handling with Pillow**: The Pillow library is used for opening, manipulating, and saving images. It aids in converting images to grayscale and performing various image-related operations.

## Usage:
1. **Setup**: Begin by cloning this repository to your local machine. Install the required dependencies by executing the following command: `pip install opencv-python pytesseract pandas pillow`.

2. **Data Input**: Place the cheque images you wish to process in the designated `Output` folder.

3. **Configuration**: Open the provided Python script and update the `image_path` variable with the path to your input image.

4. **Execution**: Run the Python script. The script performs the following steps:
   - Processes each cheque image, applying image preprocessing techniques using OpenCV.
   - Extracts relevant text content from the processed images using Tesseract OCR.
   - Parses and structures the extracted data, including bank names, cheque dates, and cheque amounts.
   - Saves individual cheque images with filenames corresponding to their bank names in the `Output` folder.
   - Exports the structured data to an Excel file.

5. **Output**: Upon completion, the script generates an Excel file containing the organized data. Additionally, processed cheque images are saved as separate files in the `Output` folder.

## Requirements:
- Python 3.x
- OpenCV: A powerful computer vision library for image processing tasks. Used for image preprocessing and manipulation.
- Tesseract OCR: A versatile optical character recognition engine. Utilized for extracting text content from images.
- Pandas: A data manipulation and analysis library. Used to structure, manipulate, and export data.
- Pillow: A library for opening, manipulating, and saving images. Applied for various image-related tasks.

## Additional Notes:
- The preprocessing steps in the code enhance OCR accuracy by converting images to grayscale, applying Gaussian blur, and thresholding.
- Regular expressions are used to extract relevant information like bank names, cheque dates, and amounts from the OCR output.
- Extracted dates are standardized to the "dd-mm-yyyy" format.
- Make sure to have Tesseract OCR installed and properly configured on your system.

## Further Enhancements:
This project serves as a foundation for advanced enhancements and customization. Consider exploring the following possibilities:
- Implement additional image preprocessing techniques to further optimize OCR accuracy.
- Extend the script to handle diverse cheque formats and layouts.
- Enhance the Excel output with additional formatting and visualization options.
- Integrate data validation checks to ensure the accuracy of extracted information.
- Incorporate user-defined configuration options for greater flexibility.

Contributions from the open-source community are highly encouraged. Feel free to contribute by submitting pull requests or addressing issues.

## Acknowledgments:
I extend my appreciation to the open-source communities behind Python, OpenCV, Tesseract OCR, Pandas, Pillow, and other libraries used in this project. Their dedication empowers us to develop innovative solutions and streamline data extraction processes.
