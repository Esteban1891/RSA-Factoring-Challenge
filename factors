#!/usr/bin/python3
from sys import argv
from math import sqrt


def factor():
    with open(argv[1]) as f:
        for line in f:
            num = int(line)
            print("{:d}=".format(num), end="")
            if num % 2 == 0:
                print("{}*2".format(num//2))
                continue
            sqn = int(sqrt(num))
            if sqn % 2 == 0:
                sqn += 1
            for i in range(3, sqn + 1, 2):
                if num % i == 0:
                    print("{}*{}".format(i, num//i))
                    break
            if num % i != 0:
                print("{}={}*1".format(num, num))


factor()
