# PDPilot User Study

This repository contains the material for the user study on [PDPilot](https://github.com/DanielKerrigan/PDPilot).

## Installation

To run the code for the study, you'll need Python 3.8 - 3.10, xgboost 1.7.4, Jupyter lab or notebook, and pdpilot 0.4.5. If you are running on an M1 Mac, then there are additional requirements of pyzmq<25 and jupyter_client<8 due to this [bug](https://github.com/jupyter/notebook/issues/6721). These dependencies are all specified in `requirements.txt`. Below are examples of setting up an environment using [conda](https://docs.conda.io/en/latest/miniconda.html) and [venv](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment).


conda:

```bash
git clone https://github.com/DanielKerrigan/PDPilotUserStudy.git
cd PDPilotUserStudy
conda env create -f environment.yml
conda activate pdpilot-study
jupyter lab
```

venv:

```bash
git clone https://github.com/DanielKerrigan/PDPilotUserStudy.git
cd PDPilotUserStudy
python -m venv pdpilot-study
source pdpilot-study/bin/activate
python -m pip install -r requirements.txt
jupyter lab
```

Additionally, download this [JSON file](https://drive.google.com/file/d/1tV77SUk9BKS9HpLOeok73eFLRmHVvuka/view?usp=share_link) containing pre-computed PDP and ICE plots and place it in the `ames` folder.
