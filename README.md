_RabbitWerks Javascript 2020_

# **Flexbox-Util v1.4**

*A utility based Flexbox css class-helper library to help take the guess work out of flexbox.*

## **Getting Started**

This project is currently in the intermediate stages. To use, simply download the repo zip and copy out the flexbox-util.css file into the css folder of your project, then link to flexbox-util.css in your markup.  
Using this library is very straight forward and is intended to be explicit in class names for anyone not familiar with the library to understand as well.

### **First Steps**

Each parent element you want to apply flexbox to will get the `.flexbox` class. This defaults to a standard assignment of `display: flex` to the parent element, thus rendering itself as a flex container and any child elements inside as flex items.

Each child will assume its explicit widths/heights if set using css. If no explicit sizing is defined, the helper classes `.flex-1` `.flex-2` `.flex-3` etc.. will determine the flex-item sizes implicitly, by taking up that available space in accordance with the rest of the flex items sizes, and parent size.

These utility classes will work across any html elements.

Flexbox works on a ratio basis. This means that the flex items, if not explicitly sized, will take up the available space according to their ratio amount in conjunction with the other flex items.

---

#### Going Further

So you have flexbox displaying your flex items now, great! Lets take a little more control.
You can align your flex-items spacings automatically by using the `flexbox-space-*` classes. These classes will justify the content along the X axis of the flex-flow.  
  
---

### **CURRENT CLASS LIST**
  
**.flexbox** | Applies the rule `display: flex` to the target element. Can be used in parent and child elements, if nested, in sequential order.  
  
**.flexdir-row** | Applies the standard css rule of `flex-direction: row` to the target element and changes the flex direction to row (horizontal).  
  
**.flexdir-rowrev** | Applies the css rule `flex-direction: row-reverse` to the target element and changes the flex direction to row (horizontal), and reversed item display order.  
  
**.flexdir-col** | Applies the css rule `flex-direction: column` to the target element and changes the flex direction to column (vertical).  
  
**.flexdir-colrev** | Applies the css rule `flex-direction: column-reverse` to the target element and changes the flex-direction to column (vertical), and reversed item display order.  
  
**.flex-[1-20]** | Applies the css rule `flex` and the flex amount to the applied element.  
  
**.flexgap -[1-5]** | Applies a custom flexgap css rule group to the parent element of the target elements. Works in conjunction with `.flexbox` class.  

**.flex-center** | Sets the properites of the flex items inside a flex container to `justify-content: center` and `align-items: center`. (horizontally and vertically)

### **Order of Sequence**

_It is best practice to follow these conventions to ensure proper behavior from css rules._

- Parent containers of flex displays must have the `.flexbox` class on it, or a class that apllies flexbox with other properties.
- Children with inherit or auto widthd must have a `.flex-[1-15]` class for sizing. Default to .flex-1
- Nested flex displays must be applied after the current elements child-flex properties are applied.
- e.g. `class="... flex-1 flexbox"`
  - where `.flex-1` is the current element sizing and we are setting the contents inside it as `display: flex`.
- each element nested as a flex container can have an independant flew-flow from its parent by applying the `.flexdir-*` class after the `.flexbox`
  - e.g. `class="... flex-1 flexbox flexdir-col"`
  - where `.flexdir-col` is changing the nested flex containers flex direction to column (vertical)

## 