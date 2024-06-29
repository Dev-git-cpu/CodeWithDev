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