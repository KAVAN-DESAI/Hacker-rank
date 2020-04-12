# Hacker-rank
Hacker rank python solution

Task
Read an integer N. For all non-negative integers i<N, print i^2. See the sample for details.

Input Format

The first and only line contains the integer,N.

Constraints
1<=N<=20

Output Format

Print N lines, one corresponding to each .

Sample Input 0

5
Sample Output 0

0
1
4
9
16
#
SOLUTION!!

if __name__ == '__main__':

    n = int(input())
    
for i in range(0,n):

    print(i*i)
