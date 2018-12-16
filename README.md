### RabbitWerks Javascript

# Flexbox-Util v1

##### *A utility based Flexbox css class-helper library to help take the guess work out of flexbox.*

### Getting Started:
This project is currently in the beginning stages. To use, simply download the repo zip and copy out the flexbox-util.css file into the css folder of your project, then link to flexbox-util.css in your markup.  
Using this library is very straight forward and intended to be explicit in class names for anyone not familiar with the library to understand as well.

#### First Steps:
Each parent you want to apply flexbox to will get the "flexbox" class. This defaults to a standard assignment of display: flex to the parent element, thus rendering the children inside the parent as flex items. 

Each child will assume is explicit widths/heights is set. The helper classes flex-1 flex-2 flex-3 etc.. will determine the flex-item sizes implicitly, by taking up that available space in accordance with the rest of the flex items sizes, and parent size.

THese utility classes will work across any html elements. 

### Going Further:

So you have flexbox displaying your flex items now, great! Lets take a little more control.
You can align your flex-items spacings automatically by using the flexbox-space-* classes. These classes will justify the content along the X axis of the flex-flow.
