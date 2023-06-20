# Machine Learning

## Introduction

Machine learning in unity takes a few steps to set up. There are instructions on how to set it up at tafe.


## Step 1: Command Prompt

We are going to have to use command prompt to get this to work. It might seem scary at first but its actually quite simple.

Firstly open up command prompt (Type CMD in the start menu to find it)

![Command Prompt](./Screenshots/CommandPrompt.png)

There are a few useful commands that we will need to know. To use the following commands, just type them in to your Command Prompt window.


* __dir__: <br/> (Directory) "dir" will display all files and folders within the directory you are currently in (in the screenshot it would be C:\Users\acapela). Think of a directory as the folder you are currently in.
* __cd [Directory name]__:<br/>  (Change Directory) "cd" will allow you to change the directory you are in, just type in cd and then type the directory you want to open. (e.g. "cd Documents")
* __del [Directory or File Name]__: <br /> (Delete) if you want to delete a folder or directory you can run this command (e.g. "del temp.txt")
* __py__ or __python__: <br /> (Python) Once we have python installed, we can use "py" or "python" to run python specific command. In our case we will be using "py -3.8".


## Step 2: Python
We are going to need to have python, at tafe we already have it installed but we need to make sure we are using the correct version.

Ensure you have python installed (and to work out which version you have) type in "py" into your Command Prompt window. It will also enter you in python mode

![python](./Screenshots/py.png)

To exit this mode, type in exit() or press Ctrl-Z plus Enter.

**We need to have python version 3.8 installed.**

1. If you do not have Python 3.8 install it from here. https://www.python.org/downloads/release/python-3810/ <br /> To install python at tafe, place the installer in c:\temp

![py website installer](./Screenshots/pyWin64Install.png)
![py install to path](./Screenshots/pyInstaller.png)

2.  To ensure you are using the correct verion of python, we are going to be using the command "py -3.8" instead of just "py"
> py -3.8 <br />
OR <br />
> python -3.8

3. Create a Unity Project (Basic 3D, Built-in Render pipeline)

4. Using "cd", go to your project (Same folder as your Assets, Packages and Project settings)
> cd c:\Temp\MachineLearning\

5. Create a virtual environment by typing in the following command
> py -3.8 -m venv venv

6. To activate that virtual environment type:
> venv\Scripts\activate

## Step 3: Virtual Environment

![MLAgents in Package Manager](./Screenshots/InVenv.png)

Now that we set up and are in our virtual environment, your Command Prompt should look like the above screenshot. If it doesn't, please look over [Step 2](#step-2:-python).
The following will be commands used within the virtual environment. Don't be scared of all the text that appears with each command. (If it looks like the commands has stopped progressing, type pressing enter)

![MLAgents in Package Manager](./Screenshots/InstallTorch.png)

1. Install/Upgrade pip
> pip install --upgrade pip

2. Install torch
> pip install torch -f https://download.pytorch.org/whl/torch_stable.html

3. Install MLAgents
> pip install mlagents

4. Test MlAgents <br /> Test to see if its all working nicely, you might need to do the next step if it gives you an error.
> mlagents-learn --help
![MLAgents working](./Screenshots/MlAgentsWorking.png)

5. Downgrade protobuf <br /> Only if you can an error that mentions downgrading protobuf do the following command, then do step 4 again.
> pip install protobuf==3.20.*



## Step 4: Unity

Lets finally head into unity.

1. Install the MLAgents package from the Package Manager.

![MLAgents in Package Manager](./Screenshots/MLAgentsPackage.png)

2. 
