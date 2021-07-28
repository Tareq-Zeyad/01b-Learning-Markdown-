# **CSS Transforms, Transitions, and Animations**.
<>
## **Transforms**
<>
### The transform property is presenting new features to CSS3 styling techniques to handle the styling in a better way.
### The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.
## **Transform Syntax**
### The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.
### *example div { -webkit-transform: scale(1.5); }*
<>
## **2D Transforms**
### Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis (depth or height).
### **2D Rotate**
### The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise.
### *example: .selector { transform: rotate(20deg); }*
### *2D Scale*
### Control the appearing size of an element of values between 0.99-.01.
### *example: .selector { transform: scale(.75);}*
### **2D Translate**
### he translate value works a bit like that of relative positioning, pushing and pulling an element in different directions (horizontal or vertical axis).
### **2D Skew**
### distort elements on the horizontal axis, vertical axis, or both.