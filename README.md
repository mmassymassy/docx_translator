# Description:
This script provides a simple GUI to translate documents from French to English using the Google Translate API.
As many websites have a limit on the number of characters that can be translated at once, this script reads the document in chunks of 5000 characters and translates each chunk separately.
# Advantages:
- Easy to use GUI
- Supports multiple document formats (docx, doc, odt)
- Handles large documents by splitting them into manageable chunks
- Saves the text in the same format as the original document
- In case of error, it will print #error# in your document so you can easily find the error location
# Requirements:
- Python 3.x
- python-docx for .docx files
- googletrans for translation
- odfpy for .odt files
# Installation:
```bash
    pip install python-docx googletrans odfpy
```
Or you can use the provided `requirements.txt` file to install all dependencies at once:
```bash
    pip install -r requirements.txt
```
You also need tkinter for the GUI, which is usually included with Python installations. If you don't have it, you can install it using your package manager (e.g., `apt-get install python3-tk` on Debian-based systems), and for Windows, it should be included with the Python installation.


# How it works :
1. install the required packages
```bash
pip install -r requirements.txt
```
2. run the script
```bash
python gui.py
```
3. Select the docx/doc/odt file you want to translate from french to english
4. Click on the "Translate" button
5. The translated file will be saved in the same directory as the original file with "_translated" appended to the filename.