# py-gdx

## 1. What?

py-gdx is a small set of Python utilities for manipulating [GAMS](http://www.gams.com) GDX files.
It uses the Python bindings available in recent (as of 2011) versions of GAMS.
py-gdx in released under the [MIT Licence](http://www.opensource.org/licenses/mit-license.php).

There are several example scripts:

- `gdx_replace_csv.py` replaces a variable in the GDX file with data in a CSV file
- `gdx_merge.py` merges two GDX files *without* creating an extra index
- `gdx_report.py` produces a CSV report of parameter and variable values in a GDX file

In call cases use `python gdx_<example>.py --help` to find out to use them.

The above scripts use `gdxdict.py` to do their magic.  `gdxdict.py` loads a
GDX file into a Python dictionary, and can write a GDX file from a dictionary.

At the moment, documentation of `gdxdict.py` is limited to the example files.


## 2. Requirements

- a "recent" version of GAMS or at least the GDX library - GAMS 23.2 does not have Python bindings, 23.7 does.
- Python 2.6 - the GDX bindings do not seem to support Python 3 or 2.7.
- The path to the relevant files on your PythonPath - on Windows this is like `\C:\Program Files\GAMS23.7\apifiles\gdx`


## 3. Who?

py-gdx was developed by [Incremental](http://www.incremental.co.nz/)
with support from the [Electricity Authority](http://www.ea.govt.nz/)
You can contact us at <info@incremental.co.nz>.