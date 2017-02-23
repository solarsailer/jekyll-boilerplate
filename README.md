# Jekyll Boilerplate

[Jekyll](https://jekyllrb.com/) is a static site generator built with [Ruby](https://www.ruby-lang.org/) and used by GitHub.

This is a basic and fully functional boilerplate to start creating a site with Jekyll, including a paginator, a 404 page, a sitemap and atom feed, as well as a few layouts and the necessary includes.

It also integrates a build pipeline with [Webpack](https://webpack.js.org/):

* Sass files are converted to CSS and augmented with Autoprefixer.
* JavaScript files are processed through Babel with the ES2015 preset.

## Installation

1. Install [Jekyll](https://jekyllrb.com/docs/installation/)
2. Install [Install Yarn](https://yarnpkg.com/en/docs/install)
3. Install dependencies with `yarn install`

## Usage

### Development

The development pipeline uses Browser-Sync, Webpack and Jekyll, through simple Yarn tasks.

To start, just run:

```
yarn run start
```

A server will be started on `localhost:8080`.

### Production

Ready to put in production? Just use:

```
yarn run build
```

And copy the files of the `_site` folder on your server, by any means.

It is also conceived with **GitHub Pages** in mind (we don't use the `github-pages` gem, but our Gemfile uses the required version for all the gems). _If you use this boilerplate for your organization/profile page, it should normally be built by GitHub automatically without errors._

So, don't forget to run `yarn run build` (and commit the files) before pushing your changes to your repo.

NB: For a project page, you need to configure this a bit to build the site in the `/docs` folder of your repository.
