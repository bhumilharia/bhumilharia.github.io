This repository powers my personal website / blog.

## Notes for self

### About the site
- This is set up using [Hugo](https://gohugo.io/)
- The theme used is https://github.com/bhumilharia/anatole (which is a fork of another simple theme)
- This current repo (bhumilharia.github.io) has the former theme repo added as a submodule

### Setup
```bash
brew install hugo

git clone <this repo>
```

### Writing
- For adding a new blog post, add a new file `content/posts/new-post.md` (copy an existing file and modify)
- For adding a new (non-blog) page, copy `content/about.md`
- Optionally, run server `hugo server` to check if the post looks ok.
- Commit to master
- Run `./publish_to_ghpages.sh`


### Deployment
- This is hosted using GitHub Pages
- The published static files are served from the `gh-pages` branch
- Running `./publish_to_ghpages.sh` will publish latest changes to the site


## TODO
- Fix Google Analytics / Tag manager
- Setup Github Actions to automatically run `./publish_to_ghpages.sh` on master merges. Intent is to take away the local build step and make it possible to publish straight from GitHub's web UI.
- Move the salary increments post to the current blog