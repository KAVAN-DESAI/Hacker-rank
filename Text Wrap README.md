# Hacker-rank
Hacker rank python solution

You are given a string S and width W.
Your task is to wrap the string into a paragraph of width W.

Input Format

The first line contains a string, S.
The second line contains the width, W.

Constraints

0<len(S)<1000

0<W<len(S)

Output Format

Print the text wrapped paragraph.

Sample Input 0

ABCDEFGHIJKLIMNOQRSTUVWXYZ
4
Sample Output 0

ABCD
EFGH
IJKL
IMNO
QRST
UVWX
YZ
#
SOLUTION!!!


def wrap(string, max_width):

    wrapper = textwrap.TextWrapper(width=max_width)
    
    string1 = wrapper.fill(text=string) 
    
    return string1
