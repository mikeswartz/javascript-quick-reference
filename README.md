# javascript-quick-reference
Some common use JavaScript for quick reference.

## Init closure function
```javascript
var outputDiv = document.getElementById('output');

var init = (function(val1) {
  outputDiv.innerHTML = val1;
  return {
    getFoo: function() {
      return outputDiv.innerHTML;
    },
    setFoo: function(val2) {
      outputDiv.innerHTML = val2;
    }
  }

})('first set this');

init.setFoo('replace it with this awesomeness');
```
```html
<div id="output">
  replace this
</div>
```
