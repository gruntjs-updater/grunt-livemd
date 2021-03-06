# grunt-livemd
> Generate live-samples from markdown files

[Demo](http://benignware.github.io/grunt-livemd)

### HTML

```html
<h4 id="click-me">Click me</h4>
<style>
  h4.btn {
    border: 1px solid currentColor;
    border-radius: 3px;
    padding: 0 4px;
    cursor: pointer;
    display: inline-block;
  }
</style>
<script>
  var el = document.querySelector('#click-me');
  el.className = 'btn';
</script>
```

### CSS

```css
h4 {
  color: #0086b3;
}
```

### Javascript

```js
var el = document.querySelector('#click-me');
el.onclick = function() {
  this.style.color = '#008080'
};
```


### Coffeescript

```html
<h4 id="click-me-with-coffeescript">Click me with coffeescript</h4>
```

```coffeescript
el = document.querySelector('#click-me-with-coffeescript');
el.onclick = () ->
  this.style.color = '#008080'
```

### SCSS

```html
<h4 id="scss">Styled with SCSS</h4>
```

```scss
@import "bubble.scss";
h4#scss {
  @include bubble(#0086b3, #fff);
}
```

### Less

```html
<h4 id="less">Styled with Less</h4>
```

```less
@import "bubble.less";
h4#less {
  .bubble(#0086b3, #fff)
}
```


### Haml

```haml
%h4#haml= "Haml Example"
```