# Cryptoasset Analytics: Data, Fundamental Concepts, and Open Source Tools

This repository contains notebooks and material for the tutorial on cryptoasset analytics, presented at The Web Conf 2022.

Additional information on the [tutorial website](https://cryptoassetanalytics.net)

# Program

Here be a summary, possible bullet points.

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