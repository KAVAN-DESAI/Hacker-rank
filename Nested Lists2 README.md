# Hacker-rank
Hacker rank python solution

Given the names and grades for each student in a Physics class of N students, store them in a nested list and print the name(s) of any student(s) having the second lowest grade.

Note: If there are multiple students with the same grade, order their names alphabetically and print each name on a new line.

Input Format

The first line contains an integer, N, the number of students.
The 2N subsequent lines describe each student over 2 lines; the first line contains a student's name, and the second line contains their grade.

Constraints
2<=N<=5
There will always be one or more students having the second lowest grade.
Output Format

Print the name(s) of any student(s) having the second lowest grade in Physics; if there are multiple students, order their names alphabetically and print each one on a new line.

Sample Input 0

5
Harry
37.21
Berry
37.21
Tina
37.2
Akriti
41
Harsh
39
Sample Output 0

Berry
Harry
Explanation 0

There are 5 students in this class whose names and grades are assembled to build the following list:

python students = [['Harry', 37.21], ['Berry', 37.21], ['Tina', 37.2], ['Akriti', 41], ['Harsh', 39]]

The lowest grade of 37.2 belongs to Tina. The second lowest grade of 37.21 belongs to both Harry and Berry, so we order their names alphabetically and print each name on a new line.
#
SOLUTION!!!

if __name__ == '__main__':

    list1=[]
    
    list2=[]
    
    list3=[]
    
    for _ in range(int(input())):
    
        name = input()
        
        score = float(input())
        
        list1.append(name)
        
        list2.append(score)
        
        list3.append([score,name])
        
    list2.sort()
    
    list3.sort()
    
    secondlowest=0
    
    if(list2[0]!=list2[1] and len(list2)>1 and len(list2)<6):
    
        if(list2[1]==list2[2]):
        
            print(list3[1][1])
            
            print(list3[2][1])
            
        elif(list2[1]!=list2[2]):
        
            print(list3[1][1])
            
    elif(list2[0]==list2[1] and len(list2)>1 and len(list2)<6):
    
        if(list2[1]==list2[2]):
        
            print(list3[3][1])
            
        elif(list2[1]!=list2[2]):
        
            if(list2[2]==list2[3]):
            
                print(list3[2][1])
                
                print(list3[3][1])
                
            elif(list2[2]!=list2[3]):
            
                print(list3[2][1])
                
