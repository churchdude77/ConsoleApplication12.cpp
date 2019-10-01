# ConsoleApplication12.cpp
/* Prime Number or Not */
#include<conio.h>
#incude<math.h>


void main() {


int n, i = 2, flag = 0;
clrscr();

cout << "Enter a positive integer value:";
cin >> n;

/* Loop to check whether 'n' is divisible by any number between 2 and sqrt(n) */
while (i <= sqrt(n))
{
    if (n % i == 0)
    {
        flag = 1;
        break;
        }
        i++;
      }
      
      /* if else condition to print Prime Number or Not */
      if (flag ==0)
          cout << n << "is a prime number.";
      else
          cout << n << "is not a prime number.";
       getch();
       
       return 0;
 }
