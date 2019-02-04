# buck-flavours-across-cells

This does not work:

```bash
buck run :app#strawberry
```

... because `foo//:foo` does not have flavour `strawberry`.

But we *can* define it using args:

```
buck run --flagfile ./strawberry.args :app#strawberry
```
