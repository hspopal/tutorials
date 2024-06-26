# Univariate Analyses in Nilearn Workshop
04/24/2024

__**Content creator:**__ Haroon Popal \
**Note**: Code heavily borrowed from [Nilearn's own tutorials](https://nilearn.github.io/dev/auto_examples/04_glm_first_level/index.html). 

## Description
This workshop serves as a beginner's guide for using Nilearn to analyze neuroimaging data. It covers first and second level analyses, with code that can be easily adopted for your own analyses.


## Prerequisites
This workshop assumes that users:
1. are comfortable coding in python OR
2. have a good understanding of fMRI analyses, with experience using other software (e.g. AFNI, FSL, SPM)
   
## Set Up (do before the workshop)
Completing the workshop can be done completely in a Google Colab notebook. If users want to use their own data for the workshop then the following needs to be done before the workshop:

1. Install a python distribution on your personal computer (I recommend [anaconda](https://www.anaconda.com/download/))
2. Install the [Nilearn package](https://nilearn.github.io/dev/quickstart.html#quickstart) and it's relevant prerequisite packages:

   a. If you have anaconda, you can run the following in the command line: `conda install conda-forge::nilearn`
   
   b. Or, if you wish to create a separate anaconda environment:
   
      `conda create -n nilearn python=3.9`
   
      `conda activate nilearn`
   
4. Download the [workshop materials](https://github.com/hspopal/tutorials/archive/refs/heads/main.zip)
    
## Workshop objectives:
1. Understand how the Nilearn package handles neuroimaging data, and the similaries to existing python structures
2. Complete first level analyses to create contrast maps
3. Complete second level analyses to create group level contrast maps

## Workshop materials:
[![Google Colab Workshop Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hspopal/tutorials/blob/main/neuroimaging/univariate_analyses/univariate_analyses.ipynb)

### Example Scripts
- social_reward_1st_level-nilearn-indiv_runs.py
   - This is the actual script I use to do first level analyses
   - It can be run via the command line and takes a participant ID number as an input
   - The script can be modified, just as we went through in the workshop, to pull conditions of interests from your specific task
   - It creates beta maps for each condition, for each run, as well as for all runs averaged together
- [social_reward_2nd_level-nilearn.ipynb](https://hspopal.github.io/tutorials/neuroimaging/univariate_analyses/social_reward_2nd_level-nilearn.html)
   - This notebook is very similar to the second level analysis section of the workshop

## What We Won't Cover:
The flaws of other neuroimaging software (I won't go there). 

## Outline
| Section | Description | Time |
| --- | --- | --- |
| Intro | Motivation for using Nilearn | 10 minutes |
| Setup | Get data downloaded and ready to go | 5 minutes |
| Section 1 | First level analyses | 20 minutes |
| Section 2 | Second level analyses| 10 minutes |
| Conclusion |  Q & A | 10 minutes |
