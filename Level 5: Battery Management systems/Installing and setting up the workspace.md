In this section of the Level we will be working with a Battery management system,

We will be using the BMS to get voltage data, current data, power data, temperature data from the cells and use it to plot and analyze how cells behave over a period of time. 

We will also be using it to control the charging and discharging of the cells.

In order to do the analysis and data collection, we will be using the `Python Programming language` as well as the `Arduino Environment` that uses `C++`.

Don't worry, you don't need to know much about these languages to perform these experiments.

Let's install Python and its libraries for now.

### Installing Python 3

Since windows don’t come with Python preinstalled, it needs to be installed explicitly. Here we will define step by step tutorial on How to install Python on Windows. Follow the steps below :

#### Step 1 : Click this link to download Python 3 : [Download Python 3](https://www.python.org/ftp/python/3.11.1/python-3.11.1-amd64.exe)

#### Step 2 : Select the Checkmark that says **"Add Python 3 to PATH"**

https://do7js0tdxrds1.cloudfront.net/klghz1covd38ijd6d98xc4dztq7o?response-content-disposition=inline%3B+filename%3D%22selectingpathandinstallingpython.png%22%3B&response-content-type=image%2Fpng&Expires=1701168114&Signature=LwiPdJ1zd6kfoclGVH3xO1z8lRQrhFMbHE9EsznHsX1TNyGr9cMBzNgdIZy7cRc1qOCe8RMKh1hRz1HghYjIMOdTEJhSyXdPIAi1rNY5TuPmPAu7u7KOptjWyFlTXG-~9-n2P22x7QTTIbXLlR0-PMRdnX5fDdouaATrzTqfiFdGDYTiO-ppX6gw3uWlqbKwbXxUXUVCvlYTZOu1cSjejM4XJpiHspMvpYW7I7dkyrdkXairhB~4GV74PlzCtI2kSth~4lot0TA-FtW3kiN8xazJyulJUaD0cXkGr0uRToDlckPh5P7RfAuenfCpVrtmeIs5wDbwm0CAz-MEIh1ufw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

#### Step 4 : Click Install Now

Once the installation is complete, you will need to install a few python packages.

#### Installing Python Packages.

1. Go to your Desktop, and press  `Win + r`  on the keyboard. 
2. In the window that appears, Copy and paste this `Pip install pyserial`

https://do7js0tdxrds1.cloudfront.net/xk7j5irhypn8twk1kdffizbfq23s?response-content-disposition=inline%3B+filename%3D%22InkedPip3Install+PySerial.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701168114&Signature=kB4c1IckjPt-1LvNbOZs168dhW02~-r9sxErrzbXUw0F79Mzyq2sWkalYgpEGDAIT~qSvIozr6fMzBbQqNMqW3D6tCshvJdfArnAl9po25quj8wyeWj6mty~32pz7yb15MKuBgUR~qXIdzpYN93c5dbDErHSS6716vnuNaYzdQ87HmUbXwXBUwpes~IalltctgQhrxH53KWVObzJIlMA0Hc4qoHcu~gjW6-3BwSeKMdL1jht8KbwQ0KvC3zNNwWelr9QN4xTvv9L9hfEnNlHydXaZppE6tTct1bRJ-j4lOVgW6tIdX9NiD0P6BVJZT6DX01ksLGYApoIbdJ83fQJfQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Once done, download the project file below and `unzip` or `Extract` the file somewhere in your computer by right-clicking on the downloaded file and clicking `Extract here` 

### -=- [Download Project File](https://github.com/swapnilmankame1995/Pupilfirst_BMS/archive/refs/heads/main.zip)

https://vimeo.com/807895093

>[Important] After Extracting, you will need to change the name of the folder `Pupilfirst_BMS-Main` to `BMS_main`