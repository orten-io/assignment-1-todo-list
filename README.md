# Todo list

You're going to make a todo list according to the provided design. The user should be able to:
- Add tasks to the list
- See the added tasks
- Be able to clear all items

Please use separate files for HTML, CSS and JS (no inline styling or JavaScript). Also, please use
the provided web server.

### Setting up the web server

Download this repository by clicking "Clone or Download" and then "Download ZIP". Unpack it in a nice
location. Then, you'll need to use *bash* to install and run the web server. To do so, use the bash `cd`
command to move into the directory where you unpacked the ZIP file (i.e. `cd ~/Orten.io/assignment-1-todo-list`
or `cd /c/src/assignment-1-todo-list`). Once you're in that directory and run the `ls` command, you should
see something like this:

```text
README.md	 content-base	design.png	package-lock.json	package.json
```

To install the web server, run the command `npm install` (you only need to do this once). It's important that
you're in the *assignment-1-todo-list* directory when you do this or it won't work. Then, to run the
web server, run the command `npm run start` (and same thing here, it's important you're in the
*assignment-1-todo-list* directory). Then you should see something like this:

```text
> assignment-1-todo-list@1.0.0 start /Users/johan/dev/orten/assignment-1-todo-list
> http-server ./content-base

Starting up http-server, serving ./content-base
Available on:
  http://127.0.0.1:8080
  http://172.20.10.2:8080
Hit CTRL-C to stop the server
```

You just created your first web server!

Now, if you go to [http://localhost:8080](http://localhost:8080) in your browser you'll see a web page. That's
what your web server sends to your browser. The web server lists the files you place in the directory `content-base`,
meaning that if you place more files there they'll show up.

### Adding your own web page

The web server looks for a file called `index.html` before listing the files, so if you create a file
called `index.html` that will be shown instead - and that's exactly what we want to do.

Create a file called `index.html` in the directory `content-base` and add this HTML content:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Todo list</title>
  <link rel="stylesheet" href="/style.css">
</head>
<body>
  Your site goes here
<script src="/app.js"></script>
</body>
</html>
```

This is where you should build the HTML content of the todo list. Now, if you reload the page at
[http://localhost:8080](http://localhost:8080) you should see *Your site goes here*.

### Adding styling

To add styling, create a file called *style.css* in the directory *content-base*. Here you can
write the CSS for the HTML in *index.html*. Because we linked *style.css* with
`<link rel="stylesheet" href="/style.css">` the css you add in *style.css* will affect the HTML
contents of *index.html*.

That's the setup, now it's your turn to create the HTML and CSS to make it look like the design.
Google will definitely become your best friend, but if that's not enough you can always reach us at
[emil@orten.io](mailto:emil@orten.io) and [johan@orten.io](mailto:johan@orten.io).

## Colors and fonts

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
