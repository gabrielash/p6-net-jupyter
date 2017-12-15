# Net::Jupyter

## SYNOPSIS

Net::Jupyter is a Perl6 Jupyter kernel

## Introduction

  This is a perl6 kernel for jupyter

  only the minumum required messages are implemented: kernel_info_request and execute_request

#### Status

  In development.

  Todo:
  1. Implement Magic statements (see section below)
  2. Implement additional messages


#### Alternatives

  1. https://github.com/timo/iperl6kernel

  2. https://github.com/bduggan/p6-jupyter-kernel


#### Portability
  relies on [Net::ZMQ](https://github.com/gabrielash/perl6-zmq)


## Documentation

  see also http://jupyter.org/

### Installation

First, install the  module: 

    git clone https://github.com/gabrielash/p6-net-jupyter
    cd p6-net-jupyter
    zef install .

then, install the kernel:

    bin/kernel-install.sh

Assuming jupyter is already installed on your system, and  LOCAL_HOME is defined,
it will try to install in the correct .local subdir that Anaconda recognizes
for jupyter kernels.  You can also specify a custom dirctory as an argument
or you can read the script and install manually.

### Magic declarations

magic declrations are lines beginning and ending with %%.

All magic declarations must come at the top, and cannot be interleaved 
with Perl6 code.

#### Implemented: 

    %% timeout 5 %%  
    # sets a timeout on execution


