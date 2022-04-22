# Cryptoasset Analytics: Data, Fundamental Concepts, and Open Source Tools

This repository contains notebooks and material for the tutorial on cryptoasset analytics, presented at The Web Conf 2022.

Additional information on the [tutorial website](https://cryptoassetanalytics.net)

# Program

This tutorial consists of two subsequent parts and several exercises, which are implemented as Jupyter notebooks:

**Analyzing UTXO-Model Ledgers**

** 01_Inspect_BTC_address.ipynb: This notebook demonstrates how-to inspect the statistical properties (e.g., balance, total_received) and the payment relations of a single Bitcoin address.

** 02_Sextortion_Study.ipynb: This notebook demonstrates how to investigate Bitcoin addresses that received funds from sextortion spam victims. The data for this demo is taken from our study [Spams meet Cryptocurrencies: Sextortion in the Bitcoin Ecosystem](https://arxiv.org/abs/1908.01051).

**Analyzing Account-Model Ledgers**

** 03_JSNORPC_web3py_experiments.ipynb: This notebook demonstrates how to access Ethereum data (blocks, transactions) through a JSON/RPC endpoint of a full node (raw and with web3py).

** 04_Extracting_token_transfers_and_airdrop_analysis.ipynb: This notebook shows how to extract token transfers from a JSON/RPC endpoint, parsing with web3py and performing a very basic analysis of entities participating multiple times in an airdrop, inspired from our study on [Address Clustering Heuristics for Ethereum](https://www.researchgate.net/profile/Friedhelm-Victor/publication/341078202_Address_Clustering_Heuristics_for_Ethereum/links/5eb2751492851cbf7fa94b12/Address-Clustering-Heuristics-for-Ethereum.pdf).

** 05_NFT_wash_trading.ipynb: This notebook shows how to extract NFT transfers and sales performed on OpenSea on the Ethereum blockchain. We visualize a small example that appears to be NFT wash trading.

** 06_Working_with_ethereum_etl_data.ipynb: This notebook shows how to work with multiple CSV files as extracted with `ethereum-etl`, extract token transfers and allow for analyses that exceed the available RAM.

# Slides and Recording

Slides are available:

1.  [Cryptoassets and Blockchain 101](https://tubcloud.tu-berlin.de/s/Pbb8pPeCZK52CBZ)
2. [Analyzing UTXO Ledgers](https://tubcloud.tu-berlin.de/s/jntdZCwWFdty9sH)
3. [Analyzing Account Ledgers](https://tubcloud.tu-berlin.de/s/Xsb24ybYRo2oQdZ)
4. [Outlook](https://tubcloud.tu-berlin.de/s/98T8rHFGki5JoCZ)

A recording will be available after the conference.

# Notebook preparation

The tutorial will make use of several notebooks, which are available in this repository.
You can run the notebooks locally, as follows:

Setup a Python environment with [Anaconda](https://www.anaconda.com/products/distribution):

    conda env create -f environment.yml
    conda activate caa-tutorial

For notebooks 1-2 you need to install the [GraphSense Python library](https://github.com/graphsense/graphsense-python).

    git clone git@github.com:graphsense/graphsense-python.git
    cd graphsense-python
    python setup.py install

Copy the config temp file and enter your GraphSense API key

    cp config.json.tmp config.json
    vi config.json

Run the jupyter notebooks

    jupyter notebook
