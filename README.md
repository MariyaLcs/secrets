# Level1

- express, body-parser (npm i express body-parser)
  body-parser extract the entire body portion of an incoming request stream and exposes it on req. body . The middleware was a part of Express. js earlier but now you have to install it separately. This body-parser module parses the JSON, buffer, string and URL encoded data submitted using HTTP POST request.

- EJS+express (npm i ejs)
  EJS is a simple templating language that lets you generate HTML markup with plain JavaScript.

  app.set("view engine", "ejs");

- mongoose (npm i mongoose)

  mongoose.connect("mongodb://localhost:27017/userDB", {useNewUrlParser: true});

# Level2 Environment variables

- mongoose-encyption (npm i mongoose-encryption)
  Simple encryption and authentication for mongoose documents.

Using environment variables

- dotenv (npm i dotenv)
  Dotenv is a zero-dependency module that loads environment variables from a .env file into process.env

  require("dotenv").config();
  .env
  secret-->process.env.SECRET
  node.gitignore

# Level3 Hashing

- md5 (npm i md5)
  a JavaScript function for hashing messages with MD5.
