# Entry 5
##### 4/8/24

## context
During this section of the year I have been learning how to create 3d models of a background/my cooking robot to try and invision my project. By using geometric shapes and codes I am able to achieve a few more steps towards my goal of the freedom project with Aframe 3d models. I tried to change some of the more basic shapes used but it was kind of hard since im not used to it. But i did try more on tinkering with positions and ideas of my project. I used the a-scene and created more shapes hoping to get used to it. 
````
<html>
  <head>
    <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
  </head>
  <body>
    <a-scene>
            <a-box position="-1.5 0.5 -5" color="#FFF"></a-box>
            <a-box position="-1 0.5 -5" color="#FFF"></a-box>
            <a-box position="-0.5 0.5 -5" color="#FFF"></a-box>
            <a-box position="0.5 0.5 -5" color="#FFF"></a-box>
            <a-box position="1 0.5 -5" color="#FFF"></a-box>
            <a-box position="1.5 0.5 -5" color="#FFF"></a-box>
            <a-box position="2 0.5 -5" color="#FFF"></a-box>
            <a-box position="2.5 0.5 -5" color="#FFF"></a-box>
            <a-box position="3 0.5 -5" color="#FFF"></a-box>
            <a-box position="3.5 0.5 -5" color="#FFF"></a-box>   
            <a-box position="4 0.5 -5" color="#FFF"></a-box>
            <a-box position="4.5 0.5 -5" color="#FFF"></a-box>
            <a-box position="5 0.5 -5" color="#FFF"></a-box>
            <a-box position="5 0.5 -5" color="#FFF"></a-box>
            <a-box position="-1.5 1.5 -5" color="#FFF"></a-box>
            <a-box position="-1 1.5 -5" color="#FFF"></a-box>
      
            <a-box position="1 3 -5" color="#FFF"></a-box>
            <a-box position="1.5 3 -5" color="#FFF"></a-box>
            <a-box position="2 3 -5" color="#FFF"></a-box>
      
      
      
      
      
      
      
    
      
      
      
      
      
      <a-plane position="0 0 -4" rotation="-90 0 0" width="4" height="4" color="#7BC8A4"></a-plane>
      <a-plane position="4 0 -4" rotation="-90 0 0" width="4" height="4" color="#7BC8A4"></a-plane>
      <a-sky color="#ECECEC"></a-sky>
    </a-scene>
  </body>
</html>
````
This is a code for the background model for the cooking robot to use and show what my project would be about. Some extra knowledge i learned was to add shadows to the shapes to add demention and make my model better looking.  
````<a-entity light="type:directional; castShadow:true;" position="1 1 1"></a-entity>
<a-gltf-model src="tree.gltf" shadow="receive: false"></a-gltf-model>
````

## Sources
[Aframe](https://aframe.io/docs/1.5.0/components/shadow.html) Website for shadows  
[shadow/light](https://aframe.io/docs/1.5.0/components/light.html#configuring-shadows) that goes in depth for the explanation.

## skills
1. First skill i learned is communicating with my peers on how to fix problems with my code even when it was identical to the website code. I realized that sometimes even if the code is the exact same it wont always work the same on every platform and asked for advice to which my peers suggested that i try researching my problem on [google](google.com) or [youtube](youtube.com) and it helped since many people seem to be having the same problem as well.
2. Second skill i learned in to be on the look out on slack because there are many students who need help with many things and sometimes one person asks a question that many have been struggling with but are too shy or scared to ask. I personally find this very convenient because I am also shy, but good thing majority of people are also doing Aframe so it makes things easier.



[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
