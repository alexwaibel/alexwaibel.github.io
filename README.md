# Alex Waibel's Personal Website

This repository contains my personal website and blog. It is built with [Jekyll](https://github.com/jekyll/jekyll), uses the [Minimal Mistakes theme](https://github.com/mmistakes/minimal-mistakes), and is deployed with [GitHub Pages](https://pages.github.com/).

## Local development

Open the repository in its devcontainer or a GitHub Codespace. Dependencies are installed when the container is created; start the preview server explicitly so its output and lifecycle remain visible:

```bash
bundle exec jekyll serve --livereload --force_polling
```

The site is available at <http://localhost:4000>. Run a production-style build without starting a server with:

```bash
JEKYLL_ENV=production bundle exec jekyll build
```

Outside the devcontainer, install the Ruby version in `.ruby-version`, install Bundler, and run `bundle install` first.

## Publishing

Create posts in `_posts` using the `YYYY-MM-DD-title.md` naming convention. A push to `master` builds and deploys the site through GitHub Actions. Posts dated in the future are withheld by Jekyll until their publication date.

## Updating dependencies

`Gemfile.lock` is committed so local and CI builds use the same dependency versions. Dependabot proposes monthly updates. To update manually, change the pinned `github-pages` version in `Gemfile` and the Minimal Mistakes release in `_config.yml`, then run:

```bash
bundle update github-pages
bundle exec jekyll build
```

Commit the resulting `Gemfile.lock` change with the version pins.
