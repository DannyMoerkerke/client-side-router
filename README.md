## client-side-router
This is a very basic (and naive) implementation of a client-side router implemented using Web Components that
extend the native `<nav>` and `<a>` through the `is` attribute.

For an in-depth explanation, see my article on Medium: [How To Extend A Native HTML Element](https://itnext.io/how-to-extend-a-native-html-element-1d4674e09c22?source=friends_link&sk=f399b6e4e70666eb092d5d409b3c0918)

### Usage

```html
<nav is="client-side-router" data-outlet="#main">
  <a href="/page1" is="router-link" slot="link" data-template="./page1.html">page 1</a>
  <a href="/page2" is="router-link" slot="link" data-template="./page2.html">page 2</a>
</nav>

<!-- Content will be rendered here -->
<div id="main"></div>
```


### Demo page
First run `npm install`, then `npm start` to view the demo page at
[http://localhost:8080](http://localhost:8080)
