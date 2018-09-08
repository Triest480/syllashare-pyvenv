## Disclaimer
Not sure if this method of a general windows pyvenv will work yet. If this doesn't work direcly, I will make a batch file to do everything for you instead of having to create the virtual environment yourself. But if you're interested: 
  - [How to make a Virtual Enviroment in Windows](https://programwithus.com/learn-to-code/Pip-and-virtualenv-on-Windows/)
  - [How to install custom packages into venv](https://packaging.python.org/guides/installing-using-pip-and-virtualenv/)

# syllashare-pyvenv-win

## Requirement Before Downloading Repository:
  - [Python 3.7](https://www.python.org/ftp/python/3.7.0/python-3.7.0-amd64.exe) - Most likely any version of Python3 will work but this venv was created with python3.7.
  
## Libraries Included in this Virtual Environment:
  - [Django](https://docs.djangoproject.com/en/2.1/) - Web Backend Framework
  - [Requests](http://docs.python-requests.org/en/master/user/quickstart/) - HTTP library for Python
  - [Pillow](https://pillow.readthedocs.io/en/latest/) - Fork of the Python Imaging Library. This is required for pytessaract
  - [Python-tesseract](https://pypi.org/project/pytesseract/) - Python Wrapper for Google's Tesseract-OCR Engine
  - [Beautiful Soup 4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - An HTML/XML Parser. 
  - [NumPy](https://docs.scipy.org/doc/numpy/user/quickstart.html) - An Advanced Math and Computation Efficiency library 
  - [Matplotlib](https://matplotlib.org/api/pyplot_summary.html) - A 2d plotting library

## How To Use Virtual Environment:
  ### On Command Line
  1. In ***Command Prompt***: '`\path\to\env\syllashare-pyvenv-win\syllashare\Scripts\activate`'
  2. You should now be in the virtual environment. (There should be a (syllashare) in the command line)
  3. In ***Command Prompt***: '`pip list`' to verify if all packages are installed in virtual environment
  4. Do Work on command line interface:
     - Call a Python file: '`py myTestfile.py`'
  
  5. To Exit Virtual Environment:
     -  In ***Command Prompt***: '`cd ~\(DOWNLOAD_PATH)\syllashare-pyvenv-win\syllashare\Scripts\`'
     -  In ***Command Prompt***: '`call deactivate.bat`'
  6. Or you can just exit the Command Prompt
  
  ### Using PyCharm
  1. Locate absolute path to: '`\path\to\env\syllashare-pyvenv-win\syllashare\Scripts\python.exe`'
  2. Either Open new project or open SyllaScan main repo
  3. In **File > Settings > Project > Project Interpreter** 
     - **Click Cog Wheel > Add Local**
     - **Existing Environment > ...**
     - Find `python.exe` from (1) in file picker
     - **Check: Make Available For All Projcets > Ok > Apply**
  4. How to run Python files in Pycharm:
     - **Right Click testFile.py tab > Run 'testFile'**
     - if there's a `if __name__ == '__main__':` in the file
       - **Click Green Arrow > Run 'testFile'**
  
  ### Using Any Other IDE/Text Editor
  1. Stop
  2. Download [Pycharm](https://www.jetbrains.com/pycharm/download/download-thanks.html?platform=windows&code=PCC)
  3. See above
  
  ##### If you're having any other issues, please buy a Mac.
