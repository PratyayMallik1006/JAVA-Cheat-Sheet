# JAVA Cheat Sheet

One glance JAVA Cheat Sheet


## Boilerplate
```java
class Main
{
        public static void main(String args[])
        {
              Scannner sc=new Scanner(System.in);
              int num=sc.nextInt();
              for(int i=0;i<num;i++){
	              System.out.println(num);
              }
              System.out.println("Hello World!");
        }
}
```





## Types
We use variables to temporarily store data in computer’s memory. In Java, the type of a variable should be specified at the time of declaration. In Java, we have two categories of types: 
- **Primitives:** for storing simple values like numbers, strings and booleans. 
- **Reference Types:** for storing complex objects like email messages.(Objects)

### Primitive Types
| # | Type | Bytes | Range |
|---| ----- | -------- | ---------- |
|1|byte |1 |[-128,127]
|2|short |2 |[-32k,32k]
|3|int |4 |[-2B,2B]
|4|long |8 |
|5|float |4 |
|6|double |8 |
|7|char |2 |A,B,C, ...
|8|boolean |1 |true/false
```java
class Main
{
        public static void main(String args[])
        {
              byte age = 30; 
              long viewsCount = 3_123_456L; 
              float price = 10.99F; 
              char letter = ‘A’; 
              boolean isEligible = true;
              System.out.println("Hello World!");
        }
}
```



### Reference Types

- Variables other than the above 8 Primitive Types.
- Objects
```java
class Main
{
        public static void main(String args[])
        {
              Object obj = new Object();
              Scanner sc = new Scanner(System.in);
              String name = “Pratyay”;
              //Internally: String name = new String("Pratyay");
        }
}
```

## Strings
```java
String name = “Pratyay”;
```
**Useful String Methods:**
The String class in Java provides a number of useful methods:
-  startsWith(“a”)
-  endsWith(“a”)
-  length()
-  indexOf(“a”)
-  replace(“a”, “b”)
-  toUpperCase()
-  toLowerCase()
```java
class Main
{
        public static void main(String args[])
        {
              String s1="Hello World!";
              System.out.println("string length is: "+s1.length());
        }
}
```
Strings are immutable, which means once we initialize them, their value cannot be
changed. All methods that modify a string (like toUpperCase) return a new string
object. The original string remains unaffected. 

**Escape Sequences:** 
If you need to use a backslash or a double quotation mark in a string, you need to prefix it with a backslash. This is called escaping.
Common escape sequences: 
- \\ 
-  \” 
-  \n (new line) 
-  \t (tab)
