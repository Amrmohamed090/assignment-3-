# usage of const keyword:
1-creating a variable that cannot be modified:

 if any variable is made as constant, using const keyword, you cannot change its value. Also, the constant variables must be initialized while they are declared.

 example
 (
	const int x = 10;
	x= 5;    //compile erorr
	x++;    //compile error
 )

2- Pointers with const keyword:

 Pointers can be declared using const keyword . 
 When we use const with pointers, we can do it in two ways, either we can apply const to what the pointer is pointing to, or we can make the pointer itself a constant.

 example
 (
	const int* x;     //the pointer is pointing to a const variable.
	int const* y;    //another way of declaration
 ) 

3-const Pointer:

 To make the pointer a constant, we have to put the const keyword to the right of the *. 
 The constant pointer to a variable is useful where you want a storage that can be changed in value but not moved in memory. 
 Because the pointer will always point to the same memory location
  
 example:
  (
	  int x = 1;
	  int* const w = &x;     // the pointer itself is a constant so it cannot be changed
  )

4-const Function Arguments and Return types
 
 We can make the return type or arguments of a function as const. Then we cannot change any of them.

 example:
 
	void f(const int i)
 {
    i++;    // compile error
 }

  const int g()
 {
     return 1;
  }
 
5-Defining Class Data members as const:
	
 These are data variables in class which are defined using const keyword. 
 They are not initialized during declaration. Their initialization is done in the constructor.

	example:

	 class Test
	 {
      const int i;
      public:
      Test(int x):i(x)
      {
          cout << "\ni value set: " << i;
      }
	 };

	 int main()
 	 {
      Test t(10);
      Test s(20);
	 }

6-Defining Class Object as const:
	
	When an object is declared or created using the const keyword, its data members can never be changed, during the object's lifetime.

	example
	(
		const class_name object;
	)

	

## usage of & (address operator) keyword:
 
The address operator is working for returns the memory address of a variable. 


examples of the usage of & operator:

1-Printing Variable Addresses:

 example:
 (
	 int x = 3;
	 cout << "Address of x in the memory is: "<< &x << endl; 
 )
	

2-Assigning Addresses to Pointers:
 
 example:
 (
	 int* pointVar, var;
     var = 5;

     // assign address of var to pointVar pointer
     pointVar = &var;
 )

