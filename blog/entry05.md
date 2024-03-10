# Boostrap Writeup
##### 3/10/2024

## What is Booststrap?

Bootstrap is a powerful feature-packed because it builds anything from prototype to production and it's a free front-end framework for faster and easier web development. Bootstrap uses **HTML** and **CSS** in order to make based design templates. It can create **buttons**, **tables**, **navigation**, **modals**, **image**, and many other more. Bootstrap as well inclues **containers** because containers allows the background to fill the page and it keeps the content from reaching the edges. 

## Containers

**Containers** are important when using Bootstrap because containers contains **pad** and **align**. It gives your content within a given device or viewport. Containers are the most **basic** layout element in Bootstrap and are required when using a default grid system. However, users don't have to use a container because a container helps **center** or put a **padding** on the user content and it can be nested as well. So, when using containers you need to know that most layouts of the container don't really need to be nested inside another container. Also, there are many different kinds of containers in Bootstrap, there's 7 different kinds of containers and each container change the breaking point based on the sizes. 

* `.container`, which sets a max-width at each **responsive breakpoint**
* `.container-{breakpoint}`, which is width: 100% until the **specified breakpoint**
* `.container-fluid`, which is width: 100% at **all breakpoints**

#### Containers
![image](https://github.com/kiaram2249/sep10-freedom-project-/assets/146884636/e9d3ce6c-0882-494f-80de-5fcf15627779)

Containers are helpful because it can create different breaking points and it can help when trying to make a **cols / row** or when you want to display something in a way for your website. It's also helpful because it allows your content to be view on different view screens. For instance, if your website looks good on a phone device but you want it to look good in all devices you can use containers in order to do that. 

#### Breakpoints
![image](https://github.com/kiaram2249/sep10-freedom-project-/assets/146884636/a880d92a-2df7-4b6d-b9cd-f9db404aaca8)

#### How I used container: 

```
 <div class="container-fluid">
            <div class="container">
                <div class="row">
                    <div class="col">
                       <p>example</p>
                    </div>
                </div>
            </div>
        </div>
```

### Components

In Bootstrap their are many **components** to use and learn about. Bootstrap has many components that are already have pre-made codes that people can use. Bootstrap even have different way in coding that one same component that user picked. Components are helpful because it allows the user to customize their website and it allows them to have many features added to their website. For instance, I used **navbar**, **close button**, and the **buttons** when I was practicing components. 

#### The Navbar that I used: 
```
<nav class="navbar navbar-expand-lg navber-light bg-light" id="Scroll">
   <div class="container-fluid">
     <a class="navbar-brand" href="#">ANIME</a>
     <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-                       controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
       <span class="navbar-toggler-icon"></span>
     </button>
     <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
       <div class="navbar-nav">
         <a class="nav-link" href="#Manga">Manga</a>
         <a class="nav-link" href="#Anime Movies">Anime Movies</a>
         <a class="nav-link" href="#Anime Episodes">Anime Episodes</a>
       </div>
     </div>
   </div>
 </nav>
```

#### The closing button that I used:
```
 <div data-bs-theme="light">
   <button type="button" class="btn-close" aria-label="Close"></button>
   <button type="button" class="btn-close" disabled aria-label="Close"></button>
 </div>
```

#### The Button that I used: 
```
<button type="button" class="btn btn-info" id="color1">Manga Shop</button>
<button type="button" class="btn btn-light" id="color2">Recommendation</button>
<button type="button" class="btn btn-dark" id="color3">Voice Actors</button>
```

Text

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
