# Tips for using web2py on OSX


## Location of application files

All application files are stored in a folder in the main web2py.app application. This can make them a little tricky to get at. 

On macbook pro they are located here:
```bash
/.../Applications/web2py.app/Contents/applications/[appname]
```

## using web2py from the command line
The web2py is in the app executable to use it from the command line it must either be referenced explicitly or the executable must be exported to the PATH.

option 1: explicit referencing
```bash
#This would create a new app with the name of [appname]
/Applications/web2py.app/Contents/MacOS/web2py -S [appname]
```

option 2: export the location of the web2py app to the environment
```bash
#Add this line to the ~/.bash_profile file
export PATH=/Volumes/SSD/Applications/mongodb/bin:$PATH
```

note on Linux the bash profile is ~/.bashrc

# Use of Python environment with Web2Py
In theory it is possible to use web2py with any python build. In practice it is sensible to use 2.7

#Selenium
Install selnium (if using Conda then will need ot choose a compatible version with the firefox browser chosen).
