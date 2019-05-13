<h1>Week Six </h1>
<h3>MVP : </h3>

<h4>Things that is going on in my head
What I was thinking: </h4>

<p>Since my topic is a little different and it's not like coding coding like an app for something. I think I am going to create a scene that incorporates each section that aframe school discusses and teaches about. 

What kind of scene do i want? 

Honestly I dont know yet, I think if I sit here and try to figure out what I want im never going to have a scene set up 

Im going to start with the basics and see what I come up with

Reminders I gave myself: </p>

REMEMBER AMANDA
Dont get stressed 
Dont compare your project to others / its really different than other topics
Start coding and see what you come up with 
Copying dont help 
Start with basics shapes and add things to it 



<h4>Where am I going to begin coding</h4>
Not gonna do it in c9 
Glitch is better to use I believe 

<h4> What I have to look into</h4>
Look into how aframe inspector will work because for github it has a website but when tried to download got lots of errors

Npm?

Scene:
Forrest 

What do i want/ basic
Background: 
Sky

What to create:
Trees 

 

Today i am creating the forrest or starting it 
	 I got the platform which is going to be the “grass” 
	And the background is going to be the sky 

 https://blog.mozvr.com/procedural-geometry-trees/ shows how they make a tree
```
<html>
  <head>
    <meta charset="utf-8">
    <title>Hello, WebVR! • A-Frame</title>
    <meta name="description" content="Hello, WebVR! • A-Frame">
    <script src="https://aframe.io/releases/0.9.0/aframe.min.js"></script>
  </head>
  <body>
    <a-scene background="color: #cceeff"></a-scene>
     <a-plane position="0 0 -4" rotation="-90 0 0" width="4" height="4" color="#267326"></a-plane>

```
Starting off code with ……
Correct way :
```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Hello, WebVR! • A-Frame</title>
    <meta name="description" content="Hello, WebVR! • A-Frame">
    <script src="https://aframe.io/releases/0.9.0/aframe.min.js"></script>
  </head>
  <body>
  <a-scene background="color: #cceeff">
     <a-plane position="0 0 -4" rotation="-90 0 0" width="4" height="4" color="#267326"></a-plane>
    </a-scene>
  </body>

```

Knowing the difference
<a-plane 
position="0 0 -4" - for the postiton the first number is left and right / second number is up and down / third number is diagnal wise 
 rotation="-90 0 0" 
width="4" height="4" 
color="#267326"></a-plane>




I built a tree with html 

Next step 
 Now with javascript - learn how to make a “class “ so that it is efficent and dont have to continue making the same code 
Example :
```
const group = new THREE.Group()
const level1 = new THREE.Mesh(
    new THREE.ConeGeometry(1.5,2,8),
    new THREE.MeshLambertMaterial({color:0x00ff00})
)
level1.position.y = 4
group.add(level1)
const level2 = new THREE.Mesh(
    new THREE.ConeGeometry(2,2,8),
    new THREE.MeshLambertMaterial({color:0x00ff00})
)
level2.position.y = 3
group.add(level2)
const level3 = new THREE.Mesh(
    new THREE.ConeGeometry(3,2,8),
    new THREE.MeshLambertMaterial({color:0x00ff00})
)
level3.position.y = 2
group.add(level3)
const trunk = new THREE.Mesh(
    new THREE.CylinderGeometry(0.5,0.5,2),
    new THREE.MeshLambertMaterial({color:0xbb6600})
)
trunk.position.y = 0
group.add(trunk)
return group

```

<h4> Links I referenced</h4>
https://threejs.org/docs/#api/en/geometries/CylinderBufferGeometry

https://threejs.org/docs/index.html#api/en/geometries/CircleGeometry
