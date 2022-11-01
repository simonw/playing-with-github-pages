# playing-with-github-pages

- https://simonw.github.io/playing-with-github-pages/ serves `index.html`
- https://simonw.github.io/playing-with-github-pages/foo serves `foo.html`
- https://simonw.github.io/playing-with-github-pages/foo.html serves `foo.html`
- https://simonw.github.io/playing-with-github-pages/bar.json serves `bar.json`
- https://simonw.github.io/playing-with-github-pages/bar serves a 404 (actually the custom `404.html` page)

And in a `folder/`:

- https://simonw.github.io/playing-with-github-pages/folder redirects to `/folder/`
- https://simonw.github.io/playing-with-github-pages/folder/ serves `folder/index.html`
- https://simonw.github.io/playing-with-github-pages/folder/index serves `folder/index.html`
- https://simonw.github.io/playing-with-github-pages/folder/index.html serves `folder/index.html`
- https://simonw.github.io/playing-with-github-pages/folder/baz serves `folder/baz.html`
- https://simonw.github.io/playing-with-github-pages/folder/baz.html serves `folder/baz.html`

The existence of the `.nojekyll` file causes GitHub Pages to publish the raw files without attempting to run Jekyll against them first.
