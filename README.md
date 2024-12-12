# Clock Display - Real-Time Digital Clock

This project is a simple **real-time digital clock** built using HTML and JavaScript. It updates every second and displays the current time in the format specified by the browser's locale.

## Features
- Displays the current time in real-time.
- Updates every second without requiring a page refresh.
- Uses the `toLocaleTimeString()` method for localized time format.

## Code Explanation

### HTML Structure
```html
<div id="clock"></div>
```
- **`<div id="clock">`**: A placeholder element where the current time will be displayed.

### JavaScript Code
```javascript
const clock = document.getElementById('clock')

setInterval(() => {
    const date = new Date()
    clock.innerHTML = date.toLocaleTimeString()
}, 1000);
```

1. **`const clock = document.getElementById('clock')`**: Selects the clock `<div>` element from the DOM.
2. **`setInterval`**: Executes the provided callback function every 1000 milliseconds (1 second).
3. **`new Date()`**: Creates a new `Date` object to get the current date and time.
4. **`toLocaleTimeString()`**: Formats the
