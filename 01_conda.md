# Conda Cheat Sheet 🤓

Conda is an open source package management system and environment management system.

## 💿 Installation

Conda can be downloaded and installed via [Anaconda](https://www.anaconda.com/download).

## 🎮 Basic Commands

- **Update Conda**
  ~~~
  conda update conda
  ~~~
- **Check Version**
  ~~~
  conda --version
  ~~~

## 🌏 Environment Management

- **Create a new environment** 🆕 *The name of the environment in this case is 'myenv'*
  ~~~
  conda create --name myenv
  ~~~
- **Create a new environment with a specific Python version** 🐍
  ~~~
  conda create -n myenv python=3.6
  ~~~
- **Activate an environment** ▶️
  ~~~
  conda activate myenv
  ~~~
- **Deactivate an environment** ⏹️
  ~~~
  conda deactivate
  ~~~
- **List all environments** 📝
  ~~~
  conda env list
  ~~~
- **Remove an environment** 🗑️
  ~~~
  conda env remove --name myenv
  ~~~
