This is simplied same pyqt5 application code to try to pass a callback function from QML/JS to python and have python (asynchronously) have JS run that function at a later time. This code causes a segfault, but I don't know why.

Best guess is QT/JS is doing garbage collection on function call and python is then running an invalid function pointer.
