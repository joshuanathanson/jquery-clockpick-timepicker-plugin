# jQuery ClockPick Plugin

[View the ClockPick demo](https://joshuanathanson.github.io/clockpick.html)

## Configuration

### Basic

After including the jQuery script in your HTML head block, include the ClockPick script:

```html
<script src="path/to/jquery.clockpick.js"></script>
```

Include the ClockPick stylesheet:

```html
<link rel="stylesheet" href="path/to/clockpick.css" type="text/css">
```

Then, in your `$(document).ready` block, add the following:

```javascript
$("#clockpick").clockpick();
```

This assumes you are binding the plugin to an element with the id `clockpick`. You can bind it to any element that makes sense for your use.

### Adding parameters

ClockPick takes two optional parameters:

- `options` (hash): an object containing settings keys and their values
- `callback` (function): a callback function to run after ClockPick is run

Example:

```javascript
$("#clockpick").clockpick({
  starthour: 6,
  endhour: 15,
  showminutes: false
}, mycallback);
```

### Click target different than value field

If you want the action on a different element than the time field, configure it as below (like the "click on clock" demo).

Assuming the field you want to fill with the time has the name `myfieldname`:

```javascript
$(".clockpick").clockpick({
  valuefield: 'myfieldname'
});
```
