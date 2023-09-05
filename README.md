# Codeforces Problem Selector

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)

## **Table of Contents**
- **[Overview](#overview)**
- **[Features](#features)**
- **[Getting Started](#getting-started)**
  - **[Prerequisites](#prerequisites)**
  - **[Installation](#installation)**
  - **[Usage](#usage)**
- **[Configuration](#configuration)**
- **[Contributing](#contributing)**


## **Overview** <a name="overview"></a>
This Python script is designed to assist competitive programmers in selecting Codeforces problems based on specified criteria. It allows you to filter problems by rating, tags, and ensures that the selected problems have not been solved by specific Codeforces handles. Additionally, you can print the problem links to the terminal and open them directly in your web browser (if you want).


## Features <a name="features"></a>

- **Problem Filtering:** You can filter problems based on minimum and maximum ratings, ensuring that they match your skill level.
- **Tag Filtering:** Select problems that belong to specific tags, helping you focus on areas of interest.
- **Exclusion of Solved Problems:** Avoid problems that have been previously solved by specific Codeforces handles.
- **Customizable Output:** The problem links are printed to the terminal. Additionally, you can choose to open them directly in your web browser.

## Getting Started <a name="getting-started"></a>

### Prerequisites <a name="prerequisites"></a> 

Before you begin, ensure you have met the following requirements:

- Python 3.x installed on your system.
- Python libraries: `requests`, `random`, `webbrowser`, `argparse`.

### Installation <a name="installation"></a>

1. Clone this repository or download the Python script:

 ```
 git clone https://github.com/Mohab96/cf-problem-selector.git
 cd cf-problem-selector
 ```
2. Install the required Python libraries:

```
pip install requests
pip install random
pip install webbrowser
pip install argparse
```

### Usage <a name="usage"></a>
To use the script, follow these steps:
- Open a terminal and navigate to the directory containing the script.
- Run the script with the desired options:

```
python main.py -o y -c 5 -mn 1500 -mx 2000
```
- `-o` (or `--open`): Set to y if you want to open the problems directly in your browser; otherwise, set to n.
- `-c` (or `--count`): Specify the number of problems you want to retrieve.
- `-mn` (or `--minRate`): Set the minimum rating for the problems.
- `-mx` (or `--maxRate`): Set the maximum rating for the problems.

### Configuration <a name="configuration"></a>
The script provides options for configuring your problem selection criteria:

- ```not_solved_by```: Add Codeforces handles to this list to exclude problems solved by specific users.
  - e.g. ```not_solved_by = ['Mohab_Yaser']```
- ```desired_tags```: Define the tags you want to see in the selected problems (and only those tags).
  - e.g. ```desired_tags = ['binary search', 'bitmasks', 'brute force', ...]```

## Contributing <a name="contributing"></a>
We welcome contributions from the community. If you'd like to contribute to this project, please follow these guidelines:

- Fork the project on GitHub.
- Create a new branch for your feature or bug fix.
- Commit your changes with clear descriptions.
- Push your changes to your fork.
- Create a pull request to the main repository.
