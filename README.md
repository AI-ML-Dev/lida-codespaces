# GitHub Codespaces ♥️ Jupyter Notebooks ♥️ Lida


## About GitHub Codespaces

This project uses the [Github codespace-jupyter](https://github.com/github/codespaces-jupyter) template for exploring machine learning and data science projects using a GitHub Codespaces development environment. You can learn more about GitHub Codespaces [here](https://docs.github.com/en/codespaces/overview). The main configuration files to know here are:
 - `.devcontainer/devcontainer.json` - configures the Dev Container environment with support for Python 3, Jupyter Notebooks & relevant VS Code Extensions
 - `requirements.txt` - configure any Python packages that need to be installed in the dev environment post creation.

In addition, the template has 2 main directories for projects:
 - `data/` - to contain the relevant datasets (CSV or JSON) on which data science and machine learning projects may be based
 - `notebooks/` - contain the Jupyter notebooks for the project exercises.

## About Project Lida

[Project Lida](https://github.com/microsoft/lida) is an open-source project project from Microsoft for the _Automatic Generation of Visualizations and Infographics using Large Language Models_. From the project README:

> LIDA is a library for generating data visualizations and data-faithful infographics. LIDA is grammar agnostic (will work with any programming language and visualization libraries e.g. matplotlib, seaborn, altair, d3 etc) and works with multiple large language model providers (OpenAI, Azure OpenAI, PaLM, Cohere, Huggingface). 

The figure below provides a high-level look at the LIDA System Architecture. You can read the details and learn more about the project from these resources:
 - [Read the research paper](https://arxiv.org/abs/2303.02927)
 - [Explore the sample notebook](https://github.com/microsoft/lida/blob/main/notebooks/tutorial.ipynb)
 - [Visit the website](https://microsoft.github.io/lida/) - with documentation & videos.

![LIDA System Architecture](https://microsoft.github.io/lida/files/lidamodules.jpg)


## About _this_ Project

This repository is meant for exploring LIDA usage with real-world datasets and examples in a GitHub Codespaces powered environment. It can serve both as a template for hands-on guided workshops, or as a source for self-guided exploration (and extension to new projects) by community.

My initial goals are as follows:
 - Establish a GitHub Codespaces environment for active learning
 - Add a Tutorial site to support step-by-step walkthrough of projects
 - Add example projects with real-world data sets and LLMs to learn-by-example


Because the `devcontainer.json` references the [Microsoft Universal Development Container Image](https://mcr.microsoft.com/en-us/product/devcontainers/universal/about) we have access to the following languages and platforms by default: _Python, Node.js, JavaScript, TypeScript, C++, Java, C#, F#, .NET Core, PHP, Go, Ruby, Conda_

This will allow us to use static site generators like Astro for the website, for more efficient and extensible documentation. The site will be hosted under the `website/` folder in the project and associated with a GitHub Actions workflow that builds/deploys to the GitHub Pages endpoint when source is changed. **Details on setup and customization of the project will be documnented in that website once setup**