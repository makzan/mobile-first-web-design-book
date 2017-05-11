## Using media query to define styles with condition

We will style our navigation on the minimal mobile-friendly website, and make it easy to click in both desktop and mobile.

Here is the result in both small and wide screen.



Here is the code to archive it.

The HTML:

``` html
<nav>
  <div class="row">
    <ul>
      <li><a href='#'>Link 1</a></li>
      <li><a href='#'>Link 2</a></li>
      <li><a href='#'>Link 3</a></li>
    </ul>
  </div>
</nav>
```

The CSS styles for normal wide screen styles.

``` css
nav li {
  width: 33%;
  float: left;
  padding: 5px;
}

nav li a {
  background: #efefef;
  display: block;
  padding: 15px 0px;
  text-align: center;
}
```

And the CSS style for small screen where the width of the viewport is smaller than 501px.

~~~ css
@media screen and (max-width: 500px) {
  nav li {
    width: 100%;
  }
}
~~~

## The mobile first approach

Here we revert the styles definition to use styles that fits mobile screen by default. When the web is displayed in a wider screen, we use the media query to define extra styles.

It’s a minor difference in code, but it’s a huge mental shift in planning website.

~~~ css
nav li {
  width: 100%;
  padding: 5px;
}

@media screen and (min-width: 500px) {
  nav li {
    width: 33.33%;
    float: left;
  }
}
~~~

