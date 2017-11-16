[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

# Red Hat UXD Design Tracker Template

This template is for creating a website to track designs created by a UXD team. Built on Jekyll using GitHub pages, this template will enable you to quickly get up and running with a basic set of sortable and filterable tables, patterns for adding designs links and sharing stories from any issue tracking system.

View the [Changelog](CHANGELOG.md)

View the [Wiki](https://github.com/rh-uxd/design-tracker-template/wiki)

---

## Installation

| This installation requires that you have Ruby, Node, Gem, Jekyll and Gulp installed. You can find a list of dependecies with versions here: [Design Tracker Dependencies](https://github.com/rh-uxd/design-tracker-template/wiki/Dependencies)

1. Fork this repository
1. Rename as desired (we recommend with UX in the name)
1. Clone to your local machine
1. With Node, Gulp, Ruby, Gem and Jekyll already installed, run `npm run initialize`
1. Start with `jekyll serve`
1. Code away!

### First Time Build
1. Verify that you have the following installed:
    - Node
    - Gulp
    - Gem
    - Jekyll
2. run `gem install bundler`
3. run `npm install`
4. run `gulp`
    - this will copy the files from your
    npm_modules directory to their respective
    locations for the jekyll build process
5. run `jekyll build`
6. run `jekyll serve`
    - for viewing locally at http://localhost:4000

### Subsequent Builds
1. `jekyll serve` to start your environment on port `:4000`.

### Troubleshooting
If you are having issues with the site building, you can run a set of cleaning commands to reset your environment.

#### Environment Troubles
- `npm run reinstall`
    - This will clear out your **node_modules** folder, any vendor folders, reinstall all modules and copy vendor files back to their respective locations.
- `gulp cleanVendors`
    - This will remove just the vendor files that were copied over during the `gulp` process.
    - Run `gulp` to copy a clean set of vendor files back to your directories.

#### Gem Issues
If you have issues with your gem bundles, you can run the following command:
- `bundle update`
    - This will check for any updates to your gem bundles, cleaning old bundles.
