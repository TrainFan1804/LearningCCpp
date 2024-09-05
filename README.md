This repo contains some stuff I wrote in C and C++ to learn those language a bit.
Nothing in here is really usefull.

# Pointer 

``` c
int value = 42;    // set the variable "value" to 42.
int* pointer;    // create a pointer that point to no specific address.
pointer = &value;    // create a pointer that point to the address of the variable "value".
```

``` c
int arr[5];    // create a array with the lenght of 5. Each value is written after another in memory.
```
CAUTION:If you declare an array like this the values aren't set to a specifc value so at the addresses are old memory values saved!

To avoid this you can also declare an array like this:

``` c
int arr[] = {42, 69, 1337};
```

# Arrays

Arrays can be declared like this:

``` c
int arr[SIZE];    // create an array with the entered SIZE.
```

A array is just a pointer that is pointing to the first element of the array (index 0).
Becaus of that you can write:

``` c
int arr[10];
arr[3];    // get the value of the 3 index.
```

or

``` c
int arr[10];
*(arr + 3);    // get also the value of the 3 index.
```

Both lines are the same.
