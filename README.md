# Installing Anaconda
Installing python with anaconda

## How to use Python using Anaconda version 3
Here I am going to help you how to install python 3.7 using anaconda3 on a "Linux" operating system. Before starting to install, click on the following link: [anaconda in linux](https://docs.anaconda.com/anaconda/install/linux/), this link will take you to the Anaconda page, where they provide you it also helps to install anaconda. In particular, I have always used that website and highly recommend it.

* Where do I find the executable to install Anaconda?

Click here: [Anaconda](https://www.anaconda.com/products/individual#linux)

Steps to follow in a terminal:
```
1. Open a terminal. Go to a folder where you want to download the executable (Ex: cd /home/name/Documents/). Being on that path, download the Anaconda executable by typing in the terminal:
  
   >> web https://repo.anaconda.com/archive/Anaconda3-2020.11-Linux-x86_64.sh
  
2. To install Anaconda for Python 3.7:
 
   >> bash Anaconda3-2020.11-Linux-x86_64.sh 

3. Scroll to the bottom of the license terms and enter “Yes” to agree.

4. The installer prompts you to click "Enter" to accept the default install location or specify an alternate installation directory. If you accept the default install location, the installer displays “PREFIX=/home/name/anaconda3” and continues the installation. It may take a few minutes to complete.

5. The installer prompts “Do you wish the installer to initialize Anaconda3 by running conda init?” We recommend “yes”.

6. The installer finishes and displays “Thank you for installing Anaconda3!”

7. At the end of the installation write in the terminal: source /home/noelia/.bashrc 

8. Run conda init, Write in the terminal: conda init

```
* Another recommendation is that you always create a project (environment) every time you want to work with certain data. This is so that the versions of different libraries do not create conflicts.

```
conda create --name py37 python=3.7 matplotlib basemap gdal 
conda activate py37
```
* Above I recommend installing the basemap and gdal libraries together because I have had problems installing the gdal library individually. 

* Finally, the platform that I usually use is the "spyder"

```
conda install -c anaconda spyder 
```

## Another way to install libraries in a specific environment

* It is very difficult to remember each installed library when we are working on a specific environment, therefore, there is another way to install these libraries all together. [evironment.yml](https://github.com/rnoeliab/Installing_anaconda/enviroment.yml). 

```
conda env create -f enviroment.yml -n pywrf 
```

# Thanks!!!!
