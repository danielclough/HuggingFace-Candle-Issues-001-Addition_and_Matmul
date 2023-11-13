# Repros for Pytorch to HuggingFace/**Candle** Issues

## Issue 1 - Addition and Matmul


1. I wish to know if there is a simple way to multiply a tensor by a scalar.
1. Should it be possible to multiply 1D tensors with `huggingface/candle`?

## Install Evcxr Jupyter Kernel

This project uses Evcxr Jupyter Kernel in order to use Rust code in `rust.ipynb` file.

I am using Jupyter Notebooks in order to simplify the comparison as much as possible, but I can adjust this practice if it is dispreferred by others.

If the below does not work refer to the [install instructions on Github](https://github.com/evcxr/evcxr/tree/main/evcxr_jupyter).

```sh
# Assumes Debian/Ubuntu with Rust and Python installed
sudo apt install jupyter-notebook libfontconfig1-dev -y
cargo install --locked evcxr_jupyter
evcxr_jupyter --install
pip install --upgrade notebook
jupyter notebook
```