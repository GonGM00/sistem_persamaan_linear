# sistem_persamaan_linear
coba coba

import numpy as np

# Sistem:
# 2x + y = 5
# x + y = 3

A = np.array([[2, 1],
              [1, 1]])
B = np.array([5, 3])

# Metode invers matriks
A_inv = np.linalg.inv(A)
X = A_inv.dot(B)

print("Solusi dengan metode invers:")
print("x =", X[0])
print("y =", X[1])

# Metode eliminasi Gauss
X_gauss = np.linalg.solve(A, B)
print("\nSolusi dengan eliminasi Gauss:")
print("x =", X_gauss[0])
print("y =", X_gauss[1])
