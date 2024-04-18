# s2p_demo
Suite2p demonstration for the <a href="https://can-acn.org/meeting-2024/satellite-events/hands-on-neural-behavioural-and-histological-data-analysis-workshop-can2024-satellite/">Hands-on, Neural, Behavioural and Histological Data Analysis Workshop</a> by the UBC Dynamic Brain Circuit Cluster as a part of CAN 2024 meeting.

# Prerequisites
Ensure you either <a href="https://www.anaconda.com/download">install Anaconda</a> or <a href="https://docs.anaconda.com/free/miniconda/miniconda-install/">install miniconda</a> on your computer.

You can verify that you have Anaconda if you have Anaconda Navigator in your applications. You can also verify by running the command ```conda --version``` in the Terminal (Mac/Linux) or the Anaconda Prompt application (Windows).

# Environment Setup
1. Click the green "Code" button at the top of the page and select "Download Zip". This will download "s2p_demo-main.zip" onto your computer. Unzip this file, and (if you'd like), move it to your desired directory on your local computer.

2. Open Terminal/Anaconda Prompt and navigate to your unzipped "s2p_demo-main" folder.

>NOTE: use the commands ls to see subdirectories and cd <subdirectory> to navigate through your files. You can use cd .. to go to the parent directory.

3. In your Terminal/Anaconda Prompt, enter the following command:
 ```
 conda env create -f suite2p.yml
 ```

# Activate the Environment

Activate environment with ```conda activate suite2p```.

To activate Jupyter Notebooks, you can either:

Open the Anaconda Navigator application and press "Launch" on Jupyter Notebook.
Open Terminal/Anaconda Prompt and run this command in the deeplabcut environment:
```
jupyter notebook
```
This will open up the Jupyter Notebook Home Page in your default browser. You will need to navigate to where "s2p_demo-main" is located on your computer. In this folder, open "s2p_tutorial.ipynb" to start.

Then, you need to run the Jupyter Notebook using the suite2p environment we just created. You can modify this by going 
<br><b>Kernel > Change Kernel > Python [conda env:suite2p].</b>

