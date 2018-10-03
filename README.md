
# ![logo](./studiolibrary/resource/icons/icon_black_on_white.png) Studio Library

A Free tool written in python for managing poses and animation in Maya.


## Features

* Save poses and animation
* Mirror poses and animation
* Create easy to use selection sets
* MMB drag for fast pose blending
* LMB drag and drop to organize items
* Insert, merge and replace animation
* Supports Windows, Linux and OSX
* Supports Maya 2016, 2017 and 2018


## Contributing

Contributions to Studio Library are always welcome! Whether it's reporting bugs, feature requests, discussing ideas or committing code.

We follow the below guides for...

* [Commit messages style](https://github.com/erlang/otp/wiki/Writing-good-commit-messages)

* [GitHub Forking Workflow](https://gist.github.com/Chaser324/ce0505fbed06b947d962)

* [Python Qt Style Guidelines](http://bitesofcode.blogspot.co.uk/2011/10/pyqt-coding-style-guidelines.html)


## Downloading

Download and unzip the *studiolibrary.zip* file from [github releases](https://github.com/krathjen/studiolibrary/releases) or [website](http://www.studiolibrary.com/download).


## Intallation

# maya-module-installer
Module template for easy drag-and-drop installation using provided mel script.

## Description
Add the module which is located in the same directory as the .mel file into the first available `MAYA_MODULE_PATH` directory. It doesn't matter where on disk the module lives as the script will make sure the path in the .mod file links to the correct place. There are some basic sanity checks in place to make sure the script doesn't error out. This includes Maya version compatibility with the module. Permissions of the directories files have to be written to and incorrectly formatted module files.

The reason for creating this script is that I have always had trouble finding a good way to distribute scripts. Especially less technical users might have trouble running python/mel code. This method will make it as easy as unpacking the package anywhere on disk and dragging the provided mel file into Maya. The template maya module file can be specific to certain versions of maya, language and operating system. It is also possible to extend the environment variables and adding a userSetup.py. This flexibility will allow you to run code on startup and provide the users with for example a custom shelf that is easily accessible to the user.

## Requires
* Template .mod file ( place `<PATH>` where normally the file path would go )
* Maya module ( scripts/icons/plug-ins directories etc. )

## Usage
<p align="center"><img src="icons/moduleInstallerExample.gif?raw=true"></p>

Drag and drop the mel file into Maya or run `source <MEL_FILE>;`.

## Maya Module Documentation
* [Maya Documentation: Distributing Multi-File Modules](https://help.autodesk.com/view/MAYAUL/2018/ENU/?guid=__files_GUID_CB76E356_753B_4837_8C5B_3296C14872CA_htm)
* [Maya Documentation: Maya module paths, folders and versions](https://help.autodesk.com/view/MAYAUL/2018/ENU/?guid=__files_GUID_130A3F57_2A5D_4E56_B066_6B86F68EEA22_htm)


## Setup

Start Maya and run the following code in the **Python** script editor.

```python
import studiolibrary
studiolibrary.main()
```

## Documentation

Find the latest documentation [here](https://drive.google.com/open?id=1v3A1YWEdJml_Qb7i8ITOrljqZaBISHYZCKUR9NJxGr8).

## Tutorials

How to use

* [poses](https://www.youtube.com/watch?v=lpaWrT7VXfM)
* [selection sets](https://www.youtube.com/watch?v=xejWubal_j8)
* [mirror tables](https://www.youtube.com/watch?v=kCv0XleJfjU&t=3s)

## License

The Studio Library is free to use in production under the GNU Lesser General Public License v3.0.
For more information please click [here](https://github.com/krathjen/studiolibrary/blob/master/LICENSE.md).


## Issues

Feel free to raise an issue with the error message and a detailed step by step process of how you got the error in [github issues](https://github.com/krathjen/studiolibrary/issues/new) or contact [krathjen](http://www.studiolibrary.com/contact).
