import numpy as np

# data
X = np.array([[66, 5, 15, 2, 500], 
              [21, 3, 50, 1, 100], 
              [120, 15, 5, 2, 1200]])
y = np.array([250000, 60000, 525000])

# alternative sets of coefficient values
c = np.array([[3000, 200 , -50, 5000, 100], 
              [2000, -250, -100, 150, 250], 
              [3000, -100, -150, 0, 150]])   

def find_best(X, y, c):
    smallest_error = np.Inf
    best_index = -1
    current_index = 0
    for coeff in c:
        err = 0
        for i in range(0,len(y)):
            coeff_at_x = coeff@X[i]
            difference = y[i] - coeff_at_x
            err += difference*difference
        if err < smallest_error:
            smallest_error = err
            best_index = current_index
        current_index += 1
    print("the best set is set %d" % best_index)


find_best(X, y, c)
