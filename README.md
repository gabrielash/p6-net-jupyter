# Net::Jupyter

## SYNOPSIS

Net::Jupyter is a Perl6 Jupyter kernel

## Introduction

  This is a perl6 kernel for jupyter

  only the minumum required messages are implemented: kernel_info_request and execute_request

#### Status

  In development.

  Todo:
  1. Implement Magic statements
  2. Implement additional messages


#### Alternatives

  1. https://github.com/timo/iperl6kernel

  2. https://github.com/bduggan/p6-jupyter-kernel


#### Portability
  relies on Net::ZMQ


## Documentation

  see http://jupyter.org/

## Installation

  The module files are installed normally, but the kernel must be installed separately.

  There is an installation script in the bin directory. It can also be run with 'make install.'

  Assuming jupyter is already installed on your system, and  LOCAL_HOME is defined,

  it will try to install in the correct .local subdir that Anaconda recognizes

  for jupyter kernels.  You can also specify a custom dirctory as an argument

  or you can read the script and install manually.
