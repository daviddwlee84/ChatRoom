# Socket.io + Express

## Usage

```sh
node index.js
```

> http://localhost:3000/

### Docker

```sh
docker build . --tag chatroom_express
docker run -p 3000:3000 chatroom_express
```

## Improvement

* [ ] Broadcast a message to connected users when someone connects or disconnects.
* [ ] Add support for nicknames.
* [ ] Don’t send the same message to the user that sent it himself. Instead, append the message directly as soon as he presses enter.
* [ ] Add “{user} is typing” functionality.
* [ ] Show who’s online.
* [ ] Add private messaging.
* [ ] Prettifier the user interface.
