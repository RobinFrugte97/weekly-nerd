# Hackathon

During one of the weekly nerds of the minor web development, we were invited to
the Leeuwenburg HvA building to do a hackathon for master students. There were a
lot of interesting cases to have a go with during the 4 hour long hackathon, but
in light of the recent theme of real-time web during the latest courses, one case
stood out to me and two other students.

## Digital noteboard

One of the master's educators, Gabriel, had an interesting case for the three of us. He wanted a way to digitalize sticky notes so he could share them with his students
or colleagues. For example, he wanted to share sticky notes on-the-go on a photograph that one of his students had made on a fieldtrip. We immediately had the idea to
do something with real-time web technologies. We thought of giving Gabriel and his
students the ability to upload a photo and to make it so a sticky note would be
created wherever the user would click. We quickly figured out how we wanted to
achieve a real-time product; Socket.io

## Socket.io

[Socket.io](https://socket.io/) is a real-time engine to be used, in our example,
[Node.JS](https://nodejs.org/en/about/). Socket.io allows direct communication
between your front-end and server-side JavaScript. This allows you to directly share
information between all, or a particular group of the users connected to the server.

Socket.io requires you to include and install a number of things;

First, install the package through a package manager, like npm;
> npm install --save socket.io

Then, require Socket.io in your server-side JavaScript.
``` javascript
var io = require('socket.io')(http);
```

After that, link the Socket.io JavaScript file in your HTML.
``` html
<script src="/socket.io/socket.io.js"></script>
```

Lastly, listen on the 'connection' event to start off with Socket.io
``` javascript
io.on('connection', function(socket){
  console.log('a user connected');
});
```

## 4 hours later

The project was coming along nicely. At the end of the hackathon period we made it
so a user could upload a picture from their local directory, or take a picture with their phone.
The uploaded picture would immediately be shared to all connected users
by sending the [BLOB](https://developer.mozilla.org/en-US/docs/Web/API/Blob) of the picture through the server.
A BLOB is essentially the picture in raw data, which we could share between the users as a string.

The users could share messages by clicking on the picture and writing/sending the
sticky note.

[]()

## The aftermath

Gabriel seemed to be impressed by what we made in a mere 4 hours. To be honest, we were quite impressed ourselves that we managed to build something in a couple of hours, which had taken us weeks to learn.
