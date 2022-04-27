# arthur-azure-resume

My own Azure Resume , Following ACG project video

## First Steps

- frontend older contains the website.
- main.js contains counter code.

```js
window.addEventListener("DOMContentLoaded", (event) => {
  getVisitCount();
});

const functionApi = "";

const getVisitCount = () => {
  let count = 30;
  fetch(functionApi)
    .then((response) => {
      return response.json;
    })
    .then((response) => {
      console.log("Website called function API");
      count = response.count;
      document.getElementById("counter").innerText = count;
    })
    .catch(function (error) {
      console.log(error);
    });
  return count;
};
```
