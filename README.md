# Pug-lint Test

This is a quick and dirty repo to test pug-lint tools. I created it to maintain "SublimeLinter-pug-lint" package, but it should work for other editors and IDE.

## Test in Terminal

```sh
# To see details. Expect 5 errors
pug-lint test.pug

# To see inline report. Expect 5 errors
pug-lint test.pug --reporter inline

# Compile pug to html
pug test.pug --pretty
```

## Test in Sublime Text 3

As usual, prepare pug-lint for ST environment:

1. In Terminal:

	```sh
	# If you installed nvm
	nvm use system

	# Required by the plugin
	npm install -g pug-lint

	# Optional for this repo
	npm install -g pug-cli
	```

1. Make sure Sublime Text 3 is working.
1. Also "[SublimeLinter][sublimelinter]" via package control
1. And also "[SublimeLinter-pug-lint][sublimelinter_pug]" via package control or local install

**Wrong:** Only see the errors in Console.

![SublimeLinter-pug-lint Wrong Screenshot][wrong_shot]

**Correct:** Shows "puglint(5|0)" and "Output: SublimeLinter" panel. No output in Console.

![SublimeLinter-pug-lint Correct Screenshot][correct_shot]

If you see something wrong, please raise an issue in "[SublimeLinter-pug-lint][sublimelinter_pug]"! :bow:

There is a `<test.json>` for reference of [SublimeLinter-json][sublimelinter_json]. Expect 1 error.


[wrong_shot]: images/sublimelinter-pug-lint-wrong-screenshot.png
[correct_shot]: images/sublimelinter-pug-lint-correct-screenshot.png

[sublimelinter]: https://github.com/SublimeLinter/SublimeLinter
[sublimelinter_pug]: https://github.com/SublimeLinter/SublimeLinter-pug-lint
[sublimelinter_json]: https://github.com/SublimeLinter/SublimeLinter-json
