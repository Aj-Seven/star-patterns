<h1 align="center"> star-pattern-codes </h1>

> It is the curated list of star pattern codes.

## Table of Content: Pattern Codes

* [C Star Pattern Codes](#c-pattern-codes)
    * [Square Pattern](#1-square-pattern)
    * [Hallow Square Pattern](#2-hallow-square-pattern)
    * [Right Triangle Pattern](#3-right-triangle-pattern)
    * [Inverted Right Triangle Pattern](#4-inverted-right-triangle-pattern)
    * [Left Triangle Pattern](#5-left-triangle-pattern)
    * [Inverted Left Triangle Pattern](#6-inverted-left-triangle-pattern)

# C Star Pattern Codes
## 1. Square Pattern
``` c
#include <stdio.h>

int main() {
  // take a size
  // you can take user input by scan Function
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
  // or take user input by scan Function
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
## 3. Right Triangle Pattern
``` c
#include <stdio.h>

int main() {
  // set size
  // or take user input by scan Function
  int size = 5;

  for (int i = 0; i < size; i++) {
    // printing spaces before stars
    for (int j = 1; j < size-i; j++) {
      printf(" ");
    }
    // printing stars
    for (int k = 0; k <= i; k++) {
      printf("*");
    }
    printf("\n");
  }
  return 0;
}
```
## Output
``` c
    *
   **
  ***
 ****
*****
```

## 4. Inverted Right Triangle Pattern
``` c
#include <stdio.h>

int main() {
  // take size
  // or take user input by scan Function
  int size = 5;

  for (int i = 0; i < size; i++) {
    // printing spaces
    for (int j = 0; j < i; j++) {
      printf(" ");
    }
    // printing stars
    for (int j = size; j > i; j--) {
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
 ****
  ***
   **
    *
```

## 5. Left Triangle Pattern
``` c
#include <stdio.h>

int main() {
  // take size of triangle
  // or take user input by scan Function
  int size = 5;
  
  for (int i = 0; i < size; i++) {
    // printing star in a row
    for (int j = 0; j <= i; j++) {
      printf("*");
    }
    printf("\n");
  }
  return 0;
}
```
## Output
``` c
*
**
***
****
*****
```
## 6. Inverted Left Triangle Pattern
``` c
#include <stdio.h>

int main() {
  // size of the triangle
  int size = 5;

  for (int i = 0; i < size; i++) {
    // printing stars
    for (int j = 0; j < size-i; j++) {
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
****
***
**
*
```

