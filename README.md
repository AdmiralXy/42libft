# Libft

This project aims to create a C library that rewrites the standard libc functions while preserving their behavior and prototypes, as well as adding some of its own.

All functions are created in accordance with [Norm](https://github.com/42School/norminette) - the bunch of rules how code should be formatted.

| Prototype | Description |
| --------- | ----------- |
| int ft_abs(int value) | Compute the absolute value of an integer. |
| int ft_atoi(const char \*str) | Convert a string to an integer. |
| void ft_bzero(void \*s, size_t n) | Write zero-valued bytes. |
| void \*ft_calloc(size_t count, size_t size) | Allocates memory for an array of count elements of size bytes. |
| int ft_isalnum(int c) | Checks for an alphanumeric character. |
| int ft_isalpha(int c) | Checks for an alphabetic character. |
| int ft_isascii(int c) | Checks whether c is a 7-bit unsigned char value that fits into the ASCII character set. |
| int ft_isdigit(int c) | Checks for a digit. |
| int ft_isprint(int c) | Checks for any printable character including space. |
| char *ft_itoa(int n) | Converts an integer value to a null-terminated string. |
| void ft_lstadd_back(t_list \*\*lst, t_list \*new) | Adds the element ’new’ at the end of the list. |
| void ft_lstadd_front(t_list \*\*lst, t_list \*new) | Adds the element ’new’ at the beginning of the list. |
| void ft_lstclear(t_list \*\*lst, void (\*del)(void\*)) | Deletes and frees the given element and every successor of that element, using the function ’del’. |
| void ft_lstdelone(t_list \*lst, void (\*del)(void\*)) | Frees the memory of the element’s content using the function ’del’ and free the element. |
| void ft_lstiter(t_list \*lst, void (\*f)(void \*)) | Iterates the list ’lst’ and applies the function ’f’ to the content of each element. |
| t_list \*ft_lstlast(t_list \*lst) | Returns the last element of the list. |
| t_list \*ft_lstmap(t_list \*lst, void \*(\*f)(void \*), void (\*del)(void \*)) | Iterates the list ’lst’ and applies the function ’f’ to the content of each element. Creates a new list. |
| t_list \*ft_lstnew(void \*content) | Allocates (with malloc(3)) and returns a new element. |
| int ft_lstsize(t_list \*lst) | Counts the number of elements in a list. |
| void \*ft_memccpy(void \*dst, const void \*src, int c, size_t n) | Copies no more than n bytes in memory area. |
| void \*ft_memchr(const void \*s, int c, size_t n) | Scan the first n bytes of memory for a character. |
| int ft_memcmp(const void \*s1, const void \*s2, size_t n) | Compare memory areas. |
| void *ft_memcpy(void *dst, const void *src, size_t n) | Copy memory area. |
| void \*ft_memmove(void \*dst, const void \*src, size_t len) | Copy memory area, can handle overlapping memory. |
| void \*ft_memset(void \*b, int c, size_t len) | Fill memory with a constant byte. |
| int ft_nbrcmp(const int n1, const int n2) | Compare two integers. |
| void ft_putchar_fd(char c, int fd) | Output character to a specific file descriptor. |
| void ft_putendl_fd(char \*s, int fd) | Output line with \n to a specific file descriptor. |
| void ft_putnbr_fd(int n, int fd) | Output integer to a specific file descriptor. |
| void ft_putstr_fd(char \*s, int fd) | Output line to a specific file descriptor. |
| char \*\*ft_split(char const \*s, char c) | Split a string into pieces by 'c' character. |
| void ft_str_replace(char \*\*str, const char \*rep, const char \*in, int start) | Replaces first line ’rep’ into line ’str’ by inserting line ’in’, starting from index ’start’. The function reallocates memory. |
| char \*ft_strchr(const char \*s, int c) | Locate character in string. |
| int ft_strcmp(const char \*s1, const char \*s2) | Compare two strings. |
| void ft_strcpy(char \*dst, const char \*src) | Copy a string. |
| char \*ft_strdup(const char \*s1) | Duplicate a string. |
| void ft_striclear(char \*str, int index) | Shifts the string removes character by index. |
| void ft_strpclear(char \*str, char \*address) | Shifts the string removes character by address. |
| char \*ft_strjoin(char const \*s1, char const \*s2) | Concatenate the strings, the function allocates new memory. |
| size_t ft_strlcat(char \*dst, const char \*src, size_t dstsize) | Size-bounded string copying and concatenation. |
| size_t ft_strlcpy(char \*dst, const char \*src, size_t dstsize) | Copies up to size - 1 characters from the NUL-terminated string src to dst , NUL-terminating the result. |
| size_t ft_strlen(const char \*s) | Get string length. |
| char \*ft_strmapi(char const \*s, char (\*f)(unsigned int, char)) | Applies the function ’f’ to each character of the string ’s’ , and passing its index as first argument to create a new string (with malloc(3)) resulting from successive applications of ’f’. |
| int ft_strncmp(const char \*s1, const char \*s2, size_t n) | Compare part of two strings. |
| char \*ft_strnstr(const char \*haystack, const char \*needle, size_t len) | Locate a substring in a string. |
| char \*\*ft_strs_push_back(char \*\*strs, const char \*str) | Create a new array of strings including ’str’ at the end. |
| char \*\*ft_strs_push_front(char \*\*strs, const char \*str) | Create a new array of strings including ’str’ at the beginning. |
| char \*\*ft_strscopy(char \*\*strs) | Create a new array of strings from existing one. |
| char \*\*ft_strscreate(char \*str) | Create a new array of strings including ’str’ and NULL-terminator. |
| int ft_strsfind(char \*\*strs, const char \*str) | Find a string in an array of strings. |
| void ft_strsfree(char \*\*strs) | Clear array of strings. |
| char \*\*ft_strsjoin(char \*\*strs1, char \*\*strs2) | Concatenate two arrays of strings. |
| int ft_strslen(char \*\*strs) | Count the number of elements in an array of strings. |
| void ft_strssort(char \*\*strs) | Sorts the array of strings using the ft_strcmp() function for comparison. |
| char \*ft_strtrim(char const \*s1, char const \*set) | Removes all whitespace characters from the beginning and the end of a string. |
| char \*ft_substr(char const \*s, unsigned int start, size_t len) | Returns the substring of the given string at the given start position with the given length. |
| int ft_tolower(int c) | Transliterate uppercase characters to lowercase. |
| int ft_toupper(int c) | Transliterate lowercase characters to uppercase. |
| int ft_wdcounter(const char \*str, char separator) | Counts the number of words in a line through a separator. |
| int get_next_line(int fd, char **line) | Read a line from a file descriptor. |