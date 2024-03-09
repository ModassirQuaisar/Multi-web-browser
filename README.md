Creating a Simple Web Browser with Python and PyQT

In this Python project, we will create GUI-based Web Browser using the Tkinter and Selenium modules. It is a beginner level project, where you will use the webdriver API with tkinter and apply them in real life. Let’s get started!

About Web Browser:
You don’t know what web browsers are?

A web browser is a software program that allows you to access the internet and all the web pages in it.
Most common web browsers are Google Chrome, Microsoft Edge, Brave, Firefox, and Safari, and you are most definitely reading this article in one of these.

About the project:
The objective of this Python project is to create a GUI based Web Browser. To build this, you must have intermediate understanding of the PyQt5 library, and its modules, including the WebEngineWidgets module that you will need to install separately.

Project Prerequisites:
To build this Python Web Browser project, we will need the following libraries:


1. PyQt5 – To create the GUI.
2. sys.argv – To get the inputs entered from the command line
3. PyQt5.QtCore.QUrl – The QUrl class will be used to convert string objects to a Qt acceptable URL object that will navigate through all the websites.
4. PyQt5.QtWidgets – To get the Widgets, including but not limited to:
a. QAction – This widget allots an abstract user interface action to widgets in the form of text.
b. QLineEdit – Single line input box [Tkinter alternative: Entry widget]
c. QToolbar – This widget is used to add a frame-like container to the top of the window.
5. PyQt5.QtWebEngineWidgets.QWebEngineView – It is used to load the content of a website directly from the internet.


The PyQT5 library does not come installed with Python, and the QtWebEngineWidgets module does not come installed with the PyQt5 library, so we will need to run the following command in the command terminal to install them:

python -m pip install pyqt5 qtwebengine
