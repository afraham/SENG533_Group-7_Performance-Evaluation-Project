# SENG 533 Group 7 Performance Evaluation Project

## Overview 
This repository contains our course project for evaluating deep learning training performance across different execution environments and experiment settings.

The project benchmarks three neural network models on the SVHN dataset:
- `MLP`
- `RNN`
- `CNN`

The main comparison in this repo is between:
- `Google Colab` and `Kaggle`
- `CPU` and `GPU` execution
- `50%` and `100%` dataset usage
- different model architectures

## Project Goal

The goal of this project is to measure how platform choice, hardware type, model type, and dataset size affect training time for the same image classification task. The repository includes the benchmark notebooks, collected CSV results, and an analysis notebook that turns the raw results into report-ready visualizations.

## Experiment Setup

The current benchmark configuration in the repo uses:
- `SVHN` as the dataset
- `MLP`, `RNN`, and `CNN` as the tested models
- `5` training epochs
- batch size `64`
- dataset fractions of `0.5` and `1.0`
- both `cpu` and `gpu` device modes where available

Each benchmark notebook logs training metrics such as:
- total training time
- average per-epoch training time
- throughput
- training, validation, and test accuracy/loss