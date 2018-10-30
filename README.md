Page Redirection
===

```
rd.ccns.moe/<token> -> http://redirect.ccns.moe/?token=<token> -> <custom_url>
```

Redirection token map is in `index.html`
```
const token_mapping = {
    get: function(target, name) {
        return target.hasOwnProperty(name) ? target[name] : "https://www.ccns.io/";
    },
    null: "https://www.ccns.io/",
    "sa": "https://hackmd.io/c/rkC3tk8im/",
    "book": "https://hackmd.io/c/HyEmupOg7/",
}
```