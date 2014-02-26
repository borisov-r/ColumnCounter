## Build procedure

Install virtual environment
```
virtualenv virtual
source virtual/bin/activate
```

Install requirements
```
pip install -r
```

Create .py file from .ui (QT user interface)
```
pyside-uic ui/columnMain.ui -o columnMain.py
```

Create .py file from .qrc (references - like icons ...)
```
pyside-rcc ui/icons.qrc -o icons_rc.py
```

Install setuptools and other softwares needed by cx_freeze
```
python ez_setup.py
```

Create stand alone application -
[example](http://www.pythonschool.net/cxfreeze_win)
```
python setup.py build
```
or create installer for windows
```
python setup.py bdist_msi
```
