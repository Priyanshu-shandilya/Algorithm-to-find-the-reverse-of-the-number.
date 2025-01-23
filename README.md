# Algorithm-to-find-the-reverse-of-the-number.

#include <stdio.h>

int main() {
  int n, reverse = 0, remainder, original;

  printf("Enter an integer: ");
  scanf("%d", &n);

  original = n;  

  while (n != 0) {
    remainder = n % 10;
    reverse = reverse * 10 + remainder;
    n /= 10;
  }
  printf("the reverse of the number is %d",reverse);
}

Input: 123
Output:321
