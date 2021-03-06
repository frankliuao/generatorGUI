# generatorGUI

Edit parameters for the Astra generator program and run generator using a GUI.

### Purpose
Summarizes all the parameters for Astra generator in a table and displays it in 
the PyQt 
environment.

The parameters are saved in an *Excel* format. The user can start from a 
blank "all-default" table, or load an Excel file with parameters already 
defined in it. The parameters can be changed and saved again to the Excel 
spreadsheet.

When all the necessary parameters are defined in the PyQt table, simply click
 "Run" to execute the Astra generator. 

### Usage

The script can be executed in two ways. Both ways require some basic 
information about how to run Python scripts, of course.

* Option 1: **Run script from command line**
    ```BASH
    > python /path/to/your/pip/installation/generatorGUI/main.py
    ```
    For instance, on my OSX I used `pip` installed by *anaconda*, such that 
    the packages are installed in my *anaconda* diretory. So for me:
    ```BASH
    > python  ~/anaconda3/lib/python3.7/site-packages/generatorGUI/main.py
    ```
* Option 2: **Import the module and run the main function**
    You can also run the GUI from the Python prompt, or *Jupyter notebook*, 
    for instance:
    ```Python
    >>> import generatorGUI
    >>> generatorGUI.main()  
    ```

For each of the parameters, the *type*, *unit*, and *default* have already 
been defined. Do not change the values in those cells. If a parameter needs 
to be modified from its default value, enter the correct value in the *set* 
column.

Notice, that for *str* type, the value does not need the single quotes ' 
around the string; the *list_?* type asks for a list of *?* type values: e.g.
 for *list_float* you can put `[1.0, 2.0, 3.0]`, just like a *Python list*, 
 for *list_str*, single quotes ' are not needed either: e.g. `[abc.dat, foo
 .dat]`.

####A note on the parameter *fname*
Notice that by default the *generator* program will be called from the 
current working directory, i.e. where you run the **main.py** script. If only
 a file name is 


### Installation
Install easyexception using `pip`, or `pip3`

    pip install generatorGUI

### Repository
[GitHub page](https://github.com/frankliuao/generatorGUI)
