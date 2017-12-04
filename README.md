# Scalation Kernel

## Overview

The **Scalation Kernel** project provides a lightweight
[Scala](http://www.scala-lang.org)
[ScalaTion](http://cobweb.cs.uga.edu/~jam/scalation.html) kernel for
Jupyter notebooks. 
More information is available on the
[project page](https://github.com/scalation/scalation_kernel).

## Installation

Installation requires a recent ScalaTion distribution (>= 1.3) from
[here](http://cobweb.cs.uga.edu/~jam/scalation.html). Once you have
ScalaTion, make sure the ``SCALATION_JARS`` environment variable is
set appropriately before continuing. This can be done individually,
as seen here:

```
$ export SCALATION_JARS=/path/to/scalation_mathstat.jar
$ export SCALATION_JARS=/path/to/scalation_modeling.jar:$SCALATION_JARS
```

It can also be done with a single command if you know the path to the
``scalation_models`` directory:

```
$ export SCALATION_JARS=$(find /path/to/scalation_models/lib | grep .jar | paste -sd ":" -)
```

To install **Scalation Kernel** from PyPI, you can use the commands:

```
$ python3 -m pip install -U scalation_kernel
$ python3 -m scalation_kernel.install
```

More installation options are presented in the
[Installation Guide](https://github.com/scalation/scalation_kernel/blob/master/INSTALL.md),
including deployment options for Python virtual environments and
Docker containers. 

## Using ScalaTion Kernel

The *New* menu in Jupyter should show an option to create a ScalaTion
notebook using the installed kernel. 

A [User Guide](https://github.com/scalation/scalation_kernel/blob/master/USER.md)
is currently under development. A complete draft is planned for the next minor
release. Until then, please see the collection of
[example notebooks](https://github.com/scalation/scalation_kernel/tree/master/notebooks)
for usage examples.

## License

This software is free and open source under an
[MIT License](https://github.com/scalation/scalation_kernel/blob/master/LICENSE.md).
The content and opinions expressed on this Web page do not necessarily
reflect the views of nor are they endorsed by the University of Georgia or
the University System of Georgia.

