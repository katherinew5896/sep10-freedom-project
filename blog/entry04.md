# Entry 4
##### 2/12/24

## Context
This step was about choosing what tools we wanted to use and i decided to use AFrame. Aframe is a framework for building most VR(virual reality) which includes 3d models of items or people. I found some resources to help me in this project with the [aframe](https://aframe.io/) website. Another website i used was [youtube](https://www.youtube.com/watch?v=ktjMCanKNLk&list=PL8MkBHej75fJD-HveDzm4xKrciC5VfYuV) where there was a whole playlist about aframe and its use.

## Basics 
There are many shapes you could add like boxes, cylinders, squares, and circles.  
**Box** `<a-entity geometry="primitive: box; width: 1; height: 1; depth: 1"></a-entity>`  

**circle** `<a-entity geometry="primitive: circle; radius: 1" material="side: double"></a-entity>`  

**cylinder** `<a-entity geometry="primitive: cylinder; height: 3; radius: 2"></a-entity>`  

**More Tinkering**
````
<html>
  <head>
    <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
  </head>
  <body>
    <a-scene>
      <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9"></a-box>
      <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E"></a-sphere>
      <a-cylinder position="1 0.75 -3" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-plane position="0 0 -4" rotation="-90 0 0" width="4" height="4" color="#7BC8A4"></a-plane>
      <a-sky color="#ECECEC"></a-sky>
    </a-scene>
  </body>
</html>
````
From this code i've learned to code and changing the property of shapes by using radius, height, color, and width. Also from previous projects we've learned how to do positioning and rotation.


## How to add aframe into your HTML
To add aframe into HTML you can implant this code from the aframe website to your HTML to start using aframe.  
````
<html>
  <head>
    <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
  </head>
  <body>
    <a-scene>
    </a-scene>
  </body>
</html>
````
## EDP
Currently on my forth step i am starting to plan out my project and how to incorporate aframe in my project. I am planning on making a 3d model with aframe with its geometry codes and creating a robot out of it for my project. 





[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
