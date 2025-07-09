# Reading the number written in base 8 from right to left,
# keeping the leading 0's, if any:
# 0: move N     1: move NW    2: move W     3: move SW
# 4: move S     5: move SE    6: move E     7: move NE
#
# We start from a position that is the unique position
# where the switch is ON.
#
# Moving to a position switches ON to OFF, OFF to ON there.


import sys

ON = '\u26aa'
OFF = '\u26ab'
code = input('Enter a non-strictly negative integer: ').strip()
try:
    if code[0] == '-':
        raise ValueError
    int(code)
except ValueError:
    print('Incorrect input, giving up.')
    sys.exit()
nb_of_leading_zeroes = 0
for i in range(len(code) - 1):
    if code[i] == '0':
        nb_of_leading_zeroes += 1
    else:
        break
print("Keeping leading 0's, if any, in base 8,", code, 'reads as',
      '0' * nb_of_leading_zeroes + f'{int(code):o}.')
print()

# INSERT YOUR CODE HERE