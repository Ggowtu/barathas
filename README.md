
1)Write a program to Swap to two numbers.

#include <iostream>  
Using namespace std;  
Int main()  
{  
Int a=5, b=10;      
Cout<<”Before swap a= “<<a<<” b= “<<b<<endl;      
A=a+b; //a=15 (5+10)    
B=a-b; //b=5 (15-10)    
A=a-b; //a=10 (15-5)    
Cout<<”After swap a= “<<a<<” b= “<<b<<endl;      
Return 0;  
}  

2) Write a program to find the largest number among three numbers entered by the user.

#include<iostream>
Using namespace std;
Int main() {
	Int num1,num2,num3;
	Cout<<” Enter value for first number”;
	Cin>>num1;
	Cout<<” Enter value for second number”;
	Cin>>num2;
	Cout<<” Enter value for third number”;
	Cin>>num3;
	If(num1>num2&&num1>num3) {
		Cout<<” First number is greatest:”<<endl<<”whick is= “<<num1;
	} else if(num2>num1&&num2>num3) {
		Cout<<” Second number is greatest”<<endl<<”whick is= “<<num2;
	} else {
		Cout<<” Third number is greatest”<<endl<<”whick is= “<<num3;
	}
	Return 0;
}

3)Write a program to check whether a year entered by a user is Leap year or not.
#include<iostream>
Using namespace std;
Int main() {
   Int year = 2016;
   If (((year % 4 == 0) && (year % 100 != 0)) || (year % 400 == 0))
   Cout<<year<<” is a leap year”;
   Else
   Cout<<year<<” is not a leap year”;
   Return 0;
}

4)Write a program to display Fibonacci Series upto nth term. (Using loops)

  #include<iostream>
    Using namespace std;
    Int main()
    {
    Int limit, first=0, second=1, next, num;
    Cout <<“Enter the limit of Fibonacci series”<<endl;
    
    Cin >> num;   
    Cout << “First “<<num<<” terms of Fibonacci series are :- “<<endl;
    For(int p=0;p<num;p++)
    {
        If (p <= 1)
            Next = p;
        Else
        {
            Next = first + second;
            First = second;
            Second = next;
        }
        Cout<<next<<” “;
    }
    Return 0;
    }

5) Write a program to check whether a number is Prime or Not.
#include <iostream>  
Using namespace std;  
Int main()  
{  
  Int n, I, m=0, flag=0;  
  Cout << “Enter the Number to check Prime: “;  
  Cin >> n;  
  M=n/2;  
  For(I = 2; I <= m; i++)  
  {  
      If(n % I == 0)  
      {  
          Cout<<”Number is not Prime.”<<endl;  
          Flag=1;  
          Break;  
      }  
  }  
  If (flag==0)  
      Cout << “Number is Prime.”<<endl;  
  Return 0;  
} 

6) Print this pattern using loops For n=5         *        * *      * * *      * * * *     * * * * *


#include <iostream>

Using namespace std;

Void pypart2(int n)
{

    Int I, j, k = n;

    For (I = 1; I <= n; i++){

        For (j = 1; j <= n; j++) {

            If (j >= k)

                Cout << “* “;

            Else

                Cout << “  “;

        }

        k--;

        cout << “\n”;

    }
}

Int main()
{

    Int n = 5;

    Pypart2(n);

    Return 0;
}

7)Write a program that takes n elements from the user and displays the second largest element of an array.

#include <iostream>
Using namespace std;
Int main(){
   Int n, num[50], largest, second;
   Cout<<”Enter number of elements: “;
   Cin>>n;
   For(int i=0; i<n; i++){
      Cout<<”Enter Array Element”<<(i+1)<<”: “;
      Cin>>num[i];
   }
   
   If(num[0]<num[1]){ 
      Largest = num[1];
      Second = num[0];
   }
   Else{ 
      Largest = num[0];
      Second = num[1];
   }
   For (int I = 2; i< n ; I ++) {
      
      If (num[i] > largest) {
         Second = largest;
         Largest = num[i];
      }
      Else if (num[i] > second && num[i] != largest) {
         Second = num[i];
      }
   }
   Cout<<”Second Largest Element in array is: “<<second;
   Return 0;
}

