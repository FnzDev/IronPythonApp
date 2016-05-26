# IronPythonApp
Test playing with IronPython and Castle.Windsor. Basically two projects.

Foo - has following classes:
- Bar: exposes a single method Dork(), implements interface IBar
- PythonInstaller: registers a IBar and its implementation Bar
- PythonWindsor: wrapper for PythonInstaller, since im not sure if possible to do Container.Resolve\<IBar>() in python

IronPythonApp
- uses PythonWindsor and Castle.Windsor to resolve an IBar and returns the object to python - calls it
