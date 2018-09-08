# Making Your Virtual Environment
  1. Download Python 3.7.
     - Windows
       - [Windows Python 3.7 Download](https://www.python.org/ftp/python/3.7.0/python-3.7.0-amd64.exe).
       - If you enter `python` or `py` in your shell, it should say 'Python 3.7.0'. If not, try `python3` and see if that works. If it does change all `python` to `python3` in commands. (ctrl+z Enter or 'quit' to exit)
     - Mac
       - [Mac >10.9 Python 3.7 Download](https://www.python.org/ftp/python/3.7.0/python-3.7.0-macosx10.9.pkg).
       - If you enter `python` or `py` in your shell, it should say 'Python 3.7.0' ('ctrl+d or 'quit' to exit)
     - Linux
       - `sudo apt-get python3.7`
     - Note: Most likely this project will work with any Python 3 interpreter, but to be safe, we'll standardize it to Python 3.7
     
  2. Upgrade pip. (the default pip is probably behind)
     - `python -m pip install --upgrade pip`
     
  3. Download virtualenvwrapper package.
     - `pip install virtualenv` - This package creates the virtualenvs
     - Windows:
       - `pip install virtualenvwrapper-win`
     - Mac/Linux:
       - `pip install virtualenvwrapper`
     
  4. Move to where you put requirements.txt.
     - `cd /path/to/syllashare-pyvenv/`
     
  5. Make Virtual Environment.
     - `mkvirtualenv syllashare`
     
  6. You should now be in the virtual environment ('(syllashare)' should be in the command line).
     - For future use:
       - To Activate: `workon syllashare`
       - To Deactivate: `deactivate`
     
  7. Install required packages to venv (make sure you're in the venv).
     - `pip install -U -r requirements.txt `
     
  8. Verify that all the packages were installed.
     - `pip list`
     
  9. Install Tesseract-OCR binaries:
     - Windows
       - [Tessaract 4 Download](https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-v4.0.0-beta.1.20180608.exe)
     - Mac
       - Install [Homebrew](https://brew.sh/) if you don't already.
         - `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
       - `brew install tesseract`
     - Linux
       - `sudo apt install tesseract-ocr`
       - `sudo apt install libtesseract-dev`
  
  10. Do Work!
     - Check out my Python Tutorial - [Here](https://github.com/Tryst480/python-tutorial)
 
## Configuring Pycharm
  1. Locate absolute path to virtual environment you created.
     - Generally with mkvirtualenv it's located in `C:\Users\{Your Name}\Envs\syllashare\Scripts\python.exe`
  2. Either Open new project or open syllashare main repo.
  3. In **File > Settings > Project > Project Interpreter** 
     - **Click Cog Wheel > Add Local**
     - **Existing Environment > ...**
     - Find `python.exe` from (1) in file picker
     - **Check: Make Available For All Projcets > Ok > Apply**
  4. How to run Python files in Pycharm:
     - **Right Click testFile.py tab > Run 'testFile'**
     - if there's a `if __name__ == '__main__':` in the file:
       - **Click Green Arrow > Run 'testFile'**
  
### If Using Any Other IDE/Text Editor for Python Development
  1. Stop
  2. Download [PyCharm](https://www.jetbrains.com/pycharm/download/download-thanks.html?platform=windows&code=PCC)
  3. See above

  
## Libraries Included in this Virtual Environment:
  - [Django](https://docs.djangoproject.com/en/2.1/) - Web backend framework
  - [Requests](http://docs.python-requests.org/en/master/user/quickstart/) - HTTP library for Python
  - [Pillow](https://pillow.readthedocs.io/en/latest/) - Fork of the Python Imaging Library. This is required for pytessaract
  - [Python-tesseract](https://pypi.org/project/pytesseract/) - Python wrapper for Google's Tesseract-OCR Engine
  - [Pdf2Image](https://pypi.org/project/pdf2image/) - Package to turn pdfs into images
  - [Beautiful Soup 4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - An HTML/XML parsing package
  - [NumPy](https://docs.scipy.org/doc/numpy/user/quickstart.html) - An advanced math and computation ibrary 
  - [Matplotlib](https://matplotlib.org/api/pyplot_summary.html) - A 2d plotting library
  
### Other Helpful Links
  - [How to make a Virtual Enviroment in Windows](https://programwithus.com/learn-to-code/Pip-and-virtualenv-on-Windows/)
  - [How to install custom packages into venv](https://packaging.python.org/guides/installing-using-pip-and-virtualenv/)
  - [How to install tesseract](https://github.com/tesseract-ocr/tesseract/wiki)

  ##### If you're having any other issues, please buy a Mac.
