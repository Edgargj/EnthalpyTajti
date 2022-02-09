# EnthalpyTajti

EnthalpyTajti is a program that calculates the enthalpies of formation (by the Gaussian09 G4, G3, G3MP2, CBS-APNO and CBS-QB3 method) of gaseous atoms at 0 K (with the exception of carbon data 711.79 kJ/mol from A. Tajti et al. J. Chem. Phys. 121, 2004, 11599) and thermal corrections for elements in their standard state at 298.16 K from: NIST-JANAF Thermochemical Tables J. Physics Chem. Data Monograph 9, 1998, 1-1951.

# Git instructions

You can obtain the source code of EnthalpyTajti as follows.
In your bash terminal type:

~~~~~~~~~~
$cd /local/path/to/EnthalpyG4
$git clone https://github.com/Edgargj/EnthalpyTajti.git
~~~~~~~~~~

After this, git will transfer the source files to ```/local/path/to/EnthalpyTajti```

## Auxiliary programs/dependencies
The following dependencies are needed:

~~~~~~~~~~
g++ std=c++11 make
~~~~~~~~~~

## Installation
For installing the program, type:

~~~~~~~~~~
$cd /local/path/to/EnthalpyTajti
$make
~~~~~~~~~~

# Testing the program

How to test the program (or how it should be):

~~~~~~~~~~
$./computeEnthalpyNIST.x 4NBALa.txt
                                                                                                  
===================================================================================================
                      New calculation of molecular enthalpies of formation                         
                                                                                                   
       Enthalpies of formation of gaseous atoms at 0 K (with the exception of carbon data          
        711.79 kJ/mol from A. Tajti et al. J. Chem. Phys. 121, 2004, 11599) and thermal            
             corrections for elements in their standard states at 298.15 K from:                   
                                                                                                   
        NIST-JANAF Thermochemical Tables J. Physics Chem. Data Monograph 9, 1998, 1-1951.          
===================================================================================================
                                                                                                   
                                                                                                   
                                                                                                   
Heats of formation: 
0K          -33.82 kJ mol-1
0K          -8.08 kcal mol-1
                                                                                                   
Using Nicolaides method: 
298K        -56.33 kJ mol-1
298K        -13.45 kcal mol-1
                                                                                                   
Using G4 Enthalpy: 
298K        -53.84 kJ mol-1
298K        -12.86 kcal mol-1
                                                                                                   
===================================================================================================
~~~~~~~~~~

