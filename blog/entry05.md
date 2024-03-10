# Boostrap Writeup
##### 3/10/2024

Is a free front-end framework for faster and easier web development
We can import it just like we do with any other (CSS) file
Includes HTML and CSS based design templates for typography, forms, buttons, tables, navigation, modals, image carousels and many other, as well as optional JS plugins
Mostly just by giving elements pre-made classes
Gives you the ability to easily create responsive design

.container vs .container-fluid
.container is fixed width
.container-fluid is 100% width
A common practice is to put a .container inside of a .container-fluid
This allows the background to fill the page, but keeps the content from reaching the edges
.container-SIZE will behave like .container-fluid on anything smaller than SIZE

Bootstrap is a powerful, feature-packed frontend toolkit. Build anything—from prototype to production—in minutes.

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







Text

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
