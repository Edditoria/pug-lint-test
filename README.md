# Test for Pug-lint

This is a quick and dirty repo to test pug-lint and "SublimeLinter-pug-lint" in Sublime Text 3.

## Prepare

As usual, you need to install:

1. In Terminal:

	```sh
	# If you installed nvm
	nvm use system
	# Required by the plugin
	npm install -g pug-lint
	# Optional for this repo
	npm install -g pug-cli
	```

1. Sublime Text 3
1. "SublimeLinter" via package control
1. "SublimeLinter-pug-lint" via local install or package control

## Play

In Terminal:

```sh
# To see details. Expect 5 errors
pug-lint test.pug
# To see inline report. Expect 5 errors
pug-lint test.pug --reporter inline
```
