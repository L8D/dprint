#!/usr/bin/env python2
import sys
import time

# Find the -d arguement
if len(sys.argv) > 1:

  if sys.argv[1] == "-d":
    n = float(sys.argv[2])
    if len(sys.argv) > 3:
      text = sys.argv[3:]
    else:
      text = sys.stdin
  else:
    text = sys.argv[1:]
else:
  n = 0.07
  text = sys.stdin

# Simple function to add up the strings in a list
def stringify(list):
  result = ""
  for i in list:
    result = result + " " + i
  return result[1:]

s = 0
# Delay
for i in stringify(text):
  if s == 1:
    s = 0
  else:
    time.sleep(n)
    sys.stdout.write(i)
    sys.stdout.flush()
  if i == "\n":
    time.sleep(0.5)
    s = 1
