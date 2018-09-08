## Disclaimer
Not sure if this method of a general windows pyvenv will work yet. If this doesn't work direcly, I will make a batch file to do everything for you instead of having to create the virtual environment yourself. But if you're interested: 
  - [How to make a Virtual Enviroment in Windows](https://programwithus.com/learn-to-code/Pip-and-virtualenv-on-Windows/)
  - [How to install custom packages into venv](https://packaging.python.org/guides/installing-using-pip-and-virtualenv/)

# Making Your Virtual Environment (Windows)

## Steps in Any Shell:
  1. Download [Python 3.7](https://www.python.org/ftp/python/3.7.0/python-3.7.0-amd64.exe) 
      - If you enter `python` in your shell, it should say 'Python 3.7.0'. If not, try `python3` and see if that works. If it does change all `python` to `python3` in commands.
      - Most likely this project will work on any Python3, but to be safe, we'll standardize it to Python 3.7
  2. Upgrade pip (the defauly pip is probably behind)
      - `python -m pip install --upgrade pip`
  3. Download virtualenvwrapper package.
      - `pip install virtualenv`
      - `pip install virtualenvwrapper`
  4. Move to where you put requirements.txt
      - `cd /path/to/syllashare-pyvenv/`
  5. Make Virtual Environment
      - `mkvirtualenv syllashare`
  6. You should now be in the virtual environment ('(syllashare)' should be in the command line):
      - To Activate: `workon syllashare`
      - To Deactivate: `deactivate`
  7. Install required packages to venv (make sure you're in the venv):
      - `pip install -U -r requirements.txt `
  8. Verify that all the packages were installed:
      - `pip list`
  
## Libraries Included in this Virtual Environment:
  - [Django](https://docs.djangoproject.com/en/2.1/) - Web Backend Framework
  - [Requests](http://docs.python-requests.org/en/master/user/quickstart/) - HTTP library for Python
  - [Pillow](https://pillow.readthedocs.io/en/latest/) - Fork of the Python Imaging Library. This is required for pytessaract
  - [Python-tesseract](https://pypi.org/project/pytesseract/) - Python Wrapper for Google's Tesseract-OCR Engine
  - [Beautiful Soup 4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - An HTML/XML Parser. 
  - [NumPy](https://docs.scipy.org/doc/numpy/user/quickstart.html) - An Advanced Math and Computation Efficiency library 
  - [Matplotlib](https://matplotlib.org/api/pyplot_summary.html) - A 2d plotting library
  
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
