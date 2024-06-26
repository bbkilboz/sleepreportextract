# SleepReportExtract
Extracts information from polysomnography reports generated by Compumedics Profusion and Natus Embla RemLogic software, and then exports the data to an Excel file.
 
The two Jupyter Notebooks contains Python script for processing DOCX and RTF reports for Compumedics Profusion and PDF for Natus Embla RemLogic. The script extracts relevant information from the documents and consolidates the data into a pandas DataFrame, exports as an Excel Worksheet (xlsx). 

## Features

- (For Profusion) Extracts text from DOC and DOCX files using `olefile` and `python-docx`.
- (For RemLogic) Extracts text from PDF files using `PyMuPDF`, also look for a DOC/DOCX file with the same name for extracting diagnosis. 
- Corrects Turkish characters in the extracted text.
- Uses `tqdm` for progress bars during file processing.

## Prerequisites

- Python 3.x
- pandas
- python-docx
- PyMuPDF
- olefile
- tqdm

## Installation & Usage

1. Clone the repository:

   ```sh
   git clone https://github.com/bbkilboz/sleepreportextract.git

2. Open the desired Jupyter Notebook (for Profusion or Embla-RemLogic)
3. Edit file_path and also keywords arrays.
4. Run the notebook.

Compumedics Profusion and Natus Embla RemLogic are trademarks of their respective owners, and I am not affiliated with them.
