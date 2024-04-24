# s2p_demo
Suite2p demonstration for the <a href="https://can-acn.org/meeting-2024/satellite-events/hands-on-neural-behavioural-and-histological-data-analysis-workshop-can2024-satellite/">Hands-on, Neural, Behavioural and Histological Data Analysis Workshop</a> by the UBC Dynamic Brain Circuit Cluster as a part of CAN 2024 meeting.

<img src=tutorial_images\NINC_DBC_DMCBH_logos.jpg>

These tutorial notebooks were developed at the Djavad Mowafaghian Centre for Brain Health by the NINC/UBC Brain Circuits team.  If you find the tutorials useful you can acknowledge us with the following statement: 

<em>"This work was supported by resources made available through the Dynamic Brain Circuits cluster and the NeuroImaging and NeuroComputation Core at the UBC Djavad Mowafaghian Centre for Brain Health (RRID:SCR_019086)."</em>

If you use the packages in your research, please cite the originators as per their documentation.

# Initial Setup
Here is what the final "s2p_demo" folder will look like at the end of the demo:
```
.
└── s2p_demo/
    ├── suite2p.yml ### configuration file for suite2p environment
    ├── s2p_tutorial.ipynb ### tutorial notebook for this demo
    ├── README.md
    └── my_files/
        └── test_run/
            ├── data/ ### folder for storing sample data
            │   └── sample_data.tiff ###
            └── suite2p ### this folder is created when you run suite2p, and is where results of the run are stored.
```
1. Download all the files in this Github repository as a zip file. 
- <b>Click</b> the green "Code" button at the top of the page and select "Download Zip". This will download "s2p_demo-main.zip" onto your computer. Unzip this file.
2. (optional) <b>Move</b> this unzipped file into a convenient location in your file explorer

# Prerequisites
Ensure you either <a href="https://www.anaconda.com/download">install Anaconda</a> or <a href="https://docs.anaconda.com/free/miniconda/miniconda-install/">install miniconda</a> on your computer.

You can verify that you have Anaconda if you have Anaconda Navigator in your applications. You can also verify by running the command ```conda --version``` in the Terminal (Mac/Linux) or the Anaconda Prompt application (Windows).

>NOTE: We have found in tests prior to this demo workshop that performance of Suite2p on Intel Macs was slightly less reliable in comparison to other CPUs. If you encounter issues running Suite2p on your computer, please find a partner to work with for this demo.

# Environment Setup
1. Open Terminal/Anaconda Prompt and navigate to your unzipped "s2p_demo-main" folder.

>NOTE: use the commands ls to see subdirectories and cd <subdirectory> to navigate through your files. You can use cd .. to go to the parent directory.

2. In your Terminal/Anaconda Prompt, enter the following command:
 ```
 conda env create -f suite2p.yml
 ```

# Downloading Data
All of the data used for this tutorial can be found <a href="https://osf.io/ztcnm/?view_only=59d6948657a742f688b4cac9ad1f54e9">here</a>.

1. <em>Sample .tiff file</em>
<br>For this workshop, you will be downloading a sample .tiff file to try implmenting several suite2p functions upon. 
* <b>Click</b> 2P_M210914_TEX_20114_FB.tiff and select "Download" to download it (500 MB).
* <b>Move</b> the .tiff file into "s2p_demo" > "my_files" > "test_run" > "data"

2. <em>Sample Data for Analysis</em><br>
Sample data will be used to try different analysis processes available on Suite2p.
* <b>Click</b> M210914_DYN_20114_FB.zip and select "Download" to download it (216 MB).
* <b>Unzip</b> the  zip file and <b>move</b> the folder into "s2p_demo" > "my_files" > "test_analysis" > "data".

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

