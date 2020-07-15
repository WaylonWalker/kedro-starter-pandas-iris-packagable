# Kedro Starter: pandas with example

## Introduction

This repository contains a Kedro project template with some initial configurations and an example pipeline to demonstrate best practices when using Kedro. It originates from our [Hello World](https://kedro.readthedocs.io/en/0.16.2/02_getting_started/04_hello_world.html) example.


### An example maching learning pipeline using only native `Kedro`

![](./images/iris_pipeline.png)

This starter contains the code for an example machine learning pipeline that trains a random forrest classifier to classify iris based on the popular iris dataset. The pipeline includes two modular pipelines: a data engineering one and a data science one.

The data engineering pipeline includes:
* A node to split the transformed data into training dataset and testing dataset using a configurable ration

The data science pipeline includes:
* A node to train a simple multi-class logistic regression model
* A node to make predictions using this pre-trained model on the testing dataset
* A node to report the accuracy of the predictions performed by the model
