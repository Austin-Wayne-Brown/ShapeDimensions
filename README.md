#
# ShapeDimensions

#
# Project Summary

This application creates two circles, two rectangles, and two triangles, all of which have their dimensions predetermined. Their x, y and z coordinates, along with their area, are then displayed to the user.

.

#
# Running the Program

To execute the program simply download the repository, compile the code, and run.

.

#
# Classes Documentation

ShapeDimensions contains 6 classes.

### **Class: Shape**

This abstract class gets the coordinates of the center of a shape, along with its area.

#### **Constructor**

public Shape(int x, int y, int z)

_Gets the center point of each shape&#39;s coordinates._

#### **Attributes**

| **Attribute** | **Description** |
| --- | --- |
| public abstract double area() | The area of the shape. |

### **Class: Point**

This class makes sure the x, y and z coordinates of each shape are each between 0 and 500, then returns each coordinate of the shape to the user.

#### **Constructor**

public Point(int x, int y, int z)

_Sets boundaries for each x, y and z coordinate to be between 0 and 500._

#### **Methods**

| **Returns** | **Method** |
| --- | --- |
| int | **getX** () |
|   | _Returns the value of the x coordinate._ |
| int | **getY** () |
|   | _Returns the value of the y coordinate._ |
| int | **getZ** () |
|   | _Returns the value of the z coordinate._ |
| String | **toString** () |
|   | _Return&#39;s the x, y, and z coordinates of the shape as a string._ |

### **Class: Circle**

A class that extends the Shape class; gets the x, y and z coordinates of the circle, then gets the circle&#39;s radius and uses it to calculate the shape&#39;s area.

#### **Constructors**

public Circle(int x, int y, int z, double r)

_Creates circle and gets the shape&#39;s x, y and z coordinates along with its radius_

#### **Methods**

| **Returns** | **Method** |
| --- | --- |
| double | **getRadius** () |
|   | _Returns the radius of the circle._ |
| double | **@Override**** area**() |
|   | _Calculates the area of the circle._ |
| String | **toString** () |
|   | _Returns the x, y and z coordinate, along with the circle&#39;s area, as a string._ |

### **Class: Triangle**

_A class that extends the Shape class; gets the x, y and z coordinates of the triangle, then gets the triangle&#39;s base and height and uses it to calculate the shape&#39;s area._

#### **Constructor**

public Triangle (int x, int y, int z, double b, double h)

_Creates triangle and gets the shape&#39;s x, y and z coordinates along with its base and height_

#### **Attributes**

| **Attribute** | **Description** |
| --- | --- |
| private double base | The base of the triangle. |
| private double height | The height of the triangle |

#### **Methods**

| **Returns** | **Method** |
| --- | --- |
| double | **getBase()** |
|   | _Returns the base of the triangle._ |
| double | **getHeight** () |
|   | _Returns the height of the triangle._ |
| double | **@Override**** area**() |
|   | _Calculates the area of the Triangle._ |
| String | **toString** () |
|   | _Returns the x, y and z coordinate, along with the triangle&#39;s area, as a string._ |

### **Class: Rectangle**

_A class that extends the Shape class; gets the x, y and z coordinates of the rectangle, then gets the rectangles length and width and uses it to calculate the shape&#39;s area._

#### **Constructor**

public Rectangle(int x, int y, int z, double l, double w)

_Creates rectangle and gets the shape&#39;s x, y and z coordinates along with its length and width_

#### **Attributes**

| **Attribute** | **Description** |
| --- | --- |
| private double length | The length of the rectangle |
| private double width | The width of the rectangle |

#### **Methods**

| **Returns** | **Method** |
| --- | --- |
| double | **getLength()** |
|   | _Returns the length of the rectangle._ |
| double | **getWidth** () |
|   | _Returns the width of the rectangle._ |
| double | **@Override**** area**() |
|   | _Calculates the area of the rectangle._ |
| String | **toString** () |
|   | _Returns the x, y and z coordinate, along with the rectangle&#39;s area, as a string._ |



### **Main**

This main class creates 2 of each shape type with their dimensions predetermined. Each shape is stored into an ArrayList, and the coordinates, along with the shape&#39;s area, are printed out as a string

#### **Methods**

| **Returns** | **Method** |
| --- | --- |
| void | **main** (String[] args) |
|   | _Creates the shapes, stores them in an ArrayList, then prints out each&#39;s coordinates and areas._ |
