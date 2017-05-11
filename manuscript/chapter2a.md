## Minimal mobile friendly website

The following code example shows how we can create a minimal website style that fits in small screen reading.

The HTML:

```
<header>
  <div class="row">
    Website Title here
  </div>
</header>

<nav>
  <div class="row">
    <ul>
      <li>Link 1</li>
      <li>Link 2</li>
      <li>Link 3</li>
    </ul>
  </div>
</nav>

<div class="row">
  <article>
    <header>
      <h1>Heading of the content</h1>
    </header>

    <p>Content paragraphs go here.</p>

    <footer>
      Author: Makzan
    </footer>

  </article>
</div>

<footer>
  <div class="row">
    Copyright goes here.
  </div>
</footer>
```

The CSS:

```
/* normalize */
body, nav, ul, li, p, h1, h2, h3 {
    padding: 0;
    margin: 0;
}

/* core styles */
* {
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
}

body > header,
body > footer {
    background: #ffce25;
}

.row {
    width: 100%;
    max-width: 600px;
    margin: 0auto;
    padding: 10px;
}

/* addition styles */
ul {
    list-style: none;
}

h1, p {
    margin-bottom: .5em;
}
```

Note: We used box-sizing in our CSS. You may reference to the Mozilla documentation.

Please find the following screenshot showing the minimal web site display in both normal view and article view in mobile Safari.

![sample-article-normal](https://junkdraft.s3.amazonaws.com/attachments/1/670/original/4fa7a8fccd6d741f0c7ee412928358495382b3e3/sample-article-normal.png)

![Website showing in iPhone article view](https://junkdraft.s3.amazonaws.com/attachments/1/671/original/5cbe638f60cf177e4ba0b24854ba581762648c28/sample-article-article-view.png)

