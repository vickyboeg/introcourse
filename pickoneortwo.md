introcourse
===========

code from the course introduction to programming
author = 'bogrenv'

import random

n1 = raw_input("Player one: ") n2 = raw_input("Player two: ") name = n2 rnd = int(random.randint (15, 25)) print(rnd*"|")

while(rnd>0): if name == n1: name = n2 else: name = n1 p1 = raw_input("%s, pick one or two: " % name)

while not p1.isdigit():

    print("No, it has to be a digit!")
    p1 = raw_input("%s, pick one or two: " % name)

p11 = int(p1)

while (p11>2):

    print("No, it has to be one or two!")
    p11 = int(raw_input("%s, pick one or two: " % name))

rnd = rnd - p11
print rnd*"|"

print("%s, YOU WON!!!!" % name)
