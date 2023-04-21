<h1 align="center"> star-pattern-codes </h1>

> It is the curated list of star pattern codes.

## Table of Content: Pattern Codes

* [C Star Pattern Codes](#c-pattern-codes)
    * [Square Pattern](#1-square-pattern)
    * [Hollow Square Pattern](#2-hollow-square-pattern)
    * [Right Triangle Pattern](#3-right-triangle-pattern)
    * [Inverted Right Triangle Pattern](#4-inverted-right-triangle-pattern)
    * [Left Triangle Pattern](#5-left-triangle-pattern)
    * [Inverted Left Triangle Pattern](#6-inverted-left-triangle-pattern)
    * [Hollow Triangle Pattern](#7-hollow-triangle-pattern)
    * [Pyramid Pattern](#8-pyramid-star-pattern)
    * [Hollow Pyramid Pattern](#9-hollow-pyramid-pattern)
    * [Inverted Pyramid Pattern](#10-inverted-pyramid-pattern)
    * [Diamond Pattern](#11-diamond-pattern)
    * [Hollow Diamond Pattern](#12-hollow-diamond-pattern)
    * [Right Pascal Pattern](#13-right-pascal-pattern)
    * [Left Pascal Pattern](#14-left-pascal-pattern)
    * [Plus Sign Pattern](#15-plus-sign-pattern)
    * [Cross Sign Pattern](#16-cross-sign-pattern)
    * [Heart Pattern](#17-heart-pattern)

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

## 2. Hollow Square Pattern
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
## 7. Hollow Triangle Pattern
> It is like the triangle but it has the Hallow Space in the Middle
``` c
#include <stdio.h>

int main() {

  // take the size
  // or take user input by scan Function
  int size = 5;

  // creating hollow triangle
  for (int i = 1; i <= size; i++) {
    for (int j = 0; j < i; j++) {
      // operation of non-last row
      if (i != size) {
        // 1st or last position of row print star
        if (j == 0 || j == i-1) {
          printf("*");
        } else {
          printf(" ");
        }
      }
      // last row print only star
      else {
        printf("*");
      }
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
* *
*  *
*   *
******
```
## 8. Pyramid Star Pattern
``` c
#include <stdio.h>

int main() {
  //take the size
  //or take user input by scan Function
  int size = 5;

  // creating pyramid
  for (int i = 0; i < size; i++) {
    // print spaces before stars
    for (int j = 0; j < size-i-1; j++) {
      printf(" ");
    }
    // print stars
    for (int k = 0; k < 2*i+1; k++) {
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
   ***
  *****
 *******
*********
```

## 9. Hollow Pyramid Pattern
``` c
#include <stdio.h>

int main() {
  // size of the pyramid
  // or take user input by scan Function
  int size = 5;
  for (int  i = 0; i < size; i++) {
    // print spaces
    for (int j = 0; j < size-i-1; j++) {
      printf(" ");
    }
    // print stars
    for (int k = 0; k < 2*i+1; k++) {
      if(k == 0 || k == 2*i || i == size-1) {
        printf("*");
      } else {
        printf(" ");
      }
    }
    printf("\n");
  }
  return 0;
}
```
## Output
``` c
    *
   * *
  *   *
 *     *
*********
```

## 10. Inverted Pyramid Pattern
``` c
#include <stdio.h>

int main() {
  // size of the pyramid
  // or take user input by scan Function
  int size = 5;
  for (int i = 0; i < size; i++) {
    // print spaces
    for (int j = 0; j < i; j++) {
      printf(" ");
    }
    // print stars
    for (int k = 0; k < 2*(size-i)-1; k++) {
      printf("*");
    }
    printf("\n");
  }
  return 0;
}
```
## Output
``` c
*********
 *******
  *****
   ***
    *
```
## 11. Diamond Pattern
``` c
#include <stdio.h>

int main() {
  // size of Diamond
  // or take user input by scan Function
  int size = 5;
  // upside pyramid
  for (int i = 1; i <= size; i++) {
    // printing spaces
    for (int j = size; j > i; j--) {
      printf(" ");
    }
    // printing star
    for (int k = 0; k < i*2-1; k++) {
      printf("*");
    }
    printf("\n");
  }
  // downside pyramid
  for (int i = 1; i <= size-1; i++) {
    // printing spaces
    for (int j = 0; j < i; j++) {
      printf(" ");
    }
    // printing star
    for (int k = (size-i)*2-1; k > 0; k--) {
      printf("*");
    }
    printf("\n");
  }
  return 0;
}
```
## Output
```
    *
   ***
  *****
 *******
*********
 *******
  *****
   ***
    *
```

## 12. Hollow Diamond Pattern
``` c
#include <stdio.h>

int main() {
  // size of hollow Diamond
  // or take user input by scan Function
  int size = 5;
  // upside pyramid
  for (int i = 1; i <= size; i++) {
    // printing spaces
    for (int j = size; j > i; j--) {
      printf(" ");
    }
    // printing star
    for (int k = 0; k < i*2-1; k++) {
      if (k == 0 || k == 2*i-2) {
        printf("*");
      }
      else {
        printf(" ");
      }
    }
    printf("\n");
  }
  // downside triangle
  for (int i = 1; i < size; i++) {
    // printing spaces
    for (int j = 0; j < i; j++) {
      printf(" ");
    }
    // printing star
    for (int k = (size-i)*2-1; k >= 1; k--) {
      if (k == 1 || k == (size-i)*2-1) {
        printf("*");
      }
      else {
        printf(" ");
      }
    }
    printf("\n");
  }
  return 0;
}
```
## Output
``` c
    *
   * *
  *   *
 *     *
*       *
 *     *
  *   *
   * *
    *
```
## 13. Right Pascal Pattern
``` c
#include <stdio.h>

int main() {
  // size right pasal triangle
  // or take user input by scan Function
  int size = 5;

  for (int i = 1; i <= size; i++) {
    for (int j = 0; j < i; j++) {
      printf("*");
    }
    printf("\n");
  }
  
  for (int i = 1; i <= size-1; i++) {
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
*
**
***
****
*****
****
***
**
*
```

## 14. Left Pascal Pattern
``` c
#include <stdio.h>

int main() {
  // size left pasal triangle
  // or take user input value by scan Function
  int size = 5;

  for (int i = 1; i <= size; i++) {
    for (int j = 0; j < size-i; j++) {
      printf(" ");
    }
    for (int k = 0; k < i; k++) {
      printf("*");
    }
    printf("\n");
  }
  for (int i = 1; i <= size-1; i++) {
    for (int j = 0; j < i; j++) {
      printf(" ");
    }
    for (int k = 0; k < size-i; k++) {
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
 ****
  ***
   **
    *
```
## 15. Plus Sign Pattern
``` c
#include <stdio.h>

int main() {
  // size of plus, use odd number
  int size = 5;

  for (int i = 0; i < size; i++) {
    for (int j = 0; j < size; j++) {
      // print only stars in middle row
      if (i == size / 2) {
        printf("*");
      }
      // other than middle row, print star only at index size/2
      else {
          if (j == size / 2) {
          printf("*");
        } else {
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
```
  *
  *
*****
  *
  *
```

## 16. Cross Sign Pattern
``` c
#include <stdio.h>

int main() {
  // size of cross, use odd number
  int size = 5;

  for (int i = 0; i < size; i++) {
    for (int j = 0; j < size; j++) {
      if (i==j || i+j==size-1) {
        printf("*");
      } else {
        printf(" ");
      }
    }
    printf("\n");
  }
  return 0;
}
```
## Output
``` c
*   *
 * * 
  *  
 * * 
*   *
```

## 17. Heart Pattern
``` c
#include <stdio.h>

int main() {
  // size of heart star pattern
  int size = 6;

  for (int i = size / 2; i < size; i += 2) {
    // print first spaces
    for (int j = 1; j < size-i; j += 2) {
      printf(" ");
    }
    // print first stars
    for (int j = 1; j < i+1; j++) {
      printf("*");
    }
    // print second spaces
    for (int j = 1; j < size-i+1; j++) {
      printf(" ");
    }
    // print second stars
    for (int j = 1; j < i+1; j++) {
      printf("*");
    }
    printf("\n");
  }
  // lower part
  // inverted pyramid
  for (int i = size; i > 0; i--) {
    for (int j = 0; j < size-i; j++) {
      printf(" ");
    }
    for (int j = 1; j < i*2; j++) {
      printf("*");
    }
    printf("\n");
  }
  return 0;
}
```
## Output
``` c
 ***   ***
***** *****
***********
 *********
  *******
   *****
    ***
     *
```

