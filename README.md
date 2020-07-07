# Packages-Installation-Jupyter-Notebook
How to install new packages in jupyter environment


Packages installation under python environment is always a challenging task for a newbie.Installing packages in Python is not as easy as "R".
I have struggeled alot to find a fix for the above issue. But believe me we have to take care of few things while installing new packages under python/jupyter envorimemt.

First Important thing to take care of is the "Path environment" ...... Secondly !!"Path Environment " only.

Ideally your Shell Environment [determined when Jupyter Notebook launched] and Python Executable[determined by Kernel] should be at the same path

I would recommend below steps for installing new package under Jupyter Notebook.
a)Run !type python- It shows the Python path being used in the notebook can be determined
b)Run sys.executable- The Python executable being used in the notebook can be determined using

if the path for the twos differ , thats the reason why pip install,Conda install gives error

Fix for the Issue-- For pip, you can specify the Python executable explicitly:in the anaconda promp by changing the directory [cd] and can fix
like-$ /Users/neerajsoni/anaconda/bin/python -m pip install numpy

alternatively, to automatically use the correct executable (again using notebook shell syntax)
!{sys.executable} -m pip install numpy.


Remember: you need your installation command to match the current python kernel if you want installed packages to be available in the notebook.



Source:-https://jakevdp.github.io/blog/2017/12/05/installing-python-packages-from-jupyter/


