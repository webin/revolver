# onStop

**Default**: `function(){}` 

**Type**: `Function`

This is a callback that you can pass through the options object to the constructor. Internally, it is registered as a listener to the [stop](https://github.com/revolverjs/revolverjs/blob/master/docs/revolver.events.stop.md) event using the [on](https://github.com/revolverjs/revolverjs/edit/master/docs/revolver.methods.on.md) method.

```javascript
var slider =  new Revolver($('.slides'), {
  onStop: function() {
    // this == slider
  }
});
```

**Note**: The `this` variable inside the callback is equal to the Revolver instance.