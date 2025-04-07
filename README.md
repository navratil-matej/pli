# PLI course assignments

The assignments are prepared in the form of Python 3.x jupyter notebooks.

## Installation

The easiest way to get everything up and running on your own Windows 11 or Linux machine is:

1. Installation: [64-bit 3.9 version of Miniconda distribution](https://docs.conda.io/en/latest/miniconda.html)
	- When installing, do not choose to add Anaconda executable scripts to the standard paths. After installation, run the Anaconda Prompt and enter the conda init command so that it can be used from the regular command line (cmd.exe). Otherwise, you will always need to run Anaconda Prompt, which already contains all the necessary paths, in order to work.
	- Do not install in a directory containing accented words in the path.
2. Create the environment for the PLI object in a regular command line: conda create -n pli python=3.9
3. Activate the created environment: conda activate pli
4. Installing the modules:
   - as conda packages using the `pip install <package>` command,
   - pip install torch
   - pip install notebook   
   - pip install numpy   
5. Run jupyter notebook in the command line: jupyter notebook (in case of problems: python -n notebook)

## Credit conditions

- In order to receive credit, you must independently complete and submit all assignments or parts of assignments that are not marked as bonus assignments by the due date.
- *Failure to submit an assignment by the due date, as well as an assignment that is copied in whole or in substantial part, will result in loss of credit.

## Individual exercises

### 1. Introduction and regular expressions
- **deadline: 18.2.2024 7:59**

### 2. Finding the best-associated word pairs using pointwise mutual information
- **deadline: 18.3.2024 7:59**

### 3. Computing unigram and bigram models
- Don't repeat your own code: create functions in your notebook that call multiple times for each input corpus or sentence
- **deadline: 18.3.2023 7:59**

### 4. Smoothing the bigram model using the Witten-Bell method
- **deadline: 25.3.2023 7:59**

### 5. Working with the Word2Vec model
- **deadline: 8.4.2023 7:59**

## Final assignment
- The final assignment is in the file final_assignment_PLI_blank.ipynb
- It corresponds to the task of automatic capitalization (increasing initial letters of words) in text written in lowercase.
- The pre-trained ELECTRA model is used as the default language model.
- The task is suitable to be solved on Metacenter using a GPU and OnDemand Jupyter laptop
-- When using OnDemand Jupyter, it is always advisable to request a minimum of 25 hours (gets higher priority).
- You can use the metacentrum_install.sh script to start up the environment within Metacenter, which will automatically perform the necessary installations and configurations for you. Copy the script to your metacenter folder, and run it there after logging into metacenter.
-- Inside the script, it is important to set only the kernel name and environment (pli by default).
- You can get 3 plus points for the exam (the maximum is 25 points) for doing the bonus part of the final assignment (extending the punctuation feature).
-- The last layer of the model, the data preparation, as well as the subsequent punctuation generation function must be modified.
- **deadline: 10. week