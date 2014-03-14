NodeInTheClouds
===============

Présentation pour le Meetup du 6 mars - Disruptive-technologies-in-Planet-Marseille

Et le bout de code de l'exemple :
```javascript
var express = require("express");
var logfmt = require("logfmt");
var app = express();

app.use(logfmt.requestLogger());

app.get('/', function(req, res) {
  res.send('Hello World!');
});

var port = Number(process.env.PORT || 5000);
app.listen(port, function() {
  console.log("Listening on " + port);
});
```
