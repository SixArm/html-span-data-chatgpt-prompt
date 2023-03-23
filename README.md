# html-div-data-chatgpt-prompt

For each HTML div tag with attribute key `data-chatgpt-prompt` and blank inner
HTML, replace the inner HTML with completion message content from ChatGPT API.

Syntax:

```sh
html-div-data-chatgpt-prompt [options]
```


## Options

* -v --verbose : print verbose messages

* -i --input <FILE> : input file path

* -o --output <FILE> : output file path

* -c --change <FILE> : change file path in place


## Examples

Example input file `example.html`:

```html
<html>
  <body>
    <div data-chatgpt-prompt="define poetry"></div>
  </body>
</html>
```

Example command:

```sh
cat example.html |
html-div-data-chatgpt-prompt
```

Example output:

```html
<html>
  <body>
    <div data-chatgpt-prompt="define poetry">Poetry is a form of literature...</div>
  </body>
</html>
```

Read an input file and write an output file:

```sh
html-div-data-chatgpt-prompt --input example.html --output result.html
```

Change a file in place:

```sh
html-div-data-chatgpt-prompt --change example.html
```


## Tracking

 * Command: html-div-data-chatgpt-prompt
 * Version: 1.1.0
 * Created: 2023-03-14T11:02:13Z
 * Updated: 2023-03-23T21:04:24Z
 * License: GPL-2.0 or GPL-3.0 or contact us for more
 * Website: https://github.com/sixarm/html-div-data-chatgpt-prompt
 * Contact: Joel Parker Henderson (joel@sixarm.com)
