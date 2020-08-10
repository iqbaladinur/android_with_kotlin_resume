[![Netlify Status](https://api.netlify.com/api/v1/badges/0d4dde1d-663c-4e7c-9beb-f8b1f8a7fee2/deploy-status)](https://app.netlify.com/sites/learnkotlinwithiqbal/deploys)

# Bloggy
> bloggy is minimum template for git based blog built with vue meta-framework nuxtjs, nuxt-content and tailwind css.

## Write Content
> using command line

```bash
# create-post will generate md file under folder structure bellow
$ npm run create-post -- your-post-title

# create-page will generate md file under folder strcuture bellow
$ npm run create-page -- your-page-title
```
> write content under this stucture.

    .
    ├── ...
    ├── content                 	# nuxt-content folder
    |   ├── page          		    # your static page
    │   |	├── home.md             # content
    │   |	└── ....md              # content
    │   └── post                    # your blog post
    │   	├── hello-world.md      # content
    │   	└── ....md              # content
    └── ...



## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project result on /dist
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

## LICENSE
[MIT License](./LICENSE)