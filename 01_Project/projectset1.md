# Projects related to DOM

## Project link
[Click here](https://stackblitz.com/edit/stackblitz-starters-dslwgn?file=page2.html)

# Solution code

## project 1

```javascript
const buttons = document.querySelectorAll('body');

// Using forEach to add an event listener to each button
buttons.forEach(button => {
    button.addEventListener('click', (e) => {
        if (e.target.id === 'grey') {
            button.style.backgroundColor = e.target.id;
        }
        if (e.target.id === 'blue') {
            button.style.backgroundColor = e.target.id;
        }
        if (e.target.id === 'white') {
            button.style.backgroundColor = e.target.id;
        }
        if (e.target.id === 'yellow') {
            button.style.backgroundColor = e.target.id;
        }
    });
});
```
## project 2
```javascript
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <h1>BMI Calculator</h1>

    <div class="container">
      <form>
        <p><label>Height in cm : </label><input type="text" id="height" /></p>
        <p><label>Weight in kg : </label><input type="text" id="weight" /></p>
        <button>Calculate</button>
        <div id="result"></div>
        <div id="weight-guide">
          <h3>BMI Weight Guide</h3>
          <p>Under Weight = Less than 18.6</p>
          <p>Normal Range = 18.6 and 24.9</p>
          <p>Overweight = Greater than 24.9</p>
        </div>
      </form>
    </div>
  </body>
  <script>
    const form = document.querySelector('form');

form.addEventListener('submit', function (e) {
  e.preventDefault();

  const height = parseInt(document.querySelector('#height').value);
  const weight = parseInt(document.querySelector('#weight').value);
  const result = document.querySelector('#result');

  if (height === '' || height < 0 || isNaN(height)) {
    result.innerHTML = `Please give a valid height ${height}`;
  } else if (weight === '' || weight < 0 || isNaN(weight)) {
    result.innerHTML = `Please give a valid height ${weight}`;
  } else {
    const bmi = (weight / ((height * height) / 10000)).toFixed(2);
    result.innerHTML = `<span>${bmi}</span>`;
  }
});
    
  </script>
</html>
```

```
