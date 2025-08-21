# Source code examples

``` py title="add_numbers.py" linenums="1" hl_lines="2-4"
# function to add 2 numbers
def add_two_numbers(num1, num2):
    return num1 + num2
result = add_two_numbers(5, 3)
print('The sum is:', result)
```

This is regular text added to explain the code in details

``` c title="add_numbers.cpp" linenums="1"
#include test.h
int num1 = 99;
int num2 = 100;
int result = num1 + num2;
cout << "\nresult is " << result << endl;
cout << "end of prog" << endl;
```

This is regular text added to explain the JAVA code below:
The input argument is check for its size if the size is 3 the execution of the 
program will continue. If not the program will quit.

``` java title="checkArgumentSize.java" linenums="1"
package BranchingApp;
public class branchingApp_test {
	public static void main(String[] args)
	{
		if (checkData(args[0]))
		{
			System.out.print("arguments oke, continue execution");
		}
		else
		{
			System.out.print("wrong argument size, exit execution");
			return;
		}
	}
		static boolean checkData(String tekst)
		{ if (tekst.length() == 3)
		{ return true; }
		else
		{ System.out.println("Fout! aantal tekens niet 3");
		return false;
		}
		}
	}
	
```
