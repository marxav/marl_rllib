# marl_rllib

## Requirements

* System
  * Ubuntu 18.04
  * Python 3.8.3
  * pip-20.2.2 (cf pip install --upgrade pip)

* Download files on your machine
  * git clone https://github.com/marxav/marl_rllib.git
  
* Go to the marl_rllib main directory
  * cd marl_rllib

* Create a virtual environment
  * python3 -m venv marl_rllib

* Activate virtual environment
  * source marl_rllib/bin/activate

* Load the python librairies needed for GIPFA (e.g. numpy, pandas, torch...) from the requirements file
  * python3 -m pip install -r requirements.txt

## Use Tensorboard for displaying metrics

* Launch Tensorboard app with a shell command line
  * $ tensorboard --logdir=~/ray-results

* Go to Tensorboard home page
  * http://localhost:6006/

## Edit and Run the notebook
* Open the Jupyter [rllib_marl.ipynb ](rllib_marl.ipynb ) notebook in a browser

* You may change some configuration values like:
  * *self.num_agents = 5* instead of *self.num_agents = 4*
  * *'run_or_experiment': 'PG'*  instead of *'run_or_experiment': 'PPO'* 
  
* Run the whole notebook

* Look at resulting metrics in Tensorboard
  * Refresh each of the three pages (SCALARS, DISTRIBUTIONS, HISTOGRAMS)
  * You should see a screen like in the following image 
    ![](marl_rllib_tensorboard.png?raw=true)
