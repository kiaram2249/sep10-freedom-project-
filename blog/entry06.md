# My Tool A-frame
##### 4/14/2024

### What did I learned about my tool:

While tinkering with **A-frame** I learned a lot of things and a lot new different **HTML** codes. I also learnt **SASS**, and **Animation** since some of the videos that I watched inclueded it. Besides just tinkering I also went to different websites like the **A-frame website** or **A-frame school**. I was looking into those websites because I wanted to gain a better understanding of A-frame and to see if I can learn how to do certain things. Which I did, I learnt many things about my tool. For instance, I learnt the **Component Method**, how to change color by using **programmatic animation**, setting the **posittion**, giving the sphere **context**, and setting **texture** to my 3D objects. As well what is a **entity**, what is a **component**, **system**, and **architecture**. 

#### What I learnt: 

Example in how to write down an **Entity**:
```
<a-entity component1="property1:value; property2:value;"><a-entity> 
```
```
<a-entity geometry="primitive:box" material="color:red" position="-1 0.5 -3"></a-entity>
```

Component Method
```
<a-entity id="lightSphere" geometry="primitive=sphere" material="color:white; shader: flat" light="type:point" position="-4 3 -10"></a-entity>
```

Animation when using **A-frame**
```
<html>
  <body>
    <a-scene>
      <a-box color="pink"
             position="0 0.5 0">
             <a-animation attribute="rotation"
                          to="0 360 0"
                          repeat="indefinite"
                          dur="1000">
             </a-animation>
      </a-box>
    </a-scene>
  </body>
</html>
```

### How I learned my tool:

I learnt my tool by going to **YouTUbe** and by going to two different **A-frame website**. However, I mostly learnt how to use my tool by watching many **YouTube** videos because in those videos the people talk about _What is A-frame?_, _How to use A-frame_, and the _Different ways in using A-frame_. They really did broke things down one by one and they show you how to write down the code. So, it's easy to follow alone with them and code the same thing with them. These videos also provide the sources that they used and when to go in order to find these learning sources. 

#### The Sources in where I learnt my tool:

* [A-frame](https://aframe.io/docs/1.5.0/introduction/)
* [Easily code a virtual reality web experience with A-Frame (WebVR)](https://www.youtube.com/watch?v=jhEfT9YjLcU&t=576s)
* [Youtude A-frame](https://www.youtube.com/watch?v=qB8Ejh_QdpE&list=PLP3KjR1TMw7ekqC4o5gy0rR4odw7Jga84&index=4)
* [Youtude A-frame](https://www.youtube.com/watch?v=rl104MfKbW8&list=PLP3KjR1TMw7ekqC4o5gy0rR4odw7Jga84&index=6)
* [Aframe school](https://aframe.io/aframe-school/)
* [Animating Objects (A-Frame Tutorial - WebVR)](https://www.youtube.com/watch?v=p3mNNZ356Ko&list=WL&index=3&t=477s)

### What did I try/change/make? 

Over these times in me learning about my tool **A-frame**. _I try/change/make_ many things and in many ways. For instance, I try changing the shapes **posittion**, **width**, **color**, **adding new shapes** and **hight**. Another thing that I try to do was **animation** because in one of my sources I watched a video in where the guy was using **animation**. I try doing that when I was tinkering because animation seem very cool when you know how to use it. However I did make something by using **A-frame** and by using **animation** as well by following a video that one of my friends provided me with. Making that code required to use **SASS**. So, I guess I try using **SASS** as well when I was learning about my tool. 

The code:
```
<html>
  <head>
    <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
  </head>
  <body>
    <a-scene>
      <a-cone position="0.4 0.4 -0.6" rotation="0 22 0" color="lightgreen"></a-cone>
      <a-box position="1 0.5 -1.7" rotation="0 33 0" color="brown"></a-box>
      <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9"></a-box>
      <a-sphere position="0 1.25 -5" radius="1.25" color="pink"></a-sphere>
      <a-cylinder position="1 0.75 -3" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-plane position="0 0 -4" rotation="-90 0 0" width="4" height="4" color="#7BC8A4"></a-plane>
      <a-sky color="#ECECEC"></a-sky>
    </a-scene>
  </body>
</html>
```
The code:
```
<script
src="https://cdnjs.cloudflare.com/ajax/libs/aframe/0.5.0/aframe.js">
</script>

<a-scene>
<a-sphere></a-sphere>
<a-plane
src="https://media.giphy.com/media/oYtVHSxngR3lC/giphy.gif"
width="10" height="10" position="0 0 -2.5" color="black"></a-plane>
</a-scene>

<script src="index.js"></script>
```
```
$ = (queryString) => document.querySelector(queryString);

const shiftHue = (hue) => (hue + 1) % 360;

let hue = 0;

const animate = () => {
    hue = shiftHue(hue);
    const color = `hsl(${hue}, 100%, 50%)`;
    $(`a-sphere`).setAttribute('color', color);

    const variation = Math.sin(Date.now() / 1000);

    const position = `0 ${1.5 + variation} -2`;
    $('a-sphere').setAttribute('position', position);

    $('a-sphere').setAttribute('rotation', `-90 0`)
    $('a-plane').setAttribute('color', color);

    requestAnimationFrame(animate);
};

requestAnimationFrame(animate);
```

### Engineering Design Process

The last blog that I did I was in the process of **Brainstroming** (step 3). To be honest I'm still in the **brainstorming** stage because I have to start brainstorming in how I want my website to look like and how I want it to look like in a moblie size srceen, a table size screen, or a computer size screen. However, I'm also in the process of **plan** and **create** (steps 4 & 5) because since everyone learnt _how to use their tool_, _how to use a temple_, and _how to use wireframe_ we can all now get started in making our **website** / **Freedom Project**. So, since we are now in the stage in **planing** and **creating**, I need to start planing in what I want to do first step by step and I have to start creating it so that I can see the results. 

### Skills

#### Collaboration

I gained the skill of **Collaboration** because since I picked `A-frame`, I also knew other people who were picking **A-frame** as well. For instance, my friend Nancy was doing **A-frame** and together we were exploring the website and we were tinkering together as well. We helped each other out by sharing videos that we found, and _talking about what we did_, _what we understood_, and _what we didn't understood_. 

#### How to learn

I learn the skill **How to learn** because I was learning **A-frame** all on my own. I had to find resouces that were updated or at least somewhat dated so that I can learn how to use **A-frame** and the different ways in how to code / tinker. 






