#!/usr/bin/env bash
# read from file given as argv[1] ($1) and print factors for each num in file

FILE=$1

while read NUM
do
    factors=($(factor $NUM))
    echo "$NUM=$(($NUM/${factors[1]}))*${factors[1]}"
done < $FILE
