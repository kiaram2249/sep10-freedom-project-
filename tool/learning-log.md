# Tool Learning Log

Tool: **A-frame**

---

2/26/2024: Learning Log 1
* Today I decided to look into the **A-frame** website more because I wanted to grasp a better understanding of A-frame. I want to do this because last time when I was tinkering I didn't really looked over **A-frame** seriously.
  * [A-frame](https://aframe.io/docs/1.5.0/introduction/)

3/3/2024: Learning Log 2
* Today I decided to try to use my **IDE** in order to practice A-frame. However, something wasn't working because when I made a new _file / folder_ and copy and pasted the **A-frame html** code I thought that I can do my coding like that. But, once I did **http-server** and clicked on the link, nothing was showing up. I don't know why nothing was showing up but once I get back to school tommorrow I'll ask one of my friends or I'll just ask my teacher in how to practice A-frame by using my IDE.
* Questions:
  * How can I use A-frame by using my **IDE** or my **https://cs50.dev/**?
* Since I couldn't practice in my IDE I just went to practice A-frame in **js-bin**. I just practiced on how to make 3D shapes and I try to memorized how to write a piece of the code. I also, tried to wonder what if I do that or change this. Meaning I was trying to see what would happen if I were to put this or change something from the A-frame code.
* Next time I'm gonna do a mini website practice and trying to see what my website would look like if I used A-frame. Or I can start trying to make my website by using A-frame. Basically drawing out a plan in how my website would like if I use A-frame. 

3/11/2024: Learning Log 3
* Today I watched a video that my friend Nancy shared with me because we are both doing A-frame. This video showed how to change color by using programmatic animation, setting the position, giving the sphere context, and setting texture to your 3D object. 
* [Easily code a virtual reality web experience with A-Frame (WebVR)](https://www.youtube.com/watch?v=jhEfT9YjLcU&t=576s)

My code that I did based on the video:

[http-server](https://shiny-spoon-pjrvrvrrww6gfxpv-8080.app.github.dev/index.html)
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



<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->

3/18/2024: Learning Log 4
* [Youtude A-frame](https://www.youtube.com/watch?v=qB8Ejh_QdpE&list=PLP3KjR1TMw7ekqC4o5gy0rR4odw7Jga84&index=4)
  * **Aframe = Framework**
    * Entity: **Entity** is just an empty container; (Keep things together) 
    * Component: are reusable modules that defines what the entity looks like and what it can do. (Specify the type of component) (Specify the type of properties of that componenent)
    * System
    * Architecture

Example in how to write down an entity: 

```
<a-entity component1="property1:value; property2:value;"><a-entity> 
```
```
<a-entity geometry="primitive:box" material="color:red" position="-1 0.5 -3"></a-entity>
```

* [Youtude A-frame](https://www.youtube.com/watch?v=rl104MfKbW8&list=PLP3KjR1TMw7ekqC4o5gy0rR4odw7Jga84&index=6)
* [Aframe school](https://aframe.io/aframe-school/)
  * Animation
    * Native Aframe API
    * 3rd party Components (found in the Aframe registry)
 
Component Method
```
<a-entity id="lightSphere" geometry="primitive=sphere" material="color:white; shader: flat" light="type:point" position="-4 3 -10"></a-entity>
```

3/26/2024 Learning Log 5

[Animating Objects (A-Frame Tutorial - WebVR)](https://www.youtube.com/watch?v=p3mNNZ356Ko&list=WL&index=3&t=477s)

Example of his code:
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

* This video is talking about the **different animations** and how to animate in Aframe. He shows how to write down codes in order to make the boxes move. He also talks about different types of animation movements that you can do and use. He examples lightly on position, the dur (_the timing of it_), and the repeat. I liked this video because when our class was doing the AVD I didn't do animation so for me by watching this video it was helpful. It was helpful because now I have some basic knowledge in how to do animation. 





