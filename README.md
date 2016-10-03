# RNN training on the Polyphonic Music dataset

The original polyphonic music data can be downloaded from http://www-etud.iro.umontreal.ca/~boulanni/icml2012, we process the cPickle file into .mat format.

## Dependencies

This code is written in python. To use it you will need:

* Python 2.7
* [Theano 0.7](http://deeplearning.net/software/theano/)
* A recent version of [NumPy](http://www.numpy.org/) and [SciPy](http://www.scipy.org/)

## How to use the code

This code can be run in CPU/GPU devices directly.  

Example commands:

Running any optimization algorithm (i.e. SGD, SGD-M, RMSprop & Adam):

    python eval_music.py sys.argv[1] sys.argv[2]

Two examples:
    python eval_music.py Piano SGD
    python eval_music.py JSB Adam

sys.argv[1] indicates which dataset to use, sys.argv[2] indicates which algorithm to use.

## Output

In order to monitor the training process, all the output information will be printed out in the .log file.
The final parameters we learned will be stored in a .npz file. 


