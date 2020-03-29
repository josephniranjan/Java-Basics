* We can assign value of reference variable to another reference variable.
* Reference Variable is used to store the address of the variable.
* Assigning Reference will not create distinct copies of Objects.
* All reference variables are referring to same Object.

 **Assigning Object Reference Variables** does not –
* Create Distinct Objects.
* Allocate Memory
* Create duplicate Copy
* Consider This Example –

Rectangle r1 = new Rectangle();

Rectangle r2 = r1;
r1 is reference variable which contain the address of Actual Rectangle Object.
r2 is another reference variable
r2 is initialized with r1 means – “r1 and r2” both are referring same object , thus it does not create duplicate object , nor does it allocate extra memory.

![Assigning-Object-Reference-Variables](https://user-images.githubusercontent.com/46956514/77846911-f5437400-71d6-11ea-8c26-972539a22f5a.gif)

**Live Example : Assigning Object Reference Variables**
class Rectangle {
  double length;
  double breadth;
}

class RectangleDemo {
  public static void main(String args[]) {

  Rectangle r1 = new Rectangle();
  
  Rectangle r2 = r1;

  r1.length = 10;
  
  r2.length = 20;

  System.out.println("Value of R1's Length : " + r1.length); 
  
  System.out.println("Value of R2's Length : " + r2.length);

  }
}
**Output :**
java>java RectangleDemo

Value of R1's Length : 20.0

Value of R2's Length : 20.0

There are generally **four** different ways to make an **Object eligible for garbage collection**.
* Nullifying the reference variable
* Re-assigning the reference variable
* Object created inside method
* Island of Isolation

![memory-jvm](https://user-images.githubusercontent.com/46956514/77846404-700a9000-71d3-11ea-8012-904aea927044.png)
