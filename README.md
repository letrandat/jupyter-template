# jupyter-template

A quick way to set up Jupyter locally.

## Introduction

This repository provides a simple and efficient way to set up a local environment to run Jupyter Notebook, especially for those with little or no experience with Python. By using a virtual environment, we can avoid conflicts with other Python projects on your machine, ensuring a clean and isolated setup.

## Prerequisites

- **Python 3**: Ensure you have Python 3 installed on your machine. You can download it from the [official Python website](https://www.python.org/downloads/).

## Setup

### 1. Create a Virtual Environment

To create a new virtual environment named `jupyter-env` and activate it, use the following commands:

```bash
python3 -m venv jupyter-env
source jupyter-env/bin/activate
```

*Note: You can change `jupyter-env` to any name you prefer, like `project-name`.*

### 2. Install Requirements

With the virtual environment activated (you'll notice your terminal prompt starts with `(jupyter-env)`), install the required packages using the `requirements.txt` file. This file contains all the necessary dependencies to run Jupyter Notebook locally.

To install the requirements, run:

```bash
pip install -r requirements.txt
```

*`requirements.txt`* is a file that lists all the packages needed for your project, along with their versions. Using this file ensures that everyone working on the project has the same setup.

### Optional: Vim Integration

For Vim users, this repository includes `jupyterlab-vim`, a package that brings Vim key bindings to JupyterLab. If you want to include this package, you can add it to your `requirements.txt`.

The official GitHub repository for `jupyterlab-vim` is [here](https://github.com/jupyterlab-contrib/jupyterlab-vim).

To include `jupyterlab-vim`, add the following line to your `requirements.txt`:

```
jupyterlab-vim
```

### 3. Optional: Upgrade `pip`

To ensure you have the latest version of `pip`, you can upgrade it using the following command:

```bash
pip install --upgrade pip
```

*`pip`* is the package installer for Python. Upgrading it ensures you have the latest features and bug fixes.

## Ignoring the Virtual Environment Directory

To prevent the virtual environment directory from being tracked by Git, add it to your `.gitignore` file. This will keep your repository clean and avoid unnecessary files being pushed to version control.

Add the following line to your `.gitignore` file:

```
jupyter-env/
```

*Note: If you named your virtual environment differently, replace `jupyter-env` with the appropriate directory name.*

## Running Jupyter Notebook

Once the setup is complete, you can start Jupyter Notebook by running:

```bash
jupyter notebook
```

This will open the Jupyter Notebook interface in your default web browser, allowing you to create and run notebooks.
