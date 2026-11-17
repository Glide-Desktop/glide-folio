# Glide Folio

The document viewer of the [Glide desktop](https://github.com/Glide-Desktop):
PDF through `hayro` and `lopdf`, plus PostScript, DjVu, XPS, comics, EPUB and
FB2; notes, forms, an organiser and presentation mode.

## Build

```sh
cargo build --release
```

The shared crates come from a tag of
[glide-libs](https://github.com/Glide-Desktop/glide-libs). To build against a
checkout of glide-libs next to this one, create `.cargo/config.toml` (ignored
by git):

```toml
[patch."https://github.com/Glide-Desktop/glide-libs"]
glide-config = { path = "../glide-libs/crates/glide-config" }
glide-sdk = { path = "../glide-libs/crates/glide-sdk" }
```

Split from the Glide monorepo with its history in November 2026.
