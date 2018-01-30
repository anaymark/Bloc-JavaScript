# What is the difference between document.querySelector() and document.querySelectorAll()?

* document.querySelector()-using this selector will return the very first element that fits the specified selector or selectors that are entered,

* document.querySelectorAll()-using this selector will return all the elements that fit the selector or selectors that are entered, these elements will be stored in a StaticNodeList.

# What is the difference between getElement(s)By and querySelector(All)?
>getElementsBy are the "old school" and most popular ways of querying elements. The querySelector and querySelectorAll allow for more functionality, they both take multiple selectors. The querySelectors are more useful when something very specific must be found. 

* getElementsById()-returns a reference to an element with the given id, if not found will return a null

* getElementsByClassName()-returns a NodeList of elements that match the class selectors specified

* getElementsByTagName()-returns a NodeList of elements with the specified tag name

* querySelector()-returns the first element with the specified parameters provided. More dynamic as it can take all parameters. 

* querySelectorAll-returns a StaticNodeList with the specified parameters provided. Again, more dynamic as it can take a mix of all parameters. 

# What do JavaScript event handlers do and what is an example of one?
>Event handlers allow for specifing what occurs when a certain event is triggered either by user, API, loading, error, interaction, etc. There is a long list of which triggers can be used to trigger an event/function. A simple example is using an onclick event handler to specify what occurs on the click of a button. Another useful example is onload that can trigger events/functions on the loading of the browser itself.


HTML

```
<h3>Shirts</h3>
<ul id='list'>
    <li>Biker Jacket</li>
    <li>Mens Shirt</li>
</ul>
```

JS

```

let list= document.getElementById('list')

let li = document.createElement('li')
li.innerText = 'Mens T-Shirt'
list.append(li)
   
document.getElementById("list").addEventListener("click",function(e) {
         if(e.target && e.target.nodeName == "LI") {
         alert(e.target.innerText + " was selected");
        }
 });

```