# 1C:Enterprise - a language grammar for highlight.js

![version](https://badgen.net/npm/v/highlightjs-1c-enterprise) ![license](https://badgen.net/badge/license/MIT/blue)
![install size](https://badgen.net/packagephobia/install/highlightjs-1c-enterprise) ![minified size](https://badgen.net/bundlephobia/min/highlightjs-1c-enterprise)

## Usage

Simply include the Highlight.js library in your webpage or Node app, then load this module.

### Static website or simple usage

Simply load the module after loading Highlight.js.  You'll use the minified version found in the `dist` directory.  This module is just a CDN build of the language, so it will register itself as the Javascript is loaded.

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" src="/path/to/1c-enterprise.min.js"></script>
<script type="text/javascript">
  hljs.highlightAll();
</script>
```

### Using directly from the UNPKG CDN

```html
<script type="text/javascript"
  src="https://unpkg.com/highlightjs-1c-enterprise@1.0.0/dist/1c-enterprise.min.js"></script>
```

- More info: <https://unpkg.com>

### With Node or another build system

If you're using Node / Webpack / Rollup / Browserify, etc, simply require the language module, then register it with Highlight.js.

```javascript
var hljs = require('highlight.js');
var hljs1C_Enterprise = require('highlightjs-1c-enterprise');

hljs.registerLanguage("1c-enterprise", hljs1C_Enterprise);
hljs.highlightAll();
```


## License

Released under the MIT License. See [LICENSE][1] file for details.

### Author(s)

maniac <> and other contributors

### Maintainer

Josh Goebel <hello@joshgoebel.com>


## Links

- The official site for the Highlight.js library is <https://highlightjs.org/>.
- The Highlight.js GitHub project: <https://github.com/highlightjs/highlight.js>
- Learn more about 1C:Enterprise: <https://1c-dn.com/1c_enterprise/what_is_1c_enterprise/>

[1]: https://github.com/highlightjs/highlightjs-1c-enterprise/blob/main/LICENSE
