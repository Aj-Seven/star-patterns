<h1 align="center"> star-pattern-codes </h1>

> It is the curated list of star pattern codes.

## Table of Content: Pattern Codes

* [C Star Pattern Codes](#c-pattern-codes)
    * [Square Pattern](#1-square-pattern)
    * [Hallow Square Pattern](#2-hallow-square-pattern)


# C Star Pattern Codes
## 1. Square Pattern
``` c
#include <stdio.h>

int main() {
  // take a size
  // you can take user input
  int size = 5;
  // external loop
  for (int i = 0; i < size; i++) {
    // internal loop
    for (int j = 0; j < size; j++) {
      printf("*");
    }
    printf("\n");
  }
  return 0;
}
```
## Output
``` c
*****
*****
*****
*****
*****
```

## 2. Hallow Square Pattern
``` c
#include <stdio.h>

int main() {
  // size of the square
  int size = 5;
  // external loop
  for (int i = 0; i < size; i++) {
    // innternal loop
    for (int j = 0; j < size; j++) {
      // in first and last row print only stars
      if (i == 0 || i == size - 1) {
        printf("*");
      }
      else {
        // at first and last position
        // of row print stars else print spaces
          if (j == 0 || j == size - 1) {
          printf("*");
        }
        else {
          printf(" ");
        }
      }
    }
    printf("\n");
  }
  return 0;
}
```
## Output
``` c
*****
*   *
*   *
*   *
*****
```


