# Module 6 Project: datafun-06-eda
Project 6 demonstrates the creation of a custom exploratory data analysis (EDA) project using GitHb, Git, Jupyter, pandas, Seaborn, and other popular analytics tools.

## Introduction to Dataset: Car Crashes 
We will be working with the dataset 'car_crashes', which provides a glimpse into various factors surrounding these incidents, such as the number of crashes, the presence of alcohol-related crashes, and more. We will use this dataset to explore patterns, identify trends, and gain insights into the factors contributing to road accidents. Throughout this notebook, we'll use the power of data visualization techniques using Python's seaborn library to uncover hidden relationships and tell a compelling story behind the statistics.

You can find the dataset [here](https://github.com/mwaskom/seaborn-data/blob/master/car_crashes.csv).


|  Column Name   |                      Description                        |
|:--------------:|:-------------------------------------------------------:|
|     total      |  Total number of car crashes per billion miles         |
|    speeding    |  Number of car crashes where speeding was involved      |
|    alcohol     |  Number of car crashes where alcohol was involved       |
| not_distracted|  Number of car crashes where the driver was not distracted|
|  no_previous  |  Number of car crashes where the driver had no previous incidents|
|  ins_premium  |  Insurance premium for car owners ($)                    |
|  ins_losses   |  Losses incurred by insurance companies for collisions ($)|
|    abbrev      |  Abbreviation for the state where the crash occurred     |




## Project Setup and Layout
Project setup consists of beginning a git repository with a README.md, cloning the project down to the root project folder, adding necesssary files and depenency installs, and performing initial commits to Github. 

### Project Structure & Deliverables
- `README.md`: Provides an overview of the project and instructions for setting up the environment and running the notebook.
- `requirements.txt`: Lists all dependencies needed to run the notebook.
- `dgraves_eda.ipynb`: Jupyter notebook.

### Environment Setup 
- Create a new github repository 'yourname_eda.ipynb'.
- Include a README.md file.

#### Clone project down and open project folder in VS Code
```bash
git clone https://github.com/dgraves4/datafun-06-eda
cd "C:\Users\derek\OneDrive\Documents\44608 Data Analytics Fundamentals\Mod 6\datafun-06-eda"
code .
```

#### Create and activate virtual environment
```bash
python -m venv .venv
source .venv/scripts/activate #windows
```

#### Create and add .gitignore file to root project folder
- Create a .gitignore file in project directory "C:\Users\derek\OneDrive\Documents\44608 Data Analytics Fundamentals\Mod 6\datafun-06-eda\.gitignore"
- Add .vscode/ and .venv/ to .gitignore file.

#### Install dependencies and freeze to requirements.txt
Dependencies for this project:
- Jupyterlab 
- pandas 
- pyarrow
- matplotlib 
- seaborn

```bash
pip install jupyterlab pandas pyarrow matplotlib seaborn
pip freeze > requirements.txt
```
#### Initial and Subsequent Commits to Github for version control

```bash
git add .
git commit -m "Initial commit"
git push origin main
```
## Project Start
- Create the Notebook: In the VS Code Explorer, create a new file i.e., yourname_eda.ipynb. Ensure it has a .ipynb extension.
- Verify your new notebook is open for editing. If needed, view the project files in VS Code Explorer and double-click the notebook file to open it for editing.
- Add a Markdown cell at the top of your notebook with the introduction (include the title, author, date and the purpose of the project).

### Import Dependencies
- Install dependencies in .ipynb file at the top of the file and after markdown introduction.

```bash
import matplotlib.pyplot as plt
import pandas as pd
import seaborn as sns
```
## Exploratory Data Analysis
Perform exploratory data analysis using the tools and skills covered previously in module 4. 

### Step 1: Data Acquisition
Load the data into a pandas DataFrame for analysis. 

Project example: 
```bash
# Load the Iris dataset into DataFrame
df = sns.load_dataset('car_crashes')

# Inspect first rows of the DataFrame
print(df.head())
```

### Step 2: Initial Data Inspection
Display the first 10 rows of the DataFrame to inspect the data types we are working with. 

Project example:
```bash
```

### Step 3: Initial Descriptive Statistics
Use the DataFrame describe() method to display summary statistics for each column.

Project example:
```bash
```

### Step 4: Initial Data Distribution for Numerical Columns
Choose a numerical column and use df['column_name'].hist() to plot a histogram for that specific column. To show all the histograms for all numerical columns, use df.hist().

Project example:
```bash
```

Use a markdown cell to document any observations.

### Step 5: Initial Data Distribution for Categorical Columns
Choose a categorical column and use df['column_name'].value_counts() to display the count of each category. Use a loop to show the value counts for all categorical columns.

Project example:
```bash
```

Use a markdown cell document any observations.

### Step 6: Initial Data Transformation and Feature Engineering
Use pandas and our other tools to perform data transformations such as renaming columns, adding new columns, or transforming existing data.

Project example:
```bash
```

### Step 7: Initial Visualizations
Create a variety of chart types with seaborn and matplotlib and display them alongside markdown cells for story and context.  Three sections are created with the following subsets for each:
- Goal
- Chart Type
- Chart Display
- Story (using markdown cells)

### Step 8: Initial Storytelling and Presentation
The objective of this notebook is to acquaint the reader with the author and the chosen topic, leading them through an immersive visual narrative enriched with markdown cells. These markdown cells serve to offer both informative and captivating insights, enhancing the reader's understanding and engagement throughout this notebook.

### Conclusion
Provide and overarching summary for the findings, results, and any trends or followup analysis that could be performed based on this initial analysis using well-structured markdown cells. 

## Contributing
We welcome contributions to this project. If you have suggestions to improve the project or encounter issues, please open an issue or submit a pull request.

## References & Acknowledgments
Special thanks to OpenAI for assistance with troubleshooting and script debugging as well as schema design. 

Additional references used for this project include:

- [car_crashes dataset](https://github.com/mwaskom/seaborn-data/blob/master/car_crashes.csv)
- [Specification for Project 6 Module](https://github.com/denisecase/datafun-06-spec)
- [JUPYTER.md](https://github.com/denisecase/datafun-04-spec/JUPYTER.md)
- [MARKDOWN.md](https://github.com/denisecase/datafun-04-spec/MARKDOWN.md)
- [Linear Regression in Python using Jupyter Notebooks!](https://www.youtube.com/watch?v=hitCh7-ZItQ)
- [Plotting graph For IRIS Dataset Using Seaborn And Matplotlib](https://www.tutorialspoint.com/plotting-graph-for-iris-dataset-using-seaborn-and-matplotlib)
- [Seaborn Tutorial](https://seaborn.pydata.org/tutorial.html)