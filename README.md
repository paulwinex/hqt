PyQt\PySide helper for Houdini
--------------------------

![alt tag](http://www.paulwinex.ru/wp-content/uploads/2015/04/hqt.jpg)


[paulwinex.ru](http://paulwinex.ru)

### Houdini 13

This script enables you to use PySide or PyQt4 with Houdini. Main differences from default pyqt_houdini.py are:

  - opportunity to have several widgets open at the same time
  
  - automaticly apply Houdini-style ui design

  - implemented 3 different modes. It is not required other functions , rather your widget inherits from one of following classes :
    - widget: a simple window opening . Works if the widget is created from QWidget or QMainWindow. Main function showUi returns a pointer to widget object.
    - dialog: opens the window blocks Houdinis window. To do this you need to create a widget that inherits from QDialog. showUi returns result of the dialogue (bool) and a pointer to the dialogue object.
    - menu: If the widget is inherited from QMenu, the menu will open at the current cursor position . showUi returns a pointer to the selected QAction
        
### Houdini 14
        
This script help you to open PySide Widgets in Houdini 14
 
  - Open widget as child of main Houdini Window
  - Insert your widget as Houdini Python Panel without .pypanel file
  - [Fix default Houdini stylesheet examples](http://www.paulwinex.ru/hqt_release2/)
        
### Install:

  - Install PySide or PyQt4 to default Python library or to Houdini python library

  - Copy hqt.py to PYTHONPATH or PATH. For example:

$HFS/python27/lib/site-packages/hqt.py
or
$HFS/houdini/python2.7libs/hqt.py

  - Execute code:

```python
import hqt
help(hqt)
```


See [hqt_example.py](https://github.com/paulwinex/hqt/blob/master/hqt_example.py) for details.

---------------

#### Compare Houdini default stylesheet and hqt stylesheet

![alt tag](http://www.paulwinex.ru/wp-content/uploads/2015/03/compare_1.png)
![alt tag](http://www.paulwinex.ru/wp-content/uploads/2015/03/compare_2.png)
![alt tag](http://www.paulwinex.ru/wp-content/uploads/2015/03/compare_3.png)
