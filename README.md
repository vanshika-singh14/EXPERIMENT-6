# EXPERIMENT-6
## AIM:
This C++ code aims to demonstrate the use of various looping constructs and nested loops.
## theory:
We would be discussing about various Looping Constructs
1.	do-while Loop: Executes the code block once, then repeats as long as the condition remains true.
2.	for Loop: Repeats code a specific number of times, based on initialization, condition, and increment.
3.	while Loop: Repeats code as long as the specified condition is true.
4.	Nested for Loops: Multiple for loops inside each other, often used for iterating over multi-dimensional data.
5.	Nested do-while Loops: Multiple do-while loops within each other, executing inner blocks multiple times based on conditions.
6.	Nested while Loops: Multiple while loops within each other, where the inner loop completes all its iterations before the outer loop continues.
7.	Nested for Loops (Matrix): A pair of for loops used to iterate over rows and columns of a matrix.
8.	Nested for + while Loops (Matrix with Condition): A for loop with an inner while loop to process matrix elements conditionally.

#include <iostream>
using namespace std; 

int main()
{
    //do-while
    cout<<"Using do while loop: "<<endl;
    int a = 10;
    do
    {
        cout<<a<<endl;
        a--;
    } while (a != 0);

    cout<<endl;
    cout<<endl;

   //for loop
    cout<<"Using for loop: "<<endl;
    int i = 0;
    for(i = 0; i <=10;i++)
    {
        cout<<i<<endl;
    }
    cout<<endl;
    cout<<endl;

    //while loop
    cout<<"Using while: "<<endl;
    int b = 10;
    while(b>0)
    {
        cout<<b<<endl;
        b--;
    }
    cout<<endl;
    cout<<endl;

    //for loop
    cout<<"Using for: "<<endl;
    for(i = 0; i <=100; i = i + 5 )
    {
         cout<<i<<endl;
    }
    cout<<endl;
    cout<<endl;

    //nested for - pattern
    cout<<"Using nested for loops for pattern: "<<endl;
    int ii,j,k = 0,n2 = 5;
    for(ii = 1; ii <= n2; ii++)
    {
        for(j = 1; j <= (n2-ii);j++)
        {
            cout<<" ";
            while(k != (2*ii-1))
            {
                cout<<"* ";
                k++;
            }
            k=0;
            cout<<endl;    
        }   
        cout<<endl;
    }
    cout<<endl;
    cout<<endl;

    //nested do while
    cout<<"Using nested do-while to find the product of numbers:"<<endl;
    int q = 0,r = 0;
    do
    {
        q++;
        do
        {
            r++;
            cout<<"Product of two numbers:  "<<q*r<<endl;
        }while(r<10);
        

    } while(q<10);
    cout<<endl;
    cout<<endl; 

    //nested while
    cout<<"Sum of 2 numbers using nested while: "<<endl;
    int q2 = 10, r2 = 10;
    while(q2>0)
    {
        q2--;
        while(r2>0)
        {
            r2--;
            cout<<"Sum: "<<q2+r2<<endl;
        }

    }
    cout<<endl;
    cout<<endl; 
    
    //nested for - matrix
    cout<<"Using nested for loops for matrix: "<<endl;
    int m,n,p;
    int mat[2][2][2] = {
                            {
                                {1, 2},
                                {3, 4}
                            }, 
                            {
                                {5, 6}, 
                                {7, 8}
                            }
                        };

    for (int m = 0; m < 2; ++m) 
    {
        for (int n = 0; n < 2; ++n) 
        {
            for (int p = 0; p < 2; ++p) 
            {
                cout<<mat[m][n][p];
            }
            cout<<endl;
        }
    }
    cout<<endl;
    cout<<endl; 
    
    //nested for + while - matrix
    cout<<"Using nested for loops and while for matrix and checking some condition: "<<endl;
        int m1,n1,p1;
        int mat1[2][2][2] = {
                                {
                                    {1, 2},
                                    {3, 4}
                                }, 
                                {
                                    {5, 6}, 
                                    {7, 8}
                                }
                            };

        for (int m1 = 0; m1 < 2; ++m1) ![image](https://github.com/user-attachments/assets/a439e80e-7325-489b-895e-a846a136ebd7)

        {
            for (int n1 = 0; n1 < 2; ++n1) 
            {
                for (int p1 = 0; p1 < 2; ++p1) 
                {
                    while(mat1[m1][n1][p1] < 8)
                    {
                        cout<<mat1[m1][n1][p1];
                        break;

                    }
                    
                }
                cout<<endl;
            }
        }
    cout<<endl;
    cout<<endl; 

   return 0;
}


*/ output
Using do while loop: 
10
9
8
7
6
5
4
3
2
1


Using for loop: 
0
1
2
3
4
5
6
7
8
9
10


Using while: 
10
9
8
7
6
5
4
3
2
1


Using for:
0
5
10
15
20
25
30
35
40
45
50
55
60
65
70
75
80
85
90
95
100


Using nested for loops for pattern:
 *
 *
 *
 *

 * * * 
 * * *
 * * *

 * * * * *
 * * * * *

 * * * * * * *




Using nested do-while to find the product of numbers:
Product of two numbers:  1
Product of two numbers:  2
Product of two numbers:  3
Product of two numbers:  4
Product of two numbers:  5
Product of two numbers:  6
Product of two numbers:  7
Product of two numbers:  8
Product of two numbers:  9
Product of two numbers:  10
Product of two numbers:  22
Product of two numbers:  36
Product of two numbers:  52
Product of two numbers:  70
Product of two numbers:  90
Product of two numbers:  112
Product of two numbers:  136
Product of two numbers:  162
Product of two numbers:  190


Sum of 2 numbers using nested while:
Sum: 18
Sum: 17
Sum: 16
Sum: 15
Sum: 14
Sum: 13
Sum: 12
Sum: 11
Sum: 10
Sum: 9


Using nested for loops for matrix:
12
34
56
78


Using nested for loops and while for matrix and checking some condition:
12
34
56
7
*/
## Conclusion:
We learnt about loops and their use case.
