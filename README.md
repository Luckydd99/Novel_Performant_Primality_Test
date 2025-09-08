# Novel performant primality test on a Pell’s cubic
*Last updated on September 8, 2025*

This Github repository contains two files: this README and one single Python file.
The latter contains an implementation of a novel primality testing procedure.
This procedure runs linearly with respect to the length in binary of the analysed integer, and it is a primality criterion under $2^{36}$.
It achieves these amazing results using linear recurring sequences arising from powers of an element lying inside the projectivization of the Pell's cubic.
Please find the proof which classifies this algorithm as a primality test inside the official open-access mathematical paper [here](https://link.springer.com/article/10.1007/s00009-025-02839-w) or inside the arXiv pre-print [here](https://arxiv.org/abs/2411.01638).

The code was tested using Python 3.8.10 and Sympy 1.12.
Note that only the testing part of the code (see below the line `if __name__ == "__main__":`) requires to import the Sympy library, whereas all the functions defined in earlier lines require zero additional imports.
Keep reading for further information regarding the goals of the code found in the Python file.

## The main goals of this implementation

The implementation found in the Python file has been written with three main goals in mind: it had to be highly readable, it had to execute realiably, and it had to be easily tested by anoyone. 
Indeed, the Python language was chosen because of its readabilty, of its stability and of its wide-spread use.
Moreover, only the famous Sympy library is required to execute the tests written inside the Python file, whereas the functions defined in the file require zero further imports to be correctly executed.
This means that, in theory, anyone can download this repository and create with incredible ease a Python library on which further tests can be built.

The functions in the Python file were not written with the idea to prioritise execution speed.
Despite this, some effort was put in to shorten the execution times as much as possible within the realms of not importing any external libraries.
There are no doubts that an implementation in a programming language like C or Java can achieve faster execution times, but this rewriting could imply a loss of both readability and ease of executability.
Feel free to try to implement the primality test in a different programming language and to contact the authors of the paper for any doubts or any novel implementations.

Enjoy the rest of your day!
