## Basic Program

```java
import java.util.*;

public class Main(){
	public static void main(String[] args){
		System.out.print("Hello World");
	}
}
```

## Overloading methods
Define methods with the same name but different signature  <em>(parameters / return value)</em>
Java will pick the most appropriate method for the given parameters
If the compiler cannot decide it is a *ambigious invocation* error

---
# Arrays

#### Declaration
```java
int numbers[] = new int[5];
numbers.length; // 5
```

- Default array values are: ` 0, \u0000, false, null `

#### Manipulation

##### Printing
```java
for(int i = 0, i < numbers.length, i++){
	System.out.println(numbers[i]);
}

int[] x = { 2, 4, 5, 6 };
        for (int item : x) {
            System.out.println(item);
        }

// ALTERNATIVELY

import java.util.Arrays
System.out.println(Arrays.toString(numbers));
```

- To copy an array make a loop and assign each value to the new array

##### Useful methods
```java
// from java.util.Arrays
Arrays.binarySearch(list, n);
Arrays.equals(l1,l2);
Arrays.fill(0, 5, 1) // Fill with 1 from i=0 to 4

// from java.lang.System
System.arraycopy(l1, 0, l2, 0, l1.length) 
```


#### Casting
`int a = 'a'`  
`char b = 98`  
`Integer.parseInt(String)`  
`Character.parseChar(String)`  




