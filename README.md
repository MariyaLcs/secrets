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

# Level4 Hashing & Salting

- bcrypt (npm i bcrypt)
  bcrypt is a password-hashing function
  It uses a 128-bit salt and encrypts a 192-bit magic value as noted in the USENIX documentation. "bcrypt" foces you to follow security best practices as it requires a salt as part of the hashing process.

  Node Version Manager
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
  nvm --version

  const saltRounds = 10;
  bcrypt.hash(myPlaintextPassword, saltRounds, function(err, hash){})
  bcrypt.compare(myPlaintextPassword, hash, function(err, result) {})

# Level5 Passport.js

- npm i passport passport-local passport-local-mongoose express-session

  app.use(session({secret: "Our little secret", resave: false,saveUninitialized: false,}));
  app.use(passport.initialize());
  app.use(passport.session());

  userSchema.plugin(passportLocalMongoose);

  passport.use(User.createStrategy());
  passport.serializeUser(User.serializeUser());
  passport.deserializeUser(User.deserializeUser());

# Level6 OAuth2.0

- passport-google-oauth20 (npm install passport-google-oauth20)
  This module lets you authenticate using Google in your Node.js applications.

  https://console.developers.google.com/

  # Social Buttons for Bootstrap
