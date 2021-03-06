# 18daycycle

This is a program to calculate the current position in the 18 day cycle. 

It contains unit tests which test accuracy, and a php script to input and
display the position in the cycle. 

## Requirements

- `python3`
- `php` 
- `pyyaml` (python library)

## Installation

Install this program by cloning this git repo:

`git clone https://github.com/blincx/18daycycle.git`

`pip3 install -r requirements.txt`
    
Now launch your php server, making sure it points to the php files included.
And navigate your browser to `cycle18.php`.

Voila, you should be able to enter your birthdate and see it working.


## Two modes of calling the program

This program can be called in two ways: 
- Through the PHP front-end provided in cycle18.php
- Through command line arguments

Calling through the command line can be done like this:
- `python3 18daycycle.py 1930-02-27`
optional extra parameters are `debug` and `json`
- `python3 18daycycle.py 1943-07-16 debug`
- `python3 18daycycle.py 1987-07-08 json`

## Logging

Look in `logs/18daycycle.log` for logging data

## Running in debug mode

Either change `DEBUGSWITCH` in `18daycycle.py`, or supply "debug" argument to your normal call from the command line. 

Leaving it in `DEBUG` mode will log several (>6) lines per request, be wary of
overloading disk space. 

## Unit tests

I calculated some examples of 18 day cycle coordinates by hand and the machinery
of the scripts can be tested against these hand-calculated coordinates by
running:

`python3 test18.py`


## Browser testing

The php and javascript in this repo has been tested against the latest versions
of the following browsers:

- Chrome
- Firefox
- Opera
- Safari

It has not yet been tested against Internet Explorer. 

### thanks!
