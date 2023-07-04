# How to Learn Pointers in C with Yashavant Kanetkar's Book
 
Pointers are one of the most powerful and challenging features of the C programming language. They allow programmers to manipulate memory directly and efficiently, but they also introduce many potential errors and complexities. Learning pointers can be daunting for beginners and even experienced programmers.
 
Fortunately, there is a book that can help you master pointers in C: *Understanding Pointers in C* by Yashavant Kanetkar. This book is a comprehensive guide to pointers, covering everything from the basics to advanced topics such as dynamic memory allocation, linked lists, trees, graphs, and more. The book also provides many fully working examples and applications of pointers that illustrate their practical use.
 
**Download ⚙⚙⚙ [https://sormindpestna.blogspot.com/?download=2uEkaM](https://sormindpestna.blogspot.com/?download=2uEkaM)**


 
The book is available as a PDF file that you can download for free from various websites[^1^] [^2^] [^3^]. However, you should be aware that the PDF file may not be the latest edition of the book, and it may contain some errors or outdated information. The latest edition of the book is the third edition, published in 2020 by BPB Publications[^2^]. You can also buy a physical copy of the book from online stores such as Amazon[^1^].
 
If you want to learn pointers in C, you should definitely check out *Understanding Pointers in C* by Yashavant Kanetkar. It is one of the best books on pointers in C, written by an experienced and renowned author who has taught millions of programmers through his books and video courses. With this book, you will be able to unlock the full potential of pointers and write better C programs.
  
## How to Use Pointers in C
 
Now that you have learned how to declare and initialize pointers in C, you may wonder how to use them in your programs. Pointers can be used for various purposes, such as:
 
- Accessing and modifying the value of a variable through its address
- Passing arguments to functions by reference
- Returning multiple values from functions
- Creating and manipulating dynamic data structures such as arrays, linked lists, trees, graphs, etc.
- Implementing function pointers and callbacks

In this section, we will see some examples of using pointers in C for each of these purposes.
  
### Accessing and Modifying the Value of a Variable through its Address
 
One of the simplest uses of pointers is to access and modify the value of a variable through its address. For example, suppose we have a variable `x` that stores an integer value. We can declare a pointer `p` that points to `x` using `p = &x;`. Then, we can use `*p` to access and modify the value of `x`. For example:

    #include <stdio.h>
    
    int main() 
      int x = 10; // declare and initialize an integer variable
      int* p; // declare a pointer
      p = &x; // assign the address of x to p
      printf("x = %d\n", x); // print the value of x
      printf("*p = %d\n", *p); // print the value pointed by p
      *p = 20; // modify the value pointed by p
      printf("x = %d\n", x); // print the new value of x
      printf("*p = %d\n", *p); // print the new value pointed by p
      return 0;

The output of this program is:
 
pointer in c by yashwant kanetkar pdf download,  pointer in c by yashwant kanetkar ebook,  pointer in c by yashwant kanetkar google books,  pointer in c by yashwant kanetkar third edition pdf,  pointer in c by yashwant kanetkar solutions,  pointer in c by yashwant kanetkar online reading,  pointer in c by yashwant kanetkar book review,  pointer in c by yashwant kanetkar amazon,  pointer in c by yashwant kanetkar flipkart,  pointer in c by yashwant kanetkar price,  pointer in c by yashwant kanetkar pdf room,  pointer in c by yashwant kanetkar bpb publications,  pointer in c by yashwant kanetkar applications of pointers,  pointer in c by yashwant kanetkar pointers and arrays,  pointer in c by yashwant kanetkar pointers and strings,  pointer in c by yashwant kanetkar pointers and structures,  pointer in c by yashwant kanetkar pointers and data structures,  pointer in c by yashwant kanetkar pointers miscellany,  pointer in c by yashwant kanetkar pointers and functions,  pointer in c by yashwant kanetkar pointers and variable arguments,  pointer in c by yashwant kanetkar pointers and command-line arguments,  pointer in c by yashwant kanetkar pointers and linked lists,  pointer in c by yashwant kanetkar pointers and stacks & queues,  pointer in c by yashwant kanetkar pointers and trees & graphs,  pointer in c by yashwant kanetkar practical use of pointers,  pointer in c by yashwant kanetkar pointers in c++,  pointer in c by yashwant kanetkar introduction to pointers,  pointer in c by yashwant kanetkar dynamic memory allocation,  pointer in c by yashwant kanetkar file pointers,  pointer in c by yashwant kanetkar typedef with function pointers,  pointer in c by yashwant kanetkar argc and argv arguments to main(),  pointer in c by yashwant kanetkar near, far and huge pointers,  pointer in c by yashwant kanetkar physical address to segment:offset conversion,  pointer in c by yashwant kanetkar exploiting the bits,  pointer in c by yashwant kanetkar dictionary using pointers,  pointer in c by yashwant kanetkar managing database using pointers,  pointer in c by yashwant kanetkar keyboard queue using pointers,  pointer in c by yashwant kanetkar infix to postfix conversion using pointers,  pointer in c by yashwant kanetkar evaluation of postfix expression using pointers,  pointer in c by yashwant kanetkar locating duplicate filenames using pointers,  pointer in c by yashwant kanetkar hashing using pointers,  pointer in c by yashwant kanetkar function calls and stack using pointers,  understanding pointers in c pdf free download 29th edition ,  understanding pointers in c pdf free download 29th chapter ,  understanding pointers in c pdf free download 29th page ,  understanding pointers in c pdf free download 29th exercise ,  understanding pointers in c pdf free download 29th solution ,  understanding pointers in c pdf free download 29th problem

    x = 10
    *p = 10
    x = 20
    *p = 20

As you can see, changing the value pointed by `p` also changes the value of `x`, since they share the same memory location.
  
### Passing Arguments to Functions by Reference
 
Another common use of pointers is to pass arguments to functions by reference. This means that instead of passing a copy of the argument's value, we pass its address. This allows us to modify the original argument inside the function. For example, suppose we want to write a function that swaps two integers. We can use pointers to pass the addresses of the integers and swap their values inside the function. For example:

    #include <stdio.h>
    
    // function prototype
    void swap(int* a, int* b);
    
    int main() 
      int x = 10; // declare and initialize two integers
      int y = 20;
      printf("Before swap: x = %d, y = %d\n", x, y); // print their values before swap
      swap(&x, &y); // call swap function with their addresses
      printf("After swap: x = %d, y = %d\n", x, y); // print their values after swap
      return 0;

    // function definition
    void swap(int* a, int* b) 
      int temp; // declare a temporary variable
      temp = *a; // store the value pointed by a in temp
      *a = *b; // assign the value pointed by b to the location pointed by a
      *b = temp; // assign the value stored in temp to the location pointed by b

The output of this program is:

    Before swap: x = 10, y = 20
    After swap: x = 20, y = 10

As you can see, swapping the values pointed by `a` and `b` inside the function also swaps the values of `x` and `y`, since they share the same memory locations.
 8cf37b1e13
 
