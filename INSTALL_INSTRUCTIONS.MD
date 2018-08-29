##Cantera example notebook install instructions

**Last updated Fall 2018 by James L Urban**

To use the notebooks in this repository, you’ll need to download 
Python, the Jupyter notebook interface, and some Python packages. 
The easiest way to do this for all major operating systems is to 
use the Anaconda package manager, and we provide these 
instructions here. 


### Step 1: Install Anaconda

These Cantera notebooks require the Python programming environment 
to operate. The Python programming environment can be installed 
using Anaconda. Download Anaconda at the following URL: 

https://www.anaconda.com/download/ 

Make sure to download the version for Python 2.7. Do NOT download 
the version for Python 3.x. If you are using macOS, click the 
Graphical Installer button.

For Windows, After installing Anaconda, search for “anaconda 
prompt” and click on “Anaconda Prompt” and an anaconda prompt 
terminal window should open on your computer. 

For macOS, simply open the Terminal application. 

You will want to run the following command:

`conda update conda`

If there is an update available, there will be a prompt to
download updates. If this happens, type y  and then <enter>. Then 
type in the command:

`conda update numpy`

This will import numpy, a software package with functions and
routines very similar to MATLAB. Then we will install/update 
Jupyter, which is a notebook interface for Python:

`conda update jupyter`

### Step 2: Install Cantera

To install Cantera, you need to type in the Anaconda command line:

`conda install --channel cantera cantera`

Some of the notebooks (those for reaction path analysis) make use 
of the graphviz package, which is installed with the following 
command:

`conda install -c anaconda graphviz=2.38.0`

This is not necessary to run Cantera, so you can skip this step if 
you do not plan on looking at reaction path analysis. 

### Step 3: Open Jupyter notebook

The notebooks are part of this GitHub repository, and the most 
updated versions are located at the following URL:

https://github.com/JLUrban/Cantera-Example-Notebooks 

Either in the Windows Command Prompt, or the macOS Terminal, or a 
Linux terminal, type:

`jupyter notebook`

A notebook interface should open in a browser window at the URL:

http://localhost:8888/tree

You should click on the folders where you saved/cloned the 
repository. For example, if you saved it in “Documents,” click 
“Documents,” etc. Click “[Cantera] Adiabatic Flame Temperature” 
which will open that notebook in a new window.  This notebook 
includes pre-made Cantera code so that you can see how Cantera 
works without typing any code yourself. You can run the code 
blocks by pressing <shift> + <enter> which will run the selected 
code block. 

Feel free to try changing parts of the code to see what happens if 
you remove the nitrogen from the mixture or what happens if you 
change the fuel. Make sure to keep an original version for 
reference!

### Step 4: Close Jupyter notebook

When you are finished with the Jupyter notebook, you will close it 
in your browser. For Windows, shutdown the Notebook by opening the 
terminal window for Jupyter and type: 

`<ctrl> + c` 

and then type 

`y` 

followed by 

<enter> 

to  shutdown Jupyter. For macOS, go to the Terminal and type:

`<ctrl> + c `

twice to shutdown Jupyter. 
