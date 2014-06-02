PySide helper for Houdini
--------------------------

![alt tag](http://paulwinex.ru/files/download/hqtScreen.jpg)

by PaylWinex

This script enables you to use PySide with Houdini. Main differences from default pyqt_houdini.py are:

  - opportunity to have several widgets open at the same time
  
  - automaticly apply Houdini-style ui design

  - implemented 3 methods of execute widgets. For use it, just inherit your widget from correct class.


### Install:

  - Install PySide to default Python library or to Houdini python library

  - Copy hqt.py to PYTHONPATH or PATH. For example:

$HFS\python27\lib\site-packages\hqt.py

<pre><code>import hqt
help(hqt)</code></pre>

See hqt_example.py for details.


