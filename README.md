# My Portfolio Landing Page Website


## Technology Used 

| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
| HTML    | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | 
| CSS     | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)      |   
| Git | [https://git-scm.com/](https://git-scm.com/)     | 


## Description 

[Visit the deployed site](https://bryannguyen9.github.io/Bryan-Nguyen-Portfolio/)

This project was started with the goal in mind to create a page that all could visit in order to learn  more about me, contact me, and see some of my previous work. 

It offers a cohesive website that allows users to switch in between navigation bar links and find about both how to contact me, a brief description of who I am, and a portfolio page that shows my past work with clickable images so they can navigate to live sites for those respective projects.

Again here is a link to my fully deployed website: 
[Portfolio Site Home](https://bryannguyen9.github.io/Bryan-Nguyen-Portfolio/)


## Table of Contents

* [Code Example](#code-example)
* [Usage](#usage)
* [Learning Points](#learning-points)
* [Author Info](#author-info)
* [Credits](#credits)
* [License](#license)


## Code Example

Here is an example code within my index.html that shows how I created my portfolio page within a portfolio-card and how I implemented a link within the actual image so users can click on the image when wanted to view my live site.

```html
<section id="portfolio-content" >
      
        <h2>portfolio</h2>
          <figure class = "portfolio" id="portfolio-card">          
                <h3> Horiseon Landing Page</h3>
                  <p> 
                    This is one of my first projects where I refactored code in order <br>
                    to make the website compliant with current accessibility terms and <br>
                    conditions. I cleaned up code behind the scenes and added semantic <br>
                    HTML elements in order to make the overall website more accessible. <br>
                  
                  </p>
                <figure class="flex-img">
                  <a href="https://bryannguyen9.github.io/3-20-23-challenge/"><img src="./Assets/images/horiseonproject1.png" alt="Screenshot of my most recent projects"/></a>
                </figure>
          </figure>
```


Here is my style.css for how I configured my portfolio page and the cards to zoom in when hovered over as well as being within the flex property to allow minimization when the screen is shrunk.

```css
.portfolio {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  text-align: center;
  border: 5px solid black;
  border-radius: 10px;
  flex: 1;
}

.portfolio:hover {
  transform: scale(1.2);
  -webkit-transition: transform 0.5s ease-in-out;
}

#portfolio-card {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  max-width: 30%;
  text-align: center;
  margin-top: 150px;
  margin-left: 50%;  
}
```

Here is an example of my navigation links that allow users to click in between the buttons within the navigation bar and see the different pages within my site.

```html
<header>
      <img src="./Assets/images/myicon.png" alt="Company Icon" />
      <h1>Bryan Nguyen Portfolio Site</h1>
        <nav>
          <ul class = "asideMain">
              <li>  
                  <a href="#about-me-content">about me</a>
              </li>
              <li>
                  <a href="#links-content">links</a>
              </li>
              <li>
                  <a href="#portfolio-content">portfolio</a>
              </li>
              <li>
                  <a href="#contact-me-content">contact me</a>
              </li>
          </ul>
```

This is the corresponding style.css that allows the user to toggle between different pages. Here I used the mechanic of display none and display block to show a certain page when a user clicks on the navbar link and nothing else.

```css
header nav a:hover {
  background-color: lightgray;
  color: black;
}

#about-me-content, #portfolio-content, #links-content, #contact-me-content {
  display: none;
}

#about-me-content:target, #portfolio-content:target, #links-content:target, #contact-me-content:target {
  display: block;
}
```

## Usage 

Here we see the header links on the landing page and how when click they lead 
to the corresponding pages within the site.

![live site navigation bar screenshot](./assets/images/navbarlinkexample.png)

Here we see that when hovered over within the portfolio page, my past project images will zoom in to focus on them. You can also click them to get to my live sites!

![live site portfolio zoom screenshot](./assets/images/portfoliozoomex.png)


## Learning Points 

There was a lot of research done with regards to different aspects within this portfolio site.

Some major points were:

* switching in between navigation bar links so that each page would show and no other pages would show

* allowing zoom abilities for portfolio images when hovered over

* flex properties and how to properly flex wrap all the different properties within my website so that when the screen is minimized users are able to see the same website but still have the same functionality as if it were the normal size.

These are some of the links I used to teach me these main points:
1. [W3 Schools](https://www.w3schools.com/cssref/css3_pr_flex.php)
2. [W3 Schools](https://www.w3schools.com/howto/howto_css_zoom_hover.asp)


## About Me

Hi, my name is Bryan Nguyen I am an up and coming full-stack web developer working
on getting into the space with projects that support both my growth, belief, and imagination. I hope to one day work within the realm of AI, web-development, and even site-reliability/the space of cyber-security.


### My links

* [Portfolio](https://bryannguyen9.github.io/Bryan-Nguyen-Portfolio/)
* [LinkedIn](https://linkedin.com/in/bryannguyen9)
* [Github](https://github.com/bryannguyen9)


## Credits

# Special thanks to David Chung: 
 
 * His Github Portfolio: [David-Chung-Github](https://github.com/dchung13/)
 * His Linked-In: [David-Chung-LinkedIn](https://www.linkedin.com/in/david-chung-77141526b/)
 * His Portfolio Site: [David-Chung-Portfolio](https://dchung13.github.io/David-Chung-Portfolio/) 

# Special thanks to these reference websites that taught me different functionalities within my website for me to create a seamless experience for users.

1. [W3 Schools](https://www.w3schools.com/cssref/css3_pr_flex.php)
2. [W3 Schools](https://www.w3schools.com/howto/howto_css_zoom_hover.asp)


## License

MIT License

Copyright (c) [2023] [Bryan-Nguyen]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
