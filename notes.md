```html
<body>
  <div class="content-wrap">
    <!-- All other page content goes here -->
  </div>
  <footer class="main-footer">
    <!-- Footer content -->
  </footer>
</body>
```

```css
html, body {
  height: 100%;
  margin: 0;
}

body {
  display: flex;
  flex-direction: column;
  min-height: 100vh; /* 100% of the viewport height */
}

.content-wrap {
  flex: 1; /* This will make the content wrap to expand and fill the space */
}

.main-footer {
  background-color: steelblue;
  color: white;
  padding: 0.25em 0;
  /* No change needed here */
}
```

Explanation:

Setting the html and body height to 100% and body to a flex container ensures the total height of the content does not fall short of the viewport height.
The min-height: 100vh on the body forces the body to be at least as tall as the viewport height.
The flex: 1 property on .content-wrap makes it grow and occupy any available space, thus pushing the footer to the bottom if the content is not enough to fill the screen.