## Creating a Simple Web Browser with Python and PyQT

In this Python project, we will create GUI-based Web Browser using the Tkinter and Selenium modules. It is a beginner level project, where you will use the webdriver API with tkinter and apply them in real life. Let’s get started!

## About Web Browser:
You don’t know what web browsers are?

A web browser is a software program that allows you to access the internet and all the web pages in it.
Most common web browsers are Google Chrome, Microsoft Edge, Brave, Firefox, and Safari, and you are most definitely reading this article in one of these.

## About the project:
The objective of this Python project is to create a GUI based Web Browser. To build this, you must have intermediate understanding of the PyQt5 library, and its modules, including the WebEngineWidgets module that you will need to install separately.

## Project Prerequisites:
To build this Python Web Browser project, we will need the following libraries:


<b>1. PyQt</b> –To create the GUI.<br>
<b>2. sys.argv</b> – To get the inputs entered from the command line.<br>
<b>3. PyQt5.QtCore.QUrl</b> – The QUrl class will be used to convert string objects to a Qt acceptable URL object that will navigate through all the websites.<br>
<b>4. PyQt5.QtWidgets</b> – To get the Widgets, including but not limited to:<br>
<b>a. QAction </b>– This widget allots an abstract user interface action to widgets in the form of text.<br>
<b>b. QLineEdit</b> – Single line input box [Tkinter alternative: Entry widget]<br>
<b>c. QToolbar</b> – This widget is used to add a frame-like container to the top of the window.<br>
<b>5. PyQt5.QtWebEngineWidgets.QWebEngineView</b> – It is used to load the content of a website directly from the internet.<br>

The PyQT5 library does not come installed with Python, and the QtWebEngineWidgets module does not come installed with the PyQt5 library, so we will need to run the following command in the command terminal to install them:

```bash
python -m pip install pyqt5 qtwebengine
```

## Explanation:

We start off by creating a Window class inherited from the QMainWindow class of the PyQt5 library.
In the __init__() function, we give it all the methods, attributes of the Window class, which in turn has functions from its parent class.
Then, we go on creating the layout of the window.
Firstly, we go about setting the details of the QWebEngineView object, including its position in the main window, its initial URL, how to change the URL and the Address bar, and setting its status bar.
Then we create 2 toolbars. Add them to the window, add widgets in them and set them in two different lines.
The navigation_bar toolbar has the back, reload, home action buttons and the address bar.
The bookmarks_toolbar contains bookmarks of the websites that you want to set as bookmarks.
To add 2 toolbars in 2 separate rows, you need to use the QMainWindow.addToolBarbreak() method to add a separator that separates the two toolbars.
The QtWidgets.QAction() function is used to add a special kind of button where each command is represented as an action, which will represent our bookmarks.
The go_to_home() method is used to set the URL of the browser back to the google homepage, which is our homepage as well.
The go_to_URL() method, which takes one QUrl object as argument, is used to change the URL of the browser and in the address bar. In case the URL does not have a ‘http://’ or ‘https://’ prefix, the function will add it and then move forward with it.
To activate this method and search your URL, press the enter key on your keyboard.
The update_AddressBar() method is used to set the text of our address bar to the string version of the URL on the browser.
After creating the Window class, we will create a QApplication object, which will essentially run our window.
The QApplication.exec_() is used to run the application.

Summary
Congratulations! You have now created your own Web Browser using the PyQt5 library.

However, this is not the end of the road. This is a basic web browser, but with the power of Python, you can make it way better!
