## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/MadalinaaM/MDPI/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/MadalinaaM/MDPI/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
<html> 
 <h3> Exercise 4 </h3>
 <script> 
 document.cookie = "session=test GDPR"; 
 document.cookie = "favorite_task=collect Data";
 function alertCookie() { alert(document.cookie); }
</script>
 <body> Bine ai venit la lab <button onclick="alertCookie()">Show cookies</button>
 <h3> Exercise 5 </h3>
  /* ---------------------Example #1--------------------------------------------------*/
  <p>Example #1</p>
  <script>
 document.cookie = "name=oeschger; SameSite=None; Secure";
document.cookie = "favorite_food=tripe; SameSite=None; Secure";
   function showCookies() {
  const output = document.getElementById('cookies')
  output.textContent = '> ' + document.cookie
}

function clearOutputCookies() {
  const output = document.getElementById('cookies')
  output.textContent = ''
}
  </script>
  <button onclick="showCookies()">Show cookies</button>

<button onclick="clearOutputCookies()">
  Clear
</button>

<div>
  <code id="cookies"></code>
</div>
<br>
    /* ---------------------Example #2--------------------------------------------------*/
  <p>Example #2</p>
 <script>
  document.cookie = "test1=Hello; SameSite=None; Secure";
document.cookie = "test2=World; SameSite=None; Secure";

const cookieValue = document.cookie
  .split('; ')
  .find(row => row.startsWith('test2='))
  .split('=')[1];

function showCookieValue() {
  const output = document.getElementById('cookie-value')
  output.textContent = '> ' + cookieValue
}

function clearOutputCookieValue() {
  const output = document.getElementById('cookie-value')
  output.textContent = ''
}
 </script>
  <button onclick="showCookieValue()">Show cookie value</button>

<button onclick="clearOutputCookieValue()">
  Clear
</button>

<div>
  <code id="cookie-value"></code>
</div>
<br>
    <!- ---------------------Example #3--------------------------------------------------->
  <p>Example #3</p>
  <script>
   function doOnce() {
  if (!document.cookie.split('; ').find(row => row.startsWith('doSomethingOnlyOnce'))) {
    // Note that we are setting `SameSite=None;` in this example because the example
    // needs to work cross-origin.
    // It is more common not to set the `SameSite` attribute, which results in the default,
    // and more secure, value of `SameSite=Lax;`
    document.cookie = "doSomethingOnlyOnce=true; expires=Fri, 31 Dec 9999 23:59:59 GMT; SameSite=None; Secure";

    const output = document.getElementById('do-once')
    output.textContent = '> Do something here!'
  }
}

function clearOutputDoOnce() {
  const output = document.getElementById('do-once')
  output.textContent = ''
}

  </script>
  <button onclick="doOnce()">Only do something once</button>

<button onclick="clearOutputDoOnce()">
  Clear
</button>

<div>
  <code id="do-once"></code>
</div>

</body>
</html>
