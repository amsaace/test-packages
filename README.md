# test-packages

#### Setup

1. Add .npmrc file to the consumer folder

`
//npm.pkg.github.com/:_authToken=PERSONAL_ACCESS_TOKEN  
@amsaace:registry=https://npm.pkg.github.com/
`

2. Add .npmrc file to the food/squab folder

`//npm.pkg.github.com/:_authToken=PERSONAL_ACCESS_TOKEN`


#### structure

Food packages are deployed to GPR and can be consumed by 
consumer.

#### issue

A bug exists with GPR where by a deployed package ends up causing 
a "404 NOT FOUND" error when the consumer tries to install it.

info
====
`yarn info @amsaace/squab`

works as expected

`npm info @amsaace/squab`

works as expected


install
=======

`yarn install`

Errors with below

https://npm.pkg.github.com/download/@amsaace/squab/1.0.2/dfd115d98665b3ddb706004d8e5e659b51af411b5ecf8b77bfb8d2238e11e5a3: Integrity checked failed for "@amsaace/squab" (none of the specified algorithms are supported)

`npm install`

works as expected

