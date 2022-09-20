# Dom Manipulation Assignment

## You can find solution for tasks below each question under solution section.



1. Webiste Name: [Dev To](https://dev.to/)

### Topics

    - Query Selctory, Inner HTML

### Sample Image

![Sample One](./Pic1.png)

### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

### Output

![Output](./Pic2.png)

### Solution

``` javascript
//to add name

let element =  document.querySelector(".side-bar")
element.querySelector(".crayons-subtitle-2").innerHTML = "Shantanu Pade"
'Shantanu Pade'

//to change description

let element =  document.querySelector(".side-bar")
var description = element.querySelector(".crayons-card")
description.querySelector(".color-base-70").innerText = "I love to write to code"
```

2. Website Name: [Apple](https://support.apple.com/en-in)

### Task

![Store](./Picture_3.png)

### Fetch all the product name and store in an array

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']

### Solution

```javascript
var arr = document.querySelectorAll(".as-imagegrid-item-title");
let products = [];
for (let i = 0; i < arr.length; i++){
	products.push(arr[i].firstChild.textContent.trim() )
}
console.log(products)

//output
(7) ['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']

```

3. Webiste Name: [Youtube Support](https://support.google.com/youtube/)

### Topics

    - Get Element By Id, Create Element, Create Text Node, Append Child

### Sample Image

![Sample One](./Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

### Output

![Output](./Pic5.png)

### Solution

```javascript
let element =  document.querySelector(".accordion-homepage")
let newElement = document.createElement("section")
newElement.className = "parent";
const text = (newElement.innerHTML = "<h3>My New FAQ</h3>");
element.append(newElement)

```

4. Webiste Name: [OnePlus](https://www.oneplus.in/support)

### Topics

     Query Selector, InnerText

### Sample Image

![Sample One](./Pic6.png)

### Tasks

      Change the contact number

### Output

![Output](./Pic7.png)

### Solution

```javascript
let number = document.querySelector(".contact-us .customer-support")

number.firstElementChild.innerText = "+91 6366256689"

```

5. Webiste Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Topics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out

### Output

![Output](./Pic9.png)

### Solution

```javascript
let element = document.querySelector(".listing")

for (let i=0; i < element.children.length; i++){
	element.children[i].firstElementChild.children[1].innerText = "Check Out"

}
```

6. Webiste Name: [Adidas](https://www.adidas.co.in/)

### Topics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

### Output

![Output](./Pic11.png)

### Solution

```javascript
let element = document.querySelector(".searchinput-wrapper___18TsX .searchinput___zXLAR")

function changeColor(){
	element.style.backgroundColor = "RED";
}

element.addEventListener("mouseenter",changeColor)
```

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

### Solution

```javascript
document.querySelector("#hp-search-input").value = "CSS Selectors"

let submit = document.querySelector("#hp-search-form").submit();
```

8. Webiste Name: [Google](https://www.google.com/)

### Topics

       Remove Elements

### Sample Image

![Sample One](./Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

### Output

![Output](./Pic15.png)

### Solution
```javascript
let element = document.querySelector("#SIvCob");

for (let i in element.children){
	element.removeChild(element.children[i])
}
```

9. Webiste Name: [Code Wars](https://www.codewars.com/)

### Topics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo’s background color.

### Output

![Output](./Pic17.png)

### Solution

```Javascript
let element = document.querySelector(".container .content-width-extra-large")

element.firstElementChild.style.fontFamily = "monospace"

element.firstElementChild.style.color = "#b1361e"

```

10. Webiste Name: [Freecodecamp](https://www.freecodecamp.org/)

### Topics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

### Output

![Output](./Pic19.png)

### Solution

```javascript
let element = document.querySelector(" .row .login-btn-text")

element.addEventListener("mouseover", () => {
  element.style.backgroundColor = "RED"
});

element.addEventListener("mouseout", () => {
  element.style.backgroundColor = "transparent"
});
```

11. Webiste Name: [realme](https://www.realme.com/in/)

### Topics

       querySelector,style,background-image

### Sample Image

![Sample One](./Pic20.png)

### Tasks

    change the realme logo to ineuron logo

### Output

![Output](./Pic21.png)

### Solution

```javascript
let element = document.querySelector(".header .icon-logo")

element.style.backgroundImage = "URL('https://ineuron.ai/images/ineuron-logo.png')" 
```

12. Webiste Name: [Github](https://github.com/)

### Topics

       querySelector,style,background-Color

### Sample Image

![Sample One](./Pic22.png)

### Tasks

     change the background colour of the button to blue.

### Output

![Output](./Pic23.png)

13. Webiste Name: [Hackerrank](https://www.hackerrank.com/)

### Topics

       querySelector,innerHtml

### Sample Image

![Sample One](./Pic24.png)

### Tasks

Target the top description and change “Matching developers with great companies” to ‘JSBOOTCAMP“.

### Output

![Output](./Pic25.png)

### Solution

```javascript
let element = document.querySelector(".fl-heading-text")

element.textContent = "JSBOOTCAMP"
```

14. Webiste Name: [Asus](https://www.asus.com/in/)

### Topics

      querySelector,style,font-size

### Sample Image

![Sample One](./Pic26.png)

### Tasks

       change the fontsize of “Hot Deals” to 80px

### Output

![Output](./Pic27.png)

### Solution
```javascript
let element = document.querySelector(".HotDealsAll__Heading__2fIbe")

element.style.fontSize = "80px"
```


15. Webiste Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Topics

      querySelector,style.textAlign

### Sample Image

![Sample One](./Pic28.png)

### Tasks

       Convert the text “G15 Gaming Laptop” from left to right

### Output

![Output](./Pic29.png)

### Solution

```javascript
let element = document.querySelector(".ps-top .ps-title")

element.style.textAlign =  "Right"
```

16. Webiste Name: [Vercel](https://vercel.com/)

### Topics

     querySelector,innerHTMl

### Sample Image

![Sample One](./Pic30.png)

### Tasks

      change the heading “Start with the developer” to “Start with Scratch”

### Output

![Output](./Pic31.png)

### Solution
```javascript
let element = document.querySelector(".section-title_title__VEDfK")

element.textContent = "Start With Scratch"
```

17. Webiste Name: [Sony](https://www.sony.co.in/)

### Topics

    querySelector,innerHTMl

### Sample Image

![Sample One](./Pic33.png)

### Tasks

     change the button text To current Date.

### Output

![Output](./Pic32.png)

### Solution
```javascript
let element = document.querySelector(".btn-container")
element.textContent = new Date()
```

18. Webiste Name: [Philips](https://www.philips.co.in/)

### Topics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./Pic34.png)

### Tasks

    change the background colour blue to orange

### Output

![Output](./Pic35.png)

### Solution

```javascript
let element = document.querySelector(".p-f03-footer-container")

element.style.background= "Orange"
```

19. Webiste Name: [Canon](https://in.canon/)

### Topics

          querySelector,src

### Sample Image

![Sample One](./Pic36.png)

### Tasks

    extract the canon logo

### Output

![Output](./Pic37.png)

### Solution
```javascript
let element = document.querySelector(".logo")

let logoURL = element.src

//output
logoURL
'https://in.canon/assets/brand/logo-300-002e45a4aec98fd92899838da9d5560f.png'
```

20. Webiste Name: [Oppo](https://www.oppo.com/in/)

### Topics

          querySelector,style,color

### Sample Image

![Sample One](./Pic38.png)

### Tasks

      Change the description colour black to orange

### Output

![Output](./Pic39.png)

### Solution
```javascript
let element = document.querySelector(" .wide .desc")

element.style.color = "orange"
```
