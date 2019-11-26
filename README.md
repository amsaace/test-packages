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

`yarn install`
