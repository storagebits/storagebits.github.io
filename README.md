# storagebits.github.io

The source of [storagebits.github.io](https://storagebits.github.io/), the personal site of storagebits, published by GitHub Pages.

## What it does

GitHub Pages builds the site with [Jekyll](https://jekyllrb.com/) from the Markdown files of the `main` branch, with the [Minimal](https://github.com/pages-themes/minimal) theme, and serves it at https://storagebits.github.io/. Every push to `main` republishes the site within a minute or two.

## Status

Placeholder. The site is live, but its only page (`index.md`) still holds GitHub's starter text: no real content has been written yet.

## Getting started

Edit `index.md` (or add pages next to it) and push to `main`; GitHub Pages does the rest.

To preview locally, you need Ruby 3.x with Bundler. Then, from a clone of this repository:

```sh
cat > Gemfile <<'EOF'
source "https://rubygems.org"
gem "github-pages", group: :jekyll_plugins
gem "webrick"
EOF
bundle install
bundle exec jekyll serve      # then open http://127.0.0.1:4000/
```

The `github-pages` gem pins the same Jekyll and theme versions as GitHub Pages. Do not commit the `Gemfile`, `Gemfile.lock` or `_site/` it creates unless you mean to.

## Configuration

`_config.yml` holds the Jekyll settings: the theme (`jekyll-theme-minimal`) and the files kept out of the site (`README.md`, `LICENSE`). The Pages source branch and the custom domain, if any, are set in the repository's settings (Settings → Pages), not in a file.

## Project layout

```
_config.yml   Jekyll settings (theme, excluded files)
index.md      home page
```

## Licence and credits

Released under the [MIT licence](LICENSE). The [Minimal](https://github.com/pages-themes/minimal) theme is by GitHub and released under CC0 1.0.
