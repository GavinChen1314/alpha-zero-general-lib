# Alpha Zero General - as a library

[![Build Status](https://travis-ci.org/peldszus/alpha-zero-general-lib.svg?branch=master)](https://travis-ci.org/peldszus/alpha-zero-general-lib)
[![codecov](https://codecov.io/gh/peldszus/alpha-zero-general-lib/branch/master/graph/badge.svg)](https://codecov.io/gh/peldszus/alpha-zero-general-lib)
[![GitHub](https://img.shields.io/github/license/peldszus/alpha-zero-general-lib)](LICENSE)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)

This is a fork of https://github.com/suragnair/alpha-zero-general turned into a library.

The idea is to have a small and clean library version of the code, with minimal requirements, without many implementations of specific games or large model files.


## Information

A simplified, highly flexible, commented and (hopefully) easy to understand implementation of self-play based reinforcement learning based on the AlphaGo Zero paper (Silver et al). It is designed to be easy to adopt for any two-player turn-based adversarial game and any deep learning framework of your choice. A sample implementation has been provided for the game of Othello in TensorFlow/Keras, see `example/othello/`.

To use this library for a game of your choice, subclass from `alpha_zero_general.Game` and `alpha_zero_general.NeuralNet` and implement their functions.

`alpha_zero_general.Coach` contains the core training loop and ```alpha_zero_general.MCTS``` performs the Monte Carlo Tree Search.

## TODO list

* [x] Poetry based build that works as library
* [x] Use `tqdm` for progress bars
* [x] Pythonic renaming of modules
* [x] Pythonic renaming of method names
* [x] Pythonic renaming of variables names
* [x] Black formatting, flake8
* [x] Fix inline comments
* [x] Make sure it works
* [x] AlphaZeroPlayer out of pit code
* [x] BareModelPlayer
* [x] HumanPlayer: named action mapping
* [x] Fix all flake8 issues
* [x] Add some tests
* [x] Use travis-ci.org tests
* [x] Coverage report on codecov.org
* [x] Use Ray to parallelize self-play
* [x] Proper abstract classes for Game and NeuralNet
* [ ] Make MCTS and model parameters explicit
* [ ] More documentation
* [ ] Provide one entrypoint for training and pitting
* [ ] Tournaments and ELO scores
* [ ] A first pypi release


## Contributors and Credits
* The original version was written by [Surag Nair](https://github.com/suragnair).
* [Shantanu Thakoor](https://github.com/ShantanuThakoor) and [Megha Jhunjhunwala](https://github.com/jjw-megha) helped with core design and implementation.
