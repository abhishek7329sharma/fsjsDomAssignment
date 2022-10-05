# Dom Manipulation Assignment

## 1. Webiste Name: [Dev To](https://dev.to/)

### Topics

    - Query Selctory, Inner HTML

### Sample Image

![Sample One](./Pic1.png)

### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

### Output

![Output](./Pic2.png)

### Solution 1

```

//fetch brand
let name = document.querySelector('.side-bar .crayons-card .crayons-subtitle-2')
name.innerHTML = "Abhishek Sharma"

//fetch description
let description = document.querySelector('.side-bar .crayons-card .color-base-70')
description.innerHTML = 'I write code'

```

### Solution 1: OUTPUT

![Solution 1](./solution%201.jpg)

<hr>

## 2. Website Name: [Apple](https://support.apple.com/en-in)

### Task

![Store](./Picture_3.png)

### Fetch all the product name and store in an array

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']

### Solution 2

```

let allProductsNode = document.querySelectorAll(".as-imagegrid-item .as-imagegrid-item-title");

let allProducts =[];
for(let item of allProductsNode){
     allProducts.push(item.innerText.split('\n')[0])
}
console.log(allProducts)

```

### Solution 2: OUTPUT

![Solution 2](./solution%202.jpg)

<hr>

##

3. Webiste Name: [Youtube Support](https://support.google.com/youtube/)

### Topics

    - Get Element By Id, Create Element, Create Text Node, Append Child

### Sample Image

![Sample One](./Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

### Output

![Output](./Pic5.png)

### Solution 3:

```

// targetting navLink
let navLinks = document.querySelector('.accordion-homepage')

// creating newSection
let newSection = document.createElement('section')

// adding class to newSection
newSection.classList.add("parent")

// appending newSection and creating textNode
let newLink = newSection.appendChild(document.createTextNode('My New FAQ'))

// creating button element
let h3Button = document.createElement('h3')

// appending button with newLink created
h3Button.appendChild(newLink)

//appending h3 button inside section
newSection.appendChild(h3Button)

//appending section inside navLinks
navLinks.appendChild(newSection)

```

### Solution 3: OUTPUT

![Solution 3](./solution%203.jpg)

<hr>

## 4. Webiste Name: [OnePlus](https://www.oneplus.in/support)

### Topics

     Query Selector, InnerText

### Sample Image

![Sample One](./Pic6.png)

### Tasks

      Change the contact number

### Output

![Output](./Pic7.png)

### Solution 4

```
// targetting contact container
let contactContainer = document.querySelector(".customer-support .one-tel-number")

//changing innerText of contact
contactContainer.innerText = '+99999 99999'
```

### Solution 4:OUTPUT

![Solution 4](./Solution4.jpg)

<hr>

## 5. Webiste Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Topics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out

### Output

![Output](./Pic9.png)

### Solution 5

```
//get all buyNowButton
let buyNowNode = document.querySelectorAll('.diwali-deals-product-sale-pro .diwali-deals-product-sale-btn')

// loop around all buy now button and changing innerText
for(let item of buyNowNode){
     item.innerText = 'Check out'
}
```

### Solution 5: OUTPUT

![Solution 5](./Solution%205.jpg)

<hr>

6. Webiste Name: [Adidas](https://www.adidas.co.in/)

### Topics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

### Output

![Output](./Pic11.png)

### Solution 6

```
let searchBar = document.querySelector('.searchinput___19uW0');

searchBar.addEventListener('mouseover', (event)=>{searchBar.style.backgroundColor = 'red'})

searchBar.addEventListener('mouseout', (event)=>{searchBar.style.backgroundColor = '#eceff1'})
```

### Solution 6: OUTPUT

![Solution 6](./Solution%206.jpg)

<hr>

7. Webiste Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)

### Topics

       Form, Value, Submit

### Sample Image

![Sample One](./Pic12.png)

### Tasks

     To Search a topic in the MDN Search bar.
     First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

### Output

![Output](./Pic13.png)

<hr>

8. Webiste Name: [Google](https://www.google.com/)

### Topics

       Remove Elements

### Sample Image

![Sample One](./Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

### Output

![Output](./Pic15.png)

### Solution 8:

```
//collect all anchor tag
let element = document.querySelectorAll('#SIvCob a')

//target elment to append
let  appendElement = document.querySelector('.z4hgWe')

// make innerHTML empty first
appendElement.innerHTML = ''

// loop all elment and push only required children
for(let i=0; i < element.length; i++){
     if(i % 2 !== 0){
          // appending each child one by one to appendElement
          appendElement.appendChild(element[i])
     }
}
```

### Solution 8: OUTPUT

![Solution 8](./Solution%208.jpg)

<hr>

9. Webiste Name: [Code Wars](https://www.codewars.com/)

### Topics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo’s background color.

### Output

![Output](./Pic17.png)

### Solution 9

```
let heading  = document.querySelector('.display-heading-1');
heading.style.fontFamily = 'monospace';
heading.style.color = '#b1361e';

```

### Solution 9: OUTPUT

![Solution 9](./Solution%209.jpg)

<hr>

10. Webiste Name: [Freecodecamp](https://www.freecodecamp.org/)

### Topics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

### Output

![Output](./Pic19.png)

### Solution 10

```
let targetText = document.querySelectorAll('.login-btn-text')[1]

targetText.addEventListener('mouseover', (event)=>{targetText.style.backgroundColor = '#b1361e'})

targetText.addEventListener('mouseout', (event)=>{targetText.style.backgroundColor = '#feac32'})
```

### Solution 10: OUTPUT

![Solution 10](./Solution%2010.jpg)

<hr>

11. Webiste Name: [realme](https://www.realme.com/in/)

### Topics

       querySelector,style,background-image

### Sample Image

![Sample One](./Pic20.png)

### Tasks

    change the realme logo to ineuron logo

### Output

![Output](./Pic21.png)

### Solution 11

```
// iNeuron Logo -  https://ineuron.ai/images/ineuron-logo.png

//targetting logo
let logo = document.querySelector('a.logo.gtag')

// targetting child element
let span = document.querySelector('.icon.icon-logo.in')

// creating img tag
let img = document.createElement('img')

// adding source of iNeuron
img.src = 'https://ineuron.ai/images/ineuron-logo.png';

// adding width and height to img
img.width = '80';
img.height = '24';

// clear child first
logo.removeChild(span)

// append img tag to logo
logo.appendChild(img)
```

### Solution 11: OUTPUT

![Solution 11](./Solution11.jpg)

12. Webiste Name: [Github](https://github.com/)

### Topics

       querySelector,style,background-Color

### Sample Image

![Sample One](./Pic22.png)

### Tasks

     change the background colour of the button to blue.

### Output

![Output](./Pic23.png)

### Solution 12

```
let createRepoBtn = document.querySelectorAll('.btn.btn-sm.btn-primary')[1];
createRepoBtn.style.backgroundColor = 'blue';
```

### Solution 12: OUTPUT

![Solution 12](./Solution12.jpg)

13. Webiste Name: [Hackerrank](https://www.hackerrank.com/)

### Topics

       querySelector,innerHtml

### Sample Image

![Sample One](./Pic24.png)

### Tasks

Target the top description and change “Matching developers with great companies” to ‘JSBOOTCAMP“.

### Output

![Output](./Pic25.png)

### Solution 13

```
let header = document.querySelectorAll('.fl-heading-text')[0]
header.innerHTML = 'JSBOOTCAMP'
```

### Solution 13: OUTPUT

![](./Solution13.jpg)

14. Webiste Name: [Asus](https://www.asus.com/in/)

### Topics

      querySelector,style,font-size

### Sample Image

![Sample One](./Pic26.png)

### Tasks

       change the fontsize of “Hot Deals” to 80px

### Output

![Output](./Pic27.png)

### Solution 14

```
let text = document.querySelector('.HotDealsAll__Heading__2fIbe')
text.style.fontSize = '100px'
```

### Solution 14: OUTPUT

![Solution14](./Solution14.jpg)

15. Webiste Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Topics

      querySelector,style.textAlign

### Sample Image

![Sample One](./Pic28.png)

### Tasks

       Convert the text “G15 Gaming Laptop” from left to right

### Output

![Output](./Pic29.png)

### Solution 15

```
let title = document.querySelectorAll('.ps-title')[4];
title.style.textAlign = 'right'
'right'
```

### Solution 15: OUTPUT

![Solution 15](./Solution15.jpg)

16. Webiste Name: [Vercel](https://vercel.com/)

### Topics

     querySelector,innerHTMl

### Sample Image

![Sample One](./Pic30.png)

### Tasks

      change the heading “Start with the developer” to “Start with Scratch”

### Output

![Output](./Pic31.png)

### Solution 16

```
// targetting text DOM
let header = document.querySelectorAll('.section-title_title__VEDfK')[0];

// replacing innerHTML
header.innerHTML = 'Start with Scratch'
```

### Solution 16: OUTPUT

![Solution 16](./Solution16.jpg)

17. Webiste Name: [Sony](https://www.sony.co.in/)

### Topics

    querySelector,innerHTMl

### Sample Image

![Sample One](./Pic33.png)

### Tasks

     change the button text To current Date.

### Output

![Output](./Pic32.png)

### Solution 17

```
let date = new Date()
let btnContainer = document.querySelector('.btn-container')
btnContainer.innerHTML = date
```

### Solution 17: OUTPUT

![Solution 17](./Solution17.jpg)

18. Webiste Name: [Philips](https://www.philips.co.in/)

### Topics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./Pic34.png)

### Tasks

    change the background colour blue to orange

### Output

![Output](./Pic35.png)

### Solution 18

```
document.querySelector('.p-footer').style.backgroundColor = 'orange'
```

### Solution 18: OUTPUT

![Solution18](./Solution18.jpg)

19. Webiste Name: [Canon](https://in.canon/)

### Topics

          querySelector,src

### Sample Image

![Sample One](./Pic36.png)

### Tasks

    extract the canon logo

### Output

![Output](./Pic37.png)

### Solution 19

```
document.querySelector('.logo').src
```

### Solution 19: OUTPUT

![Solution 19](./Solution19.jpg)

20. Webiste Name: [Oppo](https://www.oppo.com/in/)

### Topics

          querySelector,style,color

### Sample Image

![Sample One](./Pic38.png)

### Tasks

      Change the description colour black to orange

### Output

![Output](./Pic39.png)

### Solution 20

```
let descriptionArray = document.querySelectorAll('.desc')
for (let item of descriptionArray) {
     item.style.color = 'orange'
}
```

### Solution 20: OUTPUT

![Solution20](./Solution20.jpg)
