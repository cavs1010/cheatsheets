# Conda Cheat Sheet 🤓

Conda is an open source package management system and environment management system. An environment manager in computing is like having different toolboxes for different projects. Each toolbox (or "environment") has the exact tools you need for a specific project, so there's no mix-up or interference. This way, you can switch easily between projects without worrying about having the wrong tools in hand. It keeps everything organized and runs smoothly.


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
