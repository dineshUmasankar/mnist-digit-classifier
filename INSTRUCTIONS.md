# Instructions for reproducability

## Manual Dependencies

All of the code is within the src/ folder as a IPython notebook.

Ensure the following dependencies are installed:

- Python >= 3.8
- Jupyter Notebook Kernel

The above dependencies will depend on your host system, and as such
I recommended following their respective setup instructions.

On Windows, Jupyter Notebook and its kernel is usually setup
by VSCode and the traditional Python installation, but this might be incorrect.

Feel free to open an issue, if you have issues with an error log.

## Dependency Installation

I have provided a setup.py file and requirements.txt to help everyone
reproduce the project, however, ensure that you create and activate a virtual
environment in order to avoid polluting your global namespace.

Figure out how to create / activate a venv at this [link](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#create-a-new-virtual-environment)

Once you have activated the venv, then run the following command to install all project dependencies:

```py
python3 -m pip install .
```

## Reproduce Results

Open up the IPython notebook and run all the cells to reproduce every step of the project from training to testing, and reproduce the figures that were utilized
as part of the report as well.

## Last Effort

If you are still having issues, then I highly recommend utilizing the Google CoLab in order to reproduce the same results.