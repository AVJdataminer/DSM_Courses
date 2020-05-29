---
title: Objects and modules
author: Thinkful
team: grading
time: 120 minutes
uuid: 186cc634-f4ac-4ead-8502-90eb3357e4c2
timeHours: 2
---
## Working with Modules
Knowing what modules are and working with them can be two different things all together. So, let's breakdown how you work with modules. 

Check to see if the module you would like is installed. Note* These commands must be run in a terminal or caommand line window. In order to run them from within Jupyter notebooks place an exclamation mark in front of the command. `
pip list | grep <module_name_you_want_to_check>
` If you installed Python using Anaconda many common packages you will want to use such as Numpy will already be installed. You can get the entire list of modules installed in your current Python environment using `pip list` or in Jupyter `!pip list`

### Installing modules
Let's say you wanted to install the Geopandas module for working with spatial data in Python. There are three essential ways to install a package and the one you choose depends on your current Python management setup and preferrence. 

 1. If you use the conda package manager `conda install geopoandas`
 2. If you prefer pip `pip install geopandas`
 3. Finally if you'd like to install directly from the source `pip install git+git://github.com/geopandas/geopandas.git`

If you're installing a module directly from Jupyter notebook using pip you would start a new cell and type `!pip install geopandas`. 

### Loading modules
 Once you have the packages you need installed, you need to load them by running import commands. For example to load Pandas we type `import pandas as pd` and now anytime we want to call a function that's available in the pandas module we preface it with `pd.` to indicate as such. Module import statements should be at the beginning of your program or jupyter notebook with one statement per line, such as:
 
 `import numpy as np`
`import pandas as pd`
`import scipy` 
`from datetime import datetime`

Those with `from` statements are absolute imports which only load the specified function from the module rather than all the functions in that module. These are recommended when you only need one or two functions from a module as they result in more understandable error messages and cleaner code.

### Dependencies
Some packages will have dependencies, i.e. other modules they depend on in order to run properly. You can check the dependencies of a package using the `pip show module_name` command. When installing a package you may encouter a missing dependent module for the package you're trying to install. Simply install the dependent modules first and then proceed with installing the module you would like to use. The package documentation will most likely list the core dependent and optional dependent packages see the [GeoPandas page](https://geopandas.org/install.html) for an example.

 If you encounter a module loading error it is likely a dependent package missing or if running code from someone else it might be a missing module all together. If you can't discern what the error is indicating, search for the message on [Stackoverflow](https://stackoverflow.com/questions/tagged/python). Most likely someone else has posted the same error and you will find community reponses to help. 
 

## Objects
It's time to talk about something you've been using every time you write Python, but that you may not have been thinking about: objects.

You've been using objects all along because _everything in Python_ is an object. 

Integers? Objects. 

Strings? Objects. 

Lists, dictionaries, Booleans... even functions. All of these are objects.

Objects and "object-oriented programming" are deep topics that cut to the core of Python and computer science. 

Mainly, you need to recognize objects when you see them and know how to interact with them in your code. Let's practice in the below notebook.

<jupyter notebook-name="working_with_objects_modules_libraries" course-code="DSBC"></jupyter>
