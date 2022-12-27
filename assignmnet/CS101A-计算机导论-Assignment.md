# CS101A-计算机导论-Assignment 11

**Name：**杨家鉴

**SID：**12012711



##### Ex.1

C, D

##### Ex.2

D

##### Ex.3

C

##### Ex.4

B, C

##### Ex.5

When the object is passed by value, a new space will be opened in the stack and the value of the parameter will be assigned to the new object. The operation of the function on the object will not affect the value of the object outside the function.

The reference passing uses the reference of the object, that is, the address of the object in memory. The object can be modified directly in the function.

```c++

int main(){
    int a = 1;
	int b = 2;
    Swap(a,b);
}

//value passing
void Swap(int a, int b){
    int temp;
    temp = a;
    a = b;
    b = temp;
}
//reference pass
void Swap(int &a, int &b){
    int temp;
    temp = a;
    a = b;
    b = temp;
}
```

