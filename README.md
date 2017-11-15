[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

# Red Hat UXD Design Tracker Template

This template is for creating a website to track designs created by a UXD team. Built on Jekyll using GitHub pages, this template will enable you to quickly get up and running with a basic set of sortable and filterable tables, patterns for adding designs links and sharing stories from any issue tracking system.

View the [Changelog]()

----

## Local Development
Run the environment locally using the steps below:

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
1. Run the npm command `npm run site`

### Troubleshooting
If you are having issues with the site building, you can run two sets of clean commands:

- `gulp cleanVendors`
    - This will remove the vendor files that were copied over during the `gulp` process
- `npm run clean`
    - This will remove your node_modules directory, run `npm install`, run `gulp cleanVendors` to remove any old vendor files, and run `gulp` to copy updated vendor files.

If you have issues with your gem bundles, you can run the following command:
- `npm run bundle`
    - This will update the gem bundles. If you do not have node installed, just run `bundle update`.
