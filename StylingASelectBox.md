# Styling A Select Box With CSS

If you've ever seen the pure HTML selection box, you will likely agree it's rather boring. Instead here's a quick tutorial on how to style your select box to be pretty with CSS. Let's do so with 5 dropdown selections with some very basic HTML:

HTML:
```html
<div class="select-style">
  <select>
    <option value="Option1">Option 1</option>
    <option value="Option2">Option 2</option>
    <option value="Option3">Option 3</option>
    <option value="Option4">Option 4</option>
    <option value="Option5">Option 5</option>
  </select>
</div>
```

Now the CSS to make it pretty:
```css
.select-style {
    border: 1px solid #ccc;
    width: 120px;
    border-radius: 3px;
    overflow: hidden;
    background: #fff url("http://www.scottgood.com/jsg/blog.nsf/images/arrowdown.gif") no-repeat 90% 50%;
}

.select-style select {
    padding: 5px 8px;
    font-size:16px;
    font-family: sans-serif;
    width: 130%;
    border: none;
    box-shadow: none;
    background: transparent;
    background-image: none;
    -webkit-appearance: none;
}

.select-style select:focus {
    outline: none;
}

.select-style select:hover {
  cursor: pointer;
  background: blue;
  color: white;
}
```

And with this you can change it to have whatever appearance you so desire. [Reference](https://coderwall.com/p/w7npmq/fully-custom-select-box-simple-css-only) 