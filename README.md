# Data Mining Project

## Repository description

Private repository for the delivery of the Data Mining project.
It is structured as follows:

- **project.pdf**: pdf with the project specification;
- **report.pdf**: pdf with the report that explains and highlights the work done
- **dataset**: folder containing the initial datasets, all the intermediate datasets will also be saved here;
- **models**: folder (which is not initially present) where the models generated in task 4 will be saved;
- **5 Jupyter Notebook**: one for each task required.

### Requirements for code execution

Given the amount of packages to install with their dependencies, it is suggested to create a specific python environment, specifically a **python3.12** environment is recommended.

You can create it through the following command:

```bash
python3.12 -m venv DMenv
```

and you can access it with:

```bash
source DMenv/bin/activate
```

Once inside the environment to download the dependencies the command is as follows:

```bash
pip install -r requirements.txt
```

## Dependencies between notebooks

Since the transformed datasets need to be used, the *third_task* and *fourth_task* files need the *second_task* to be executed first. For the same reason regarding the models, the *fourth_task* needs to be executed before executing the *fifth_task*.

As also indicated in the notebook of the fourth task, to visualize the decision tree it is necessary to install GraphViz:

- MacOs: brew install graphviz

- Linux: sudo apt-get install graphviz

- Windows: Install from here https://graphviz.org/download/ and add the following enviroment variable (the path can change):
  
  ```python
  import os
  os.environ["PATH"] += os.pathsep + 'C:\Program Files (x86)\Graphviz2.38/bin/'
  ```