# Cryptoasset Analytics: Data, Fundamental Concepts, and Open Source Tools

This repository contains notebooks and material for the tutorial on cryptoasset analytics, presented at The Web Conf 2022.

Additional information on the [tutorial website](https://cryptoassetanalytics.net)

# Program

This tutorial consists of two subsequent parts and several exercises, which are implemented as Jupyter notebooks:

**Analyzing UTXO-Model Ledgers**

** 01_Inspect_BTC_address.ipynb: This notebook demonstrates how-to inspect the statistical properties (e.g., balance, total_received) and the payment relations of a single Bitcoin address.

** 02_Sextortion_Study.ipynb: This notebook demonstrates how to investigate Bitcoin addresses that received funds from sextortion spam victims. The data for this demo is taken from our study [Spams meet Cryptocurrencies: Sextortion in the Bitcoin Ecosystem](https://arxiv.org/abs/1908.01051).

**Analyzing Account-Model Ledgers**

TODO: Friedhelm


# Slides and Recording

Slides and a recording of the tutorial are available at ... 

# Notebooks

The tutorial will make use of several notebooks, which are available in this repository.
You can run the notebooks locally, as follows:

Setup a Python environment:

    conda env create -f environment.yml
    conda activate caa-tutorial

For notebooks 4-5 you need to install the [GraphSense Python library](https://github.com/graphsense/graphsense-python).

    git clone git@github.com:graphsense/graphsense-python.git
    cd graphsense-python
    python setup.py install
    
Copy the config temp file and enter your GraphSense API key

    cp config.json.tmp config.json
    vi config.json

Run the jupyter notebooks

    jupyter notebook