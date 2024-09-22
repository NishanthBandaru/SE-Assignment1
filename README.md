# Fermat's Last Theorem Near Misses

## Overview
This project aims to find "near misses" for Fermat's Last Theorem in the form \(x^n + y^n \approx z^n\). According to Fermat's Last Theorem, there are no natural numbers \(x, y, z\) such that \(x^n + y^n = z^n\) for \(n > 2\). However, for given values of \(n\) and \(k\), this program searches for combinations of \(x, y, z\) that nearly satisfy this equation.

## Program Overview
This program allows interactive users to search for "near misses" in the formula \(x^n + y^n \approx z^n\), using positive integers \(x, y, z, n,\) and \(k\). The program systematically searches for the smallest relative miss and outputs the results.

## Requirements
- *Python 3.x*: Ensure that Python is installed on your machine.

## Utilization
1. *Clone the repository*:
   ```bash
     git clone https://github.com/NishanthBandaru/SE-Assignment1
       cd SE-Assignment1
2. Launch the Windows OS exe file
   ```bash
    ./dist/SE Assignment1.exe

  or 
  
 Run the Python script:

    
      python SE Assignment1.py. 
    
3. *Input values when prompted*:
- *\(n\)*: The power to apply in the calculation, between 3 and 11.
- *\(k\)*: The maximum value that \(x\) and \(y\) can take (must be greater than 10).

4. *Results*: The application will display the smallest relative miss for the given values of \(n\) and \(k\).

5. *Continue or Exit*: After the search finishes, the program will prompt you to input "yes" or "no" to determine whether you'd like to search for another set of values.

## Program Structure
### Primary Elements:
- **find_near_miss(n, k)**: This function handles the primary near-miss search. It iterates over potential values of \(x\) and \(y\) (from 10 to \(k\)) to find the smallest relative miss, computing the difference between \(x^n + y^n\) and the closest \(z^n\).

- **main()**: This function calls find_near_miss, manages user input, and validates values for \(n\) and \(k\).

## Implementation
- Users can experiment with different values of \(n\) and \(k\) as the script loops and asks after each run whether you'd like to continue the search.
