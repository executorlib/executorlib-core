# executorlib-core

[![Coverage Status](https://coveralls.io/repos/github/executorlib/executorlib-core/badge.svg?branch=main)](https://coveralls.io/github/executorlib/executorlib-core?branch=main)
[![Unittests](https://github.com/executorlib/executorlib-core/actions/workflows/unittest.yml/badge.svg)](https://github.com/executorlib/executorlib-core/actions/workflows/unittest.yml)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/executorlib/executorlib-core/HEAD?labpath=notebooks%2Fexample.ipynb)

The `executorlib-core` package is based on the [concurrent.futures.Executor](https://docs.python.org/3/library/concurrent.futures.html)
abstract class from the Python standard library to define `Executor` classes for specific application. This is achieved
by coupling two Python processes using [zeroMQ](https://zeromq.org) universal messaging library and serializing the 
Python objects using [cloudpickle](https://github.com/cloudpipe/cloudpickle) which extends the serialization support for
Python objects. 