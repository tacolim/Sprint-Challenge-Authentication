<!-- Answers to the Short Answer Essay Questions go here -->
## Describe Middleware, Sessions (as we know them in express), bcrypt and JWT.
Middleware
Sessions
bcrypt
JWT

## What does bcrypt do in order to prevent attacks?
bcrypt makes it very difficult for someone to use brute force to figure out passwords
* bcrypt adds salt (random characters) to a password and hashes it so that it is not stored in plain text; can also adjust cost added to make the time it takes to hash salted password longer (which in turn would slow down the process for anyone trying to decrypt the password)
* when a user enters a password, bcrypt salts & hashes the password and compares it to the hashed password stored on the database

## What are the three parts of the JSON Web Token?
* Header: typically the type of token & algorithm being used
* Payload: contains claims which are statements about the entity/user and additional metadata
* Signature: hash of combined encoded header, encoded payload, and secret 