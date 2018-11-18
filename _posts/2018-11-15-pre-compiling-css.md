---
layout: post
title: "Pre-compiling CSS"
date: 2018-11-15 13:27:00 +0100
category: blog
author: Mikael Eriksson
---
Before building this website I have never used pre-compiled CSS but I have heard a lot about how effective it is to use, so I was really excited to start using it when I began working on this website. For this website I used Sass, and maybe my judgement is a bit clouded by all the times I've heard or read about how great is it and how much easier and less tedious it makes writing CSS.

## Sass - why I like it
![Sass logo](/images/sass-logo.png)

There are a lot of reasons why I think Sass is superior to regular CSS and here are some of them:
 - Variables! Oh how much easier they make it to change your design as you go. Perhaps a color looked really good in Illustrator or Sketch but as you start designing the actual website you realise that it needs to be a bit darker? Well, instead of going through the entire CSS file and replace the rgba-values on every single element where it is used, you can now assign that color to a variable and only have to change it in one place. A typical Sass variable could look like this: `$text-color: #333;`. The same thing goes for any value that you would typically use in your CSS. Not sure about the font? Just create a variable like this, `$headings-font: 'Open Sans', sans-serif` and apply it to all your headings. If, later on, you realise that you want to change the font, you only need to do it in one place!
 - Nesting is now a thing. I found this to be really helpful when working with a website that I haven't created from scratch myself. Perhaps I found a class called `wrapper` by using the developer tools in my browser, and I wanted to change the background color of it. Well, since I didn't create all the CSS and HTML from scratch I don't know if the `wrapper` class is used elsewhere. Instead of searching through every single HTML file on the website, I can just use nesting to make sure that my changes only effect the elements that I intend to change. Of course, there is a solution for this in standard CSS as well, but by nesting elements within curly brackets I find it much easier to get an overview of my code and (perhaps even more important) of other developers code.

 ### What I don't like about Sass
 Of course, I have only used Sass for about a week now but I haven't found a single thing I dislike about it. Especially since even if I use Sass, there is nothing stopping me from just writing plain regular CSS instead. I could actually install and run Sass on a website just because I want it to add all necessary pre-fixes that I often forget to add myself (such as the `-webkit-` or `-ms-` pre-fixes).