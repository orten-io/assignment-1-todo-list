# Todo list

You're going to make a todo list according to the provided design. The user should be able to:
- Add a task to the list
- See the added tasks
- Be able to clear all items

Please use separate files for HTML, CSS and JS (no inline styling or JavaScript). Also, please use
the provided web server. To do that, download this repository by clicking "Clone or Download" and
then "Download ZIP". Unpack it in a nice location.
To install the web server, (in bash) run `npm install` from inside this directory
(the directory where the zip file is unpacked). To start the web server, run `npm start`.
Place your project in the directory `content-base`. You can then include the StyleSheet and
JavaScript by linking them to `/` like so:

```html
<link rel="stylesheet" href="/style.css">

<script src="/app.js">
```

When you visit [http://localhost:8080](http://localhost:8080) in chrome (or whatever internet
browser you prefer) you'll find the files placed in `content-base`.

## Assets

Colors:

- Background grey/blue: `#475E67`
- Add button green: `#31D500`
- "Clear all" text red: `#C75959`
- Borders & "Add another task" placeholder grey: `#95989A`

**Font**: "Arial, sans-serif"

## Want an extra challenge?

Here are some things you can do if you feel interested and have time left:

- Display a message informing the user that they have nothing to do (when there are no tasks ofc)
- Make it responsive! Adapt it to both mobile and desktop, and make it look good on both
- Allow the user to remove individual tasks (add a delete button by each task)
- Make it smooooooth by adding some animations, i.e. when the user adds a task and clears the list

## Design

![Todo list design](https://raw.githubusercontent.com/orten-io/assignment-1-todo-list/master/design.png)
