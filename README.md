# Example js cloudcode for Skygear Cloud

This is an example project for building js cloudcode for Skygear Cloud. It
uses [The Cat API](http://thecatapi.com) to demonstrate how to cloudcode
can be written to integrate with third-party libraries and services.

## Pushing cloudcode to Skygear Cloud for the first time

This example requires a Skygear Cloud account.

Once registered, add your SSH public key to the portal so that you have
permission to push your cloudcode to Skygear Cloud.

You have to set up git remote so that git knows where to push the repo to.
You are assigned a git remote URL and you have to add it to your git
repository.

```shell
$ git remote add skygear git@<url>:<app-name>.git
```

To push your code:

```shell
$ git push skygear master
```

Wait until your cloudcode is successfully built.

## Creating from scratch

If building an app serving cat photos is not your thing, you can create
a cloudcode project completely from scratch.

All you need to create a Skygear cloudcode project is a file
called `index.js`. This file serves as the entry point of your cloudcode
and it must exist in the root directory of your repository.

```shell
$ mkdir cloudcode
$ cd cloudcode
$ git init
Initialized empty Git repository in /Users/skygear/cloudcode/.git/
$ touch index.js
$ git add index.js
$ git commit -m "Initial commit"
[master (root-commit) 1e6b5f5] Initial commit
 1 file changed, 0 insertions(+), 0 deletions(-)
  create mode 100644 index.js
$ git remote add skygear git@<url>:<app-name>.git
$ git push skygear master
```

The above commands would help you build a blank git repository and push it
to Skygear Cloud. However, a blank project is probably not very useful, but
you get the idea of the bare minimum to get you started.

To get started adding features to your cloudcode, read the
[Skygear documentation](http://docs.skygear.io/).
