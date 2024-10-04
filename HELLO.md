# Reactive menu button

## Activity Directions

|||info

## [Preview your page](open_preview Week1/5_Practice/index.html panel=1)

|||

|||important

#### Use only `transition` and not `animation`

|||

### 1. When the hamburger is clicked, toggle the `.hamburger--open` class name

**In `index.js`:**

1. Add a 'click' event listener on the hamburger reference, that when fired will toggle the class name "hamburger--open"
   ```javascript
   hamburger.addEventListener("click", () => {
     // code here
   });
   ```
2. When the hamburger is clicked, the middle line should disappear! When clicked again it should reappear.

### 2. Add transitions

1. Add this to `.hamburger-inner`, `.hamburger-inner::before`, and `.hamburger--inner::after`:
   - `transition: all 0.4s ease-in-out;`
2. Now the middle line should be slowly disappearing and reappearing.

### 3. Rotate the top and bottom lines

1. Add a `transform` of `rotate(45deg)` to the `.hamburger-—open .hamburger-inner::after`
2. Add a `transform` of `rotate(-45deg)` to the `.hamburger—open .hamburger-inner::before`
3. For both `.hamburger-—open .hamburger-inner::after` and `.hamburger—open .hamburger-inner::before` rulesets, add a `top` of `calc(var(--hamburger-layer-height) * 2)`
