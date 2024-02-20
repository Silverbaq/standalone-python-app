
## Setup project
`py2applet --make-setup main.py`

## Clean up your build directories
`rm -rf build dist`

## Building for deployment
`python setup.py py2app -A`


## Run application
`./dist/main.app/Contents/MacOS/main`

To start your application normally with LaunchServices, you can use the open tool:
`open -a dist/main.app`


--- 

### Building it "manually"
`pyinstaller --onedir main.py`

### Additional options
* No console (only GUI): `--noconsole`
* Apply an icon: `--icon icon.ico`


### Official documentation
https://py2app.readthedocs.io/en/latest/tutorial.html