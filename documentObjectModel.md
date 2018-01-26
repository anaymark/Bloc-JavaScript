# What does the acronym DOM stand for and explain in your own words what it is.

* DOM stands for document object mode. Document object model enables the HTML document to be seen as one large javascript object with all the elements being made accessable through JavaScript, as well as writable and editable. 

# How does the DOM make web programming more efficient?

* This makes programming more efficient since the HTML can be added, edited and removed through JavaScript, thus programs can interact and change the document. Moreover, this enables API's.

```
let list= document.getElementById('list')
let li = document.createElement('li')
li.innerText = 'Mens T-Shirt'
list.append(li)

```