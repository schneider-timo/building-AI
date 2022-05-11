import numpy as np

def generate(p1):
    # change this so that it generates 10000 random zeros and ones
    # where the probability of one is p1
    seq = np.random.choice([0,1], p=[1-p1, p1], size=10000)
    return seq

def count(seq):
    five1s = 0
    ones = 0
    for number in seq:
        if number == 1:
            ones += 1
            if ones >= 5:
                five1s += 1
        else:
            ones = 0
    return five1s

def main(p1):
    seq = generate(p1)
    return count(seq)

print(main(2/3))
