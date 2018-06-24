# Remote Rights Advocacy Toolkit

## Dev setup

- Install dependencies

```
npm install
npm install -g bower - if you don't have bower already
bower install
```

**NOTE**: You may have to rebuild sass with `npm rebuild node-sass --force` if the next step doesn't work.

- Run the server

```
gulp serve
```

Changes will be live-reloaded in the browser as you work.

## Deployment

I didn't take the time to sort out how to use a `gh-pages` branch for this, so I just used two repos. 

`cd` indto a directory at the same level as your development directory and `git clone git@github.com:remote-rights/remote-rights.github.io.git`.

Your directory structure should look like this:

```
my-dev-dir
├── advocacy-tool-kit
└── remote-rights.github.io
```

Then run the deploy script `$ ./deploy.sh`. This script builds the app to the `dist` directory, copies the contents over to remote-rights.github.io and pushes those changes.
