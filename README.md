# MultiLingual Speech Recognition in Snowflake using Snowpark Python, PyTorch, Streamlit and OpenAI

## Overview
In this guide, you will learn how to build audio sentiment recognition in Snowflake using Snowpark for Python,Streamlit, NRCLex and OpenAI – "an application system which can ease the customer satisfaction for various customer support businesses".

## Environment setup
Create new Conda environment
```
conda create --name spark_openai_py38 --override-channels -c https://repo.anaconda.com/pkgs/snowflake python=3.8 numpy pandas -y
```
Activate conda environment
```
conda activate spark_openai_py38
```
Install into Conda environment
```
conda install snowflake-snowpark-python
pip3 install streamlit watchdog openai nrclex
```
List all the python packages in our environment
```
conda list
```
## Update config.py
Static pandas data with a static chart.
Update Snowflake account connection details

Update OpenAI key obtained from https://platform.openai.com/account/api-keys
OPENAI_API_KEY = "sk-zisILbg3oT..."

## Setup snowflake objects
Run the contents of snowflake_objects.sql with the same credentials you put in config.py

## Run app
Static pandas data with a static chart.
```
streamlit run Snowpark_NRCLex_Streamlit_OpenAI_Audio_rec.py
```
