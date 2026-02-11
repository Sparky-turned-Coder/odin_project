# HTML Boilerplate

### Creating an HTML file

It is worth noting that we named our HTML file <em>index</em>. We should always name the HTML file that will 
contain the homepage of our website <strong>index.html</strong>. This is because web servers will by default 
look for an index.html page when users land on our websites – and not having one will cause big problems.

### The DOCTYPE

The DOCTYPE heading can be long and complicated if you're trying to use an older version of HTML. But for most
purposes, you will simply include <!DOCTYPE html> to use the latest and greatest.

### HTML element

After the DOCTYPE declaration, we need to provide an <html> element. This is the <strong>root</strong> element 
of the document, meaning that every other element in the document will be a descendant of it.

This becomes more important later when we start implementing javascript in our document. For now, just know that 
<html> should be included on every HTML document.

Notice the word <em>lang</em>. It represents an HTML <strong>attribute</strong> which is associated with the given 
HTML tag. These <strong>"attributes"</strong> provide additional information about HTML elements. (More about HTML 
attributes in the following lesson)

<em>lang</em> specifies the language of the text content in that element. So, in our example, we are specifying 
that the language in our html element will be english. This allows assistive technologies, such as screen readers, 
to adapt according to the language and invoke correct pronunciation.

### Head element

The "head" element is where we put important meta-information about our webpages, and stuff required for our 
webpages to render correctly in the browser. Inside the "head", we <strong>should not</strong> use any element that displays content on the webpage.

#### Meta element

We should always have the <meta> tag with the charset encoding of the webpage in the "head" element: 
<meta charset="UTF-8">.

Setting the encoding is very important because it ensures that the webpage will display special symbols and 
characters from different languages correctly in the browser.

#### Title element

Another element we should always include in the head of an HTML document is the "title" element:

<title>My First Webpage</title>

The "title" element is used to give webpages a human-readable title, which is displayed in our webpage’s browser 
tab. For example, if you look at the current tab’s name of your browser, it will read 
“HTML Boilerplate | The Odin Project”; this is the "title" of the current .html file.

If we didn’t include a "title" element, the webpage’s title would default to its file name. In our case that 
would be index.html, which isn’t very meaningful for users; this would make it very difficult to find our 
webpage if the user has many browser tabs open.

There are many more elements that can go within the head of an HTML document. However, for now it’s only crucial 
to know about the two elements we have covered here. We will introduce more elements that go into the head 
throughout the rest of the curriculum.

### Body element

The final element needed to complete the HTML boilerplate is the <body> element. This is where all the content 
that will be displayed to users will go - the text, images, lists, links, and so on.

To complete the boilerplate, add a <body> element to the index.html file. The <body> element also goes within 
the <html> element and is always below the 'head' element

### Viewing HTML files in the browser

The HTML boilerplate in the index.html file is complete at this point, but how do you view it in the browser? 
There are a couple of different options:

1) You can drag and drop an HTML file from your text editor into the address bar of your browser.

2) You can find the HTML file in your file system and then double click it. This will open up the file in the 
default browser your system uses.

3) You can use the terminal to open the file in your browser:
    - Ubuntu: Navigate to the directory containing the file and type google-chrome index.html
    - macOS: Navigate to the directory containing the file and type open ./index.html
    - WSL: Navigate to the directory containing the file and type explorer.exe index.html. This will open the file 
in your system’s default browser. Note, You must use the filename only. Using a path (e.g., ./index.html or 
an absolute path) will open the Windows File Explorer instead.
