# Monte Carlo Simulations for a Kanban/Agile Flow

<br><br>

## WHY - Facts over Opinions

Estimates are based on gut feeling, which means they're subjective and circumstancial. Being intangible and hard to quantify, they're not very realiable indicators to share. 

On the other hand, data can be measured, collected, reported, and analyzed — even visualized. It can enable data-driven discussions and enrich decision making through forecasts.

Benefits of forecasting with a [Monte Carlo Simulation](https://simple.wikipedia.org/wiki/Monte_Carlo_algorithm) instead of estimating (in Story Points): 
- Save the team member's time in estimating,
- More realistic planning: data collected from the past includes everything (vacations, sick days, outliers, ...)
- The forecast can be discussed and enrich decision making by chosing the risk the team/management wants to take.

Further thoughts on Agile metrics and #NoEstimates (with a focus on how to collect data and use it with a sense of responsibility): [You must be this tall to use agile metrics](https://medium.com/@jabopiti/you-must-be-this-tall-to-use-agile-metrics-9d2e3b4d4e20)

<br><br>

## Instructions to prepare the dataset exported from Jira

Depending on the system you have your data stored (Jira, or other), you should be able to export the data.

<br><br>
The format of the CSV will show:

- Criteria:
    - Project: 
        - Name of the Project in Jira
    - Issue types: 
        - Epic
        - Story
        - Task
        - Sub-task
        - Bug
    - Issue resolution Date: 2018-07-13

For the purpose of the simulation only the *Bug*, *Story* and *Task* will be considered.


<br><br>

## How to run the code in this repo

### If you already have VSCode installed + Python

Then go to the *Extensions* pane on the left menu and search for Jupyter and install the following ones (Provider = **Microsoft**):
- Jupyter
- Jupyter Cell Tags
- Jupyter Keymap
- Jupyter Notebook Renderers

After the installation, you can open the [MCS_When notebook](Generator/MCS_When.ipynb)

### If you don't have VSCode installed

In order to use the tool and generate the results, you'll need to:
1. Install an IDE. I recommend VSCode: download [here](https://code.visualstudio.com/download)
2. Then open the terminal and install:
- [Python](https://realpython.com/installing-python/)
- [Jupyter Notebooks](https://towardsdatascience.com/installing-jupyter-notebook-support-in-visual-studio-code-91887d644c5d)
- [pandas](https://pandas.pydata.org/docs/getting_started/install.html) 
- [matplotlib](https://matplotlib.org/stable/users/installing/index.html)
- [seaborn](https://seaborn.pydata.org/installing.html)
3. Then go to the *Extensions* pane on the left menu and search for Jupyter and install the following ones (Provider = **Microsoft**):
- Jupyter
- Jupyter Cell Tags
- Jupyter Keymap
- Jupyter Notebook Renderers 

<br><br>

# Major changes since the Fork

1. Fixed the *Distribution of Monte Carlo Simulation 'When'* chart to properly pass the correct param in the simulation method
2. Fixed the *Probabilities of Completion Dates* chart to properly calculate the percentiles from the distribution dataframe as process after the sampling from the MCS


<br><br>

If you like these topics and want to discuss project management stuff, consider visiting my page [here](https://bmhash.github.io/)
