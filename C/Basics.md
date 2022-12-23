## Pointers

```c
//Array of 5 integer pointers
int *ptr[5]
```


**You can have negative indexes for pointers**
```c 
char q[3]={'A','B','C'};
char *v=q;
v++;
v[-1] // IS VALID AND RETURNS 'A'
```

## Datatypes
[[ASCII]]
```c
char a = 'A'; // 65
char b = 'B'; // 66
a - b // -1
```

### Strings
```c
strcpy(s1, s2);
//Copies string s2 into string s1.

strcat(s1, s2);
//Concatenates string s2 onto the end of string s1.

strcmp(s1, s2);
//Returns 0 if s1 and s2 are the same; less than 0 if s1<s2; greater than 0 if s1>s2.
```
## Structures

#### Definition
```c
struct x
{
	int a;
	int b;
};
struct x first = {1,4};
//OR
first.a = 1;
first.b = 4;
```

#### Accessing

**Wrong**
```c
void change(struct x temp){
	temp.a = 0
} 
change(first)
 ```

**Correct**
 ```c
// Original structure changes
void newChange(struct x *temp){
	temp->a = 0
} 
newChange(&first) 
 ```

#### Misc
```c
struct test
{
char *name;
} a = {"Hello"};

struct test *cp = &a;
cp->name+1;

// returns 'ello'
// name is itself a pointer
```

## Precedence
- Prefix ++ and * have the same precedence (right to left)
- Postfix ++ is higher than both (left to right)
```c
// These are equal
*++p  >  *(++p)
++*p  >  ++(*p)
*p++  >  *(p++)
```
if p++ assign first then ++
## Infix, Postfix, Infix

**Infix to Postfix**
1. If same operator don't push
2.  If same priority don't push
3. Highest priority cannot be added if there is a lower priority operator
4. Pop operator in brackets

## Queue
```c
struct queue
{
	{3,2,1,5}
	int items[MAXQUEUE];
	int front, rear;
};
```
- Rear is the index of the rear item
- Front will be the index just before the front item
	If front == MAXQUEUE -1, front item is at items[0]

## Stack
```c
struct stack
{
	int items[100];
	int top;
};

void pop(struct stack *ptr){
	printf("%d", ptr->items[ptr->top--]); // in 1 line
	//OR
	printf("%d", ptr->items[ptr->top])
	ptr->top--;
}
```
- When empty top = -1
- Stack Underflow :   top < -1
- Stack Overflow   :   top > 100

## Binary Search Tree
Higher on right
Lower on left

                 Action Print Action
In-order      : Left Root Right
Pre-order    : Root Left Right
Post-order  : Left Right Root

![[Pasted image 20221130165906.png|500]]
