while not summit:
        summit = True         # stop unless there's a way up
        for i in range(5):
            if h[x + i] > h[x]:
                x = x + i         # right is higher, go there
                summit = False    # and keep going
            elif h[x-i]>h[x]:
                x -=i
                summit = False
    return x
