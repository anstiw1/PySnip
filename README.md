# PySnip

***Please note this is a work in progress, and not yet complete!***

Text and images share a strange relationship. While we want to be able to edit documents on the fly (think Google Docs, or even MS Word), we want to send them to folks where they look best (think PDF). PDFs have a significant advantage over documents because they are multi-dimensional and can integrate text, images, vector graphics and even animations into one format. They also don't lose graphical integrity, or formatting regardless of what device they are opened on. PDFs are so secure and offer differing levels of access to protect content, and they're relatively compact for the amnount of information they contain. 

Unfortunately, PDFs have one giant drawback: the ability to edit these documents is severely limited as the original goal of the file format was to protect the contest on the page. Even extracting info from PDFs is difficult and cumbersome. 

PySnip's purpose is to read the text content on an image, and allow the user to edit in a word processor of their choosing! 

## Usage

Running ```python pysnip.py``` will open a drag-box overlay on the screen where your mouse is. At this point, using the tool is as simple as dragging and highlighting the text you want to copy. 

PySnip supports multiple languages! For example, running ```python pysnip.py rus``` will allow you to copy Russian Cyrillic text. PySnip also supports multiple languages--typing ```python pysnip eng+rus``` will let you copy text from documents that are written in both English and Russian Cyrillic. **The default language is always the user's system language.***

Using multiple languages requires the appropriate data files for Tesseract to be installed. The currently supported languages can be found [here](https://github.com/tesseract-ocr/tesseract/blob/master/doc/tesseract.1.asc#languages-and-scripts).

If you are a Windows user, I *strongly* reccomend attaching a hotkey to this tool. This can be accomplished easily by using an [AutoHotkey](https://www.autohotkey.com/) script; and pysnip.ahk contains a simple script to do this!

## Install

  * You must have [Python 3](https://www.python.org/downloads/) installed.
  * Fork & Clone this repo, and then ```cd``` into it.
  * Install the required packages and libarires with ```pip install -r requirements.txt```
  * Install [Google's Tesseract Engine](https://github.com/tesseract-ocr/tesseract) and make sure that ```tesseract``` can be reached from the command line by adding the directory to your system path.
