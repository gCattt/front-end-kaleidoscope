# front-end-kaleidoscope

A little compiler for a non-trivial language built for the Programming Languages and Compilers course @ UniMoRe.

## Table of Contents
- [Setup](#setup)
- [Usage](#usage)
  - [Testing](#testing)
- [Authors](#authors)
- [References](#references)
  
## Setup
For this project you need to install [llvm-17](https://releases.llvm.org/), [bison](https://www.gnu.org/software/bison/bison.html) and [flex](https://gothub.frontendfriendly.xyz/westes/flex/blob/master/README.md) on your machine.

Install **llvm-17** using the [automatic script](https://apt.llvm.org/).
```bash
 wget https://apt.llvm.org/llvm.sh
 chmod +x llvm.sh
 sudo ./llvm.sh 17
```
_You can delete the file llvm.sh after running it_

```bash
 sudo apt install bison flex
```
**NOTE**: check to have **make** and **wget** installed, otherwise install them with ```sudo apt install make wget``` 

## Usage

1. Clone the repository
```
git clone https://github.com/gCattt/front-end-kaleidoscope
```

2. Create the compiler binary ```kcomp```
```
cd front-end-kaleidoscope
make
``` 
This will create the **kcomp** compiler 

3. Compile your ```.k``` files using ```kcomp```
```bash
./kcomp <file.k> 2> <file.ll>
./tobinary <file.ll>
```

### Testing
Use the **test** folder as a "_workspace_" to create your own ```.k``` file and compile them adding proper instructions in the Makefile:
- floor &rarr; rounds down a number to the closest integer <= to that number (whole or fractional);
- rand  &rarr; generate and print 10 pseudorandom numbers;
- fibonacci &rarr; calculate the n-th Fibonacci number;
- sqrt  &rarr; calculate the (approximate) square root of an arbitrary number;
- eqn2  &rarr; calculate the solutions of a quadratic equation, given the coefficients a,b and c;
- sqrt2 &rarr; like sqrt but uses the logical operator 'or';
- sqrt3 &rarr; like sqrt but uses the logical operators 'and' and 'not'.

## Authors
 - [gCattt](https://github.com/gCattt)
 - [neRIccardo](https://github.com/neRIccardo)

## References
- https://llvm.org/docs/tutorial/MyFirstLanguageFrontend/index.html
