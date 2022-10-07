<p align="center">
    <img src="jumpy-text.png" width="500px"/>
</p>

JumPy is a common backend for [JAX](https://github.com/google/jax) or
[NumPy](https://numpy.org/):

* A JumPy function returns a JAX outputs if given a JAX inputs
* A JumPy function returns a JAX outputs if jitted
* Otherwise a jumpy function returns NumPy outputs

JumPy lets you write framework agnostic code that is easy to debug by running
as raw NumPy, but is just as performant as JAX when jitted.

We maintain this repository primarily so to enable writing Gymnasium and PettingZoo wrappers that can be applied to both standard NumPy or hardware accelerated Jax based environments, however this package can be used for many more things. 

## Installing JumPy

To install JumPy from pypi:

```
python3 -m venv env
source env/bin/activate
pip install --upgrade pip
pip install brax-jumpy
```

Alternatively, to install JumPy from source, clone this repo, `cd` to it, and then:

```
python3 -m venv env
source env/bin/activate
pip install --upgrade pip
pip install -e .
```
