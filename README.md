PyQt\PySide helper for Houdini
--------------------------

![alt tag](http://paulwinex.ru/files/download/hqtScreen.jpg)


[paulpinex.ru](http://paulwinex.ru)

This script enables you to use PySide or PyQt4 with Houdini. Main differences from default pyqt_houdini.py are:

  - opportunity to have several widgets open at the same time
  
  - automaticly apply Houdini-style ui design

  - implemented 3 different modes. It is not required other functions , rather your widget inherits from one of following classes :
    - widget: a simple window opening . Works if the widget is created from QWidget or QMainWindow. Main function showUi returns a pointer to widget object.
    - dialog: opens the window blocks Houdinis window. To do this you need to create a widget that inherits from QDialog. showUi returns result of the dialogue (bool) and a pointer to the dialogue object.
    - menu: If the widget is inherited from QMenu, the menu will open at the current cursor position . showUi returns a pointer to the selected QAction
        
### Install:

  - Install PySide or PyQt4 to default Python library or to Houdini python library

  - Copy hqt.py to PYTHONPATH or PATH. For example:

$HFS\python27\lib\site-packages\hqt.py

<pre><code>import hqt
help(hqt)</code></pre>

See hqt_example.py for details.


