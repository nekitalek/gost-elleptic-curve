# dedov_lab1_crypt
During the laboratory work, a program was developed that generates the parameters of an elliptic curve.
The starting point was the taking of the discriminant. By condition, it must be negative, not equal to zero modulo three and equal to one modulo 8. 
This condition was used to calculate the j-invariant in which the Weber polynomial is used. D=-7050359 was selected. 

Next, the number of classes was calculated based on the discriminant that was selected. The result was hD = 3652. This value satisfies the restriction set by the teacher, in which the number of classes must be more than 3000. 

To calculate the characteristic of the field p, random numbers a and b were found, because it was declared more equal that the discriminant is equal to 1 modulo 4. 

Then, the number of points m in p was found. By condition, one of the divisors m, r must be greater than $2^{252}$. If r is less than $2^{252}$, then the whole procedure with the selection of coefficients a, b and the calculation of p was repeated until the condition was met.

Further, using the Wolfram Math program and a script, the Weber polynomial and j-invariants on it were calculated. 
The calculations required a discriminant and a characteristic of the field. After the calculations, it was verified that none of the j-invariants is equal to 0 or 1728, because otherwise the curve will be isogenic curves that are not allowed by the GOST standard.
