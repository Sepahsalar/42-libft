# 42-libft
The main goal of this project is to build a library containing a variety of functions that will be used throughout the `42` Cursus. Most of the functions are low-level and work directly with memory management and allocation, key concepts of the `C` programming. Learning about the building and implementation of the `Makefile` is the core of the project.

</br>

# Content

1. [Usage](#usage)
2. [Description](#description)
3. [Functions](#functions)

</br>

## Usage

Follow the steps below to test the project: 

1. Clone the repository:
```bash
$> git clone https://github.com/Sepahsalar/42-libft.git
```
2. Compile the project:
```bash
$> make
```
3. And for the bonus part:
```bash
$> make bonus
```

</br>

## Description

**Libft (Library of Functions)**

In this project, I created a library of functions, the file structure for this project is the following:

### `.c` Files 
Where all of the functions will be written in. 

### `.h` (Header)
The header file is useful for 2 things:
- First, instead of doing for example `#include <unistd.h>` in all of `.c` files, you can just write it once in your header and all of your `.c` files will read it from your header file. 
- Secondly, let's say one of your `.c` files uses another function from another `.c` file, well instead of writting that function above, just write `#include "libft.h"` and it will find it in your header file.

### Makefile 
`Makefile` is the file I created to compile my projects.
- With a `Makefile`, you don't have compile your projects one by one or write a main function for them, you can just type `make` once you have created your Makefile.

</br>

## Functions

### Functions from `<ctype.h>`

- [`ft_isalnum`](ft_isalnum.c): Checks for an alphanumeric character.
- [`ft_isalpha`](ft_isalpha.c): Checks for an alphabetic character.
- [`ft_isascii`](ft_isascii.c): Checks whether c fits into the `ASCII` character set.
- [`ft_isdigit`](ft_isdigit.c): Checks for a digit (`0` through `9`).
- [`ft_isprint`](ft_isprint.c): Checks for any printable character.
- [`ft_tolower`](ft_tolower.c): Convert char to lowercase.
- [`ft_toupper`](ft_toupper.c): Convert char to uppercase.

### Functions from `<string.h>`

- [`ft_bzero`](ft_bzero.c): Write zeroes to a byte string.
- [`ft_memset`](ft_memset.c): Fill memory with a constant byte.
- [`ft_memcpy`](ft_memcpy.c): Copy memory area.
- [`ft_memmove`](ft_memmove.c): Copy byte string.
- [`ft_memchr`](ft_memchr.c): Scan memory for a character.
- [`ft_memcmp`](ft_memcmp.c): Compare memory areas.
- [`ft_strlen`](ft_strlen.c): Calculate the length of a string.
- [`ft_strlcpy`](ft_strlcpy.c): Copy string to an specific size.
- [`ft_strlcat`](ft_strlcat.c): Concatenate string to an specific size.
- [`ft_strchr`](ft_strchr.c): Locate character in string.
- [`ft_strrchr`](ft_strrchr.c): Locate character in string.
- [`ft_strncmp`](ft_strncmp.c): Compare two strings.
- [`ft_strnstr`](ft_strnstr.c): Locate a substring in a string.
- [`ft_strdup`](ft_strdup.c): Create a duplicate for the string passed as parameter.

### Functions from `<stdlib.h>`
- [`ft_atoi`](ft_atoi.c): Convert a string to an integer.
- [`ft_calloc`](ft_calloc.c): Allocate memory and set its bytes' values to `0`.

### Non-standard functions
- [`ft_substr`](ft_substr.c): Return a substring from a string.
- [`ft_strjoin`](ft_strjoin.c): Concatenate two strings.
- [`ft_strtrim`](ft_strtrim.c): Trim the beginning and end of string with specific set of chars.
- [`ft_split`](ft_split.c): Split a string using a char as parameter.
- [`ft_itoa`](ft_itoa.c): Convert a number into a string.
- [`ft_strmapi`](ft_strmapi.c): Apply a function to each character of a string.
- [`ft_striteri`](ft_striteri.c): Apply a function to each character of a string.
- [`ft_putchar_fd`](ft_putchar_fd.c): Write a char to a file descriptor.
- [`ft_putstr_fd`](ft_putstr_fd.c): Write a string to a file descriptor.
- [`ft_putendl_fd`](ft_putendl_fd.c): Write a string to a file descriptor, followed by a new line.
- [`ft_putnbr_fd`](ft_putnbr_fd.c): Write a number to a file descriptor.

### Linked-list functions

- [`ft_lstnew`](ft_lstnew_bonus.c): Create a new list element.
- [`ft_lstadd_front`](ft_lstadd_front_bonus.c): Add an element at the beginning of a list.
- [`ft_lstsize`](ft_lstsize_bonus.c): Count the number of elements in a list.
- [`ft_lstlast`](ft_lstlast_bonus.c): Return the last element of the list.
- [`ft_lstadd_back`](ft_lstadd_back_bonus.c): Add an element at the end of a list.
- [`ft_lstclear`](ft_lstclear_bonus.c): Delete and free list.
- [`ft_lstiter`](ft_lstiter_bonus.c): Apply a function to each element of a list.
- [`ft_lstmap`](ft_lstmap_bonus.c): Apply a function to each element of a list.