# aosomer-adventure

overhang = input("Overhang: ")
slope = input("Slope: ")
eave = input("Eaves: ")
valley = input("valley: ")
warmwall = float(28)
base = warmwall + float(overhang)
hypotenuse = ((float(overhang) + warmwall) * float(slope)) / 12
a = hypotenuse ** 2
b = base ** 2
hyp = a + b

def square_root(hyp):
    from math import sqrt
    print(sqrt(hyp))

if hyp > 36:
    ice_barrier = (float(eave) * 6) + (float(valley) * 3)
else:
    ice_barrier = (float(eave) * 3) + (float(valley) * 3)

rolls = round(ice_barrier / 200)

print(f"The insurance should pay to cover: {ice_barrier}SF.  Which means you will need to order {rolls} rolls.")

