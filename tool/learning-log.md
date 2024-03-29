# Tool Learning Log

Tool: **Aframe**

---

## LL2
### 3/10/24
## bootstrap grid-
````
<div class="container">
  <div class="row">
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
  </div>
</div>
````
## bootstrap component-
List group
````
<ul class="list-group">
  <li class="list-group-item">An item</li>
  <li class="list-group-item">A second item</li>
  <li class="list-group-item">A third item</li>
  <li class="list-group-item">A fourth item</li>
  <li class="list-group-item">And a fifth one</li>
</ul>
````
button
````
<button type="button" class="btn btn-primary">Primary</button>

````
spinner
````
<div class="spinner-border" role="status">
  <span class="visually-hidden">Loading...</span>
</div>
````
# LL3
## 3/17/24
## single property component
````
<!-- `position` is the name of the position component. -->
<!-- `1 2 3` is the data of the position component. -->
<a-entity position="1 2 3"></a-entity>
````
## multi-property component
````
<!-- `light` is the name of the light component. -->
<!-- The `type` property of the light is set to `point`. -->
<!-- The `color` property of the light is set to `crimson`. -->
<a-entity light="type: point; color: crimson"></a-entity>
````

## animation component-this lets us animate values
````
<a-box position="-1 1.6 -5" animation="property: position; to: 1 8 -10; dur: 2000; easing: linear; loop: true" color="tomato"></a-box>
````
## light
this shows the light values to make the shapes come alive
````
<a-entity light="color: #AFA; intensity: 1.5" position="-1 1 0"></a-entity>
````



<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->


# LL4
## 3/24/24

### Link:

https://www.youtube.com/watch?v=K4LEMBjaV9E&list=PL8MkBHej75fJD-HveDzm4xKrciC5VfYuV&index=6
https://aframe.io/docs/1.5.0/introduction/javascript-events-dom-apis.html


### About how the camera: 

````
<a-scene>
  <a-box></a-box>
  <a-camera></a-camera>
</a-scene>
````
````
<!-- Place camera at ground level (will be overridden by VR devices) -->
<a-camera position="0 0 0"></a-camera>
````

````
<a-entity id="rig" position="25 10 0">
  <a-camera id="camera"></a-camera>
</a-entity>
````


### shapes:
````
<a-entity geometry="primitive: box; width: 1; height: 1; depth: 1"></a-entity>
````
````
<a-entity geometry="primitive: circle; radius: 1" material="side: double"></a-entity>
````
````
<a-entity geometry="primitive: cone; radiusBottom: 1; radiusTop: 0.1"></a-entity>
````
````
<a-entity geometry="primitive: cylinder; height: 3; radius: 2"></a-entity>
````
````
<a-entity geometry="primitive: cylinder; openEnded: true" material="side: double"></a-entity>
````
````
<a-entity geometry="primitive: cylinder; openEnded: true; thetaLength: 180"
          material="side: double"></a-entity>
````
````
<a-entity geometry="primitive: dodecahedron; radius: 2"></a-entity>
````
````
<a-entity geometry="primitive: octahedron"></a-entity>
````
````
<a-entity geometry="primitive: icosahedron"></a-entity>
````
````
<a-entity geometry="primitive: plane; height: 10; width: 10" material="side: double"></a-entity>
````
````
<a-entity geometry="primitive: ring; radiusInner: 0.5; radiusOuter: 1"
          material="side: double"></a-entity>
````

### Adding text:

````
<html>
  <head>
    <meta charset="UTF-8">
    <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
  </head>
  <body>
    <a-scene>
      <a-sky color="lightblue"></a-sky>
      <a-text value="ABCあいうえお日本語" font="custom-msdf.json" font-image="custom-msdf.png" negate="false" scale="2 2 1" position="-2 2 -4"></a-text>
    </a-scene>
  </body>
</html>
````


### hand-controls:

````
<a-entity id="leftHand" hand-controls="hand: left; handModelStyle: lowPoly; color: #ffcccc"></a-entity>
<a-entity id="rightHand" hand-controls="hand: right; handModelStyle: lowPoly; color: #ffcccc"></a-entity>
````

### hand-tracking-controls:
````
<a-entity id="leftHand" hand-tracking-controls="hand: left;"></a-entity>
<a-entity id="rightHand" hand-tracking-controls="hand: right;"></a-entity>
````


### hand-tracking-grab-controls: 
````
<a-entity id="leftHand" hand-tracking-grab-controls="hand: left;"></a-entity>
<a-entity id="rightHand" hand-tracking-grab-controls="hand: right;"></a-entity>
````

#### Background

How to add sky:
````
<a-scene>
  <a-assets>
    <img id="sky" src="sky.png">
  </a-assets>
  <a-sky src="#sky"></a-sky>
</a-scene>
````


````
<a-sky color="#6EBAA7"></a-sky>
````

#### Reflection:
````
<a-scene reflection="directionalLight:a-light#dirlight;"></a-scene>
	<a-light id="dirlight" intensity="1" light="castShadow:true;type:directional" position="1 1 1"></a-light>
````



# LL5
## 3/29/24

### Link:

https://www.youtube.com/watch?v=K4LEMBjaV9E&list=PL8MkBHej75fJD-HveDzm4xKrciC5VfYuV&index=6
https://aframe.io/docs/1.5.0/introduction/javascript-events-dom-apis.html



#### Anchored
````
<a-entity id="myBox" anchored="persistent: true" geometry="primitive: box" material="color: red"></a-entity>
````

#### Position
It goes like x,y,z

x	Negative X axis extends left. Positive X Axis extends right.	0
y	Negative Y axis extends down. Positive Y Axis extends up.	0
z	Negative Z axis extends in. Positive Z Axis extends out.	0

````
<a-entity position="0 1 -1"></a-entity>
````
````
<a-entity id="parent" position="1 2 3">
  <a-entity id="child1"></a-entity>
  <a-entity id="child2" position="2 3 4"></a-entity>
</a-entity>
````

#### Scale

x	Scaling factor in the X direction.	1
y	Scaling factor in the Y direction.	1
z	Scaling factor in the Z direction.	1

````
<a-entity scale="0.5 1 2"></a-entity>
````


````
<a-entity geometry="primitive: sphere; radius: 1000"
          material="src: sky.png"
          scale="1 1 -1"></a-entity>
````

#### Shadow
````
<a-entity light="type:directional; castShadow:true;" position="1 1 1"></a-entity>
<a-gltf-model src="tree.gltf" shadow="receive: false"></a-gltf-model>
````

#### xr-mode-ui
````
<a-scene xr-mode-ui="enabled: false"></a-scene>
````

windows-motion-controls
````
<a-entity windows-motion-controls="hand: left"></a-entity>
<a-entity windows-motion-controls="hand: right"></a-entity>
````
