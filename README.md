#include <stdio.h>

int main() {

  double num1, num2, num3;

  printf("Enter first number: ");
  scanf("%lf", &num1);
  printf("Enter second number: ");
  scanf("%lf", &num2);
  printf("Enter third number: ");
  scanf("%lf", &num3);

  // if num1 is greater than num2 & num3, num1 is the largest
  if (num1 >= num2 && num1 >= num3)
    printf("%lf is the largest number.", num1);

  // if num2 is greater than num1 & num3, num2 is the largest
  if (num2 >= num1 && num2 >= num3)
    printf("%lf is the largest number.", num2);

  // if num3 is greater than num1 & num2, num3 is the largest
  if (num3 >= num1 && num3 >= num2)
    printf("%lf is the largest number.", num3);

  return 0;
}
Output:
C Program to find greatest of three numbers

Example 2: Program to find largest number using if..else statement
#include <stdio.h>
int main() {

  double num1, num2, num3;

  printf("Enter first number: ");
  scanf("%lf", &num1);
  printf("Enter second number: ");
  scanf("%lf", &num2);
  printf("Enter third number: ");
  scanf("%lf", &num3);

  if (num1 >= num2 && num1 >= num3)
    printf("%lf is the largest number.", num1);

  else if (num2 >= num1 && num2 >= num3)
    printf("%lf is the largest number.", num2);

  // if both the above conditions are false then
  // num3 is the largest number
  else
    printf("%lf is the largest number.", num3);

  return 0;
}
Output:

Enter first number: 10
Enter second number: 50
Enter third number: 1
50.000000 is the largest number.
Example 3: Program to find largest number using nested if..else
#include <stdio.h>

int main() {

  double num1, num2, num3;

  printf("Enter first number: ");
  scanf("%lf", &num1);
  printf("Enter second number: ");
  scanf("%lf", &num2);
  printf("Enter third number: ");
  scanf("%lf", &num3);

  if (num1 >= num2) {
    if (num1 >= num3)
      printf("%.2lf is the largest number.", num1);
    else
      printf("%.2lf is the largest number.", num3);
  }
  else {
    if (num2 >= num3)
      printf("%.2lf is the largest number.", num2);
    else
      printf("%.2lf is the largest number.", num3);
  }

  return 0;
}
