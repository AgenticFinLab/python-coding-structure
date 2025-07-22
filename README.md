# python-coding-structure


This repo provides a template for Python projects, including a setup script, configuration files, and a basic directory structure. It is designed to help developers quickly set up a new Python project with best practices in mind. With this template, your project named `cdemo` will be used as an internal package in python coding. By doing so, any module you created under the `cdemo/` can be imported directly after a `pip install -e .` command.


After creating a new Python project using this template, you still need to make the following changes:

1. Change the `cdemo` directory name to your project name.
2. Update the `description.txt` to describe your project.
3. Change the `setup.py` file by updating the version in `get_version` function and `name`, `description`, `url`, `keywords` fields of the `setuptools.setup`, where the `url` is the link address of the current repo.
4. Update the `README.md` file to provide a description of your project.   
5. Remove the `examples/Test/test.py` file if you don't need it. Then, create your own method based on your code under `cdemo/` directory.

Note that the `examples/` is a folder to allow you to place any method implemented based on the `cdemo`.


**Potential bugs**

If the program encounters bugs during installing site-packages, please try updating the setuptools first:
```python
 pip install -- upgrade setuptools
```


### Structure

```text
.
├── README.md               # Overview and structure of the project.
├── documents/
│   ├── files               # Various documentations related to the research.
│   ├── Progress-record.md  # Record of progress and findings.
├── examples/               # Exact demos and methods implemented based on the code from `cdemo/`.
├── cdemo/
│   ├── ???
└── requirements.txt        # List of dependencies required to run the project.
```


### Additional Packages

One may need to use additional packages to control the configuration and logging of the project. Please refer to the [project-init](https://github.com/AgenticFinLab/project-init) for details.


