# Experiment-2
## NUMERICAL PYTHON (NUMPY)

### NORMALIZATION PROBLEM
```
#Access numpy library
import numpy as np

#Create a randomly-generated 5x5 array called X
X = np.random.random((5,5))

#Formulate the equation for Normalization
mean = X.mean()
std = X.std()
Z = (X - mean) / std

#Save normalized array
np.save('X_normalized.npy', Z)

#Print arrays
print("Random Array: \n", X)
print("\nNormalized Array: \n", Z)
```

### DIVISIBLE BY 3 PROBLEM
```
#Access numpy library
import numpy as np

#Create array of first 100 positive integers
INT = np.arange(1,101,1) 

#Make an array of the square of INT
square = INT**2

#Reshape A as a 10x10 array
A = square.reshape((10,10))

#Determine which elements are divisible by 3
DB3 = A[A % 3 == 0]
#Save array as  div_by_3.npy
np.save('div_by_3.npy', DB3)

#Print arrays
print("A =\n", A)
print ("\nElements divisible by 3: \n", DB3) 
```
