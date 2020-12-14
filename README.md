# react-waterpipe
Waterpipe.js converted from a jQuery plugin to a React Component.

---
### Usage
1. Download import Waterpipe.js into your react component
```
import Waterpipe from './Waterpipe.jsx
```
2. Initialize
```
function App() {

  const options = {
    gradientStart: '#034A92',
    gradientEnd: '#011F3E',
    smokeOpacity: 0.1,
    numCircles: 1,
    maxMaxRad: 'auto',
    minMaxRad: 'auto',
    minRadFactor: 0,
    iterations: 8,
    drawsPerFrame: 10,
    lineWidth: 2,
    speed: 1,
    bgColorInner: "#ffffff",
    bgColorOuter: "#ffffff"
  }

  return (
    <div className="App">
      <Waterpipe options={options} />
    </div>
  );
}

export default App;
```

If no options are given than the component will automatically initialize with default settings.

---
### Options
| Option | Type | Default | Description |
| :--- | :--- | :--- | :--- |
| gradientStart | string | '#000000' | Gradient start color in hex format. |
| gradientEnd | string | '#222222' | Gradient end color in hex format. |
| smokeOpacity | number | 0.1 | Smoke opacity 0 to 1. |
| numCircles | int | 1 | Number of circles (smokes). |
| maxMaxRad | int or 'auto' | 'auto' | Could be used to change circle radius size |
| minMaxRad | int or 'auto' | 'auto' | Could be used to change circle radius size |
| minRadFactor | int | 0 | It's a factor representing the size of the smallest radius with respect to the largest possible. Integer from 0 to 1. |
| iterations | int | 8 | The number of subdividng steps to take when creating a single fractal curve. Can use more, but anything over 10 (thus 1024 points) is overkill for a moderately sized canvas. |
| drawsPerFrame | int | 10 | Number of curves to draw on every tick of the timer. |
| lineWidth | number | 2 | Line width |
| speed | int | 1 | Drawing speed (tick of timer in ms) |
| bgColorInner | string | '#ffffff' | Background outer color in hex format |
| bgColorOuter | string | '#666666' | Background inner color in hex format |


---
### Demo
See original creator for demo
https://github.com/dragdropsite/waterpipe.js/


---
### Credits
Waterpipe.js is originally developed by dragdropesite.com. View the full source code and original jQuery plugin here:
https://github.com/dragdropsite/waterpipe.js/


---
### License
Licensed under MIT license
