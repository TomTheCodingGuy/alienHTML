# alienHtml
- A Python package to help with HTML development.

## Features
- Creates a HTML file in a specified directory.
- Helps you edit it through functions and parameters.
- Allows you to open the HTML file in your browser with one simple function.
- You can edit an already existing file, or create a new one.
- Indentation!

## Install:
```
pip install alienHTML
```
- Latest version:
```
pip install alienHTML==0.0.5
```

## Example:
```python
from alienHTML import *

# "w" is the mode to open, in this case write. 
mypage = WebPage("/path/to/file/to/create/or/edit", "w", tabhead="Hello World", bgcolour="powderblue",icon="path/to/icon.ico")
# If you put it as "a" it switches to edit mode
# For tabhead, bgcolour and icon, if not set it will automatically set itself to some defaults.

# This creates a heading of the largest size as the number is one.
# It will ask you where you want it in the <body> section of your code
mypage.Heading("Hello World",1)
# Similar for images, just with different parameters. The second is the alt text.
mypage.Image("/path/to/image.png", "Image!")

mypage.showfile() # Prints the contents of the file with line numbers and indentation.
mypage.openpage() # Opens the HTML file in web browser.						             
```
Outputs:

- Ask you where to put code for heading and image.
- Prints the file in shell.
- Opens the page in a web browser

## Tips:
- If you do not have a .ico file, you can use https://cloudconvert.com to convert any image files to .ico.
- This is designed to help people learn HTML, and is not recommened for advanced web development.
## To do:

- Add more web page features.
- Make the showfile function open the HTML file in web browser, so there is syntax highlighting.

## Credits:

- Made by TomTheCodingGuy
