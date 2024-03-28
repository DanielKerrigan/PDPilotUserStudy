# PDPilot User Study

This repository contains the material for the user study on [PDPilot](https://github.com/DanielKerrigan/PDPilot).

## Contents

- [introduction-and-interview-slides.pdf](https://github.com/DanielKerrigan/PDPilotUserStudy/blob/main/introduction-and-interview-slides.pdf): Slides to introduce the study and review PDP and ICE plots and slides for the semi-structured interview.
- [protocol.pdf](https://github.com/DanielKerrigan/PDPilotUserStudy/blob/main/protocol.pdf): A document that outlines the protocol of the study. In particular, it includes the script for the tutorial of how to use PDPilot, the questions that were asked to participants during training, and the prompt for the model analysis.
- [ames](https://github.com/DanielKerrigan/PDPilotUserStudy/tree/main/ames): The Ames, Iowa housing dataset, trained model, and notebooks for preprocessing the dataset, training the model, calculating the plots, and running PDPilot. This dataset is for the main model analysis that the participant performs.
- [bike-rental](https://github.com/DanielKerrigan/PDPilotUserStudy/tree/main/bike-rental): The Bike Sharing dataset and notebook for training the model and running PDPilot. This dataset is used during training.
- [churn](https://github.com/DanielKerrigan/PDPilotUserStudy/tree/main/churn): The Churn dataset and notebook for training the model and running PDPilot. This dataset is used during the tutorial.

## Installation

To run the code for the study, you'll need Python 3.8 - 3.11, XGBoost, Jupyter lab or notebook, and pdpilot. Below are examples of setting up an environment using [conda](https://docs.conda.io/en/latest/miniconda.html) and [venv](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment).


conda:

```bash
git clone https://github.com/DanielKerrigan/PDPilotUserStudy.git
cd PDPilotUserStudy
conda env create -f environment.yml
conda activate pdpilot-study
jupyter-notebook
```

venv:

```bash
git clone https://github.com/DanielKerrigan/PDPilotUserStudy.git
cd PDPilotUserStudy
python -m venv pdpilot-study
source pdpilot-study/bin/activate
python -m pip install -r requirements.txt
jupyter-notebook
```

Additionally, download this [JSON file](https://drive.google.com/file/d/1tV77SUk9BKS9HpLOeok73eFLRmHVvuka/view?usp=sharing) containing pre-computed PDP and ICE plots and place it in the `ames` folder.
