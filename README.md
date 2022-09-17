# Move with Mouse Cursor

A simple javascript implementation of element moving with the cursor. Made a simple UI and a cursor which has basic styling and code.

### CSS

> only mandatory style is `position: absolute`. Rest can be styled as you like.

```CSS
.mousefollow {
  background-color: transparent;
  width: 100px;
  height: 100px;
  border-radius: 50%;
  position: absolute;
  box-shadow: 0 0 3px rgba(0, 0, 0, 0.55);
  display: flex;
  place-items: center;
  place-content: center;
  color: #fff;
}
```

### Javascript

> Get the `x` and `y` coordinates of the mouse pointer and use those values as the `translate` property of the above element. Do this by attaching a `mousemove` event on the document or window.

```JavaScript
let pop = document.getElementById("pop");
document.addEventListener("mousemove", (event) => {
  pop.style.translate = `${event.clientX}px ${event.clientY}px`;
});

```
