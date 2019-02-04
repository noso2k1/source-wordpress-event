# source-wordpress-event
WordPress source for Gridsome with Tribe Events plugin fields

Based on @gridsome/source-wordpress plugin version 0.1.1

To install:

```npm install https://github.com/noso2k1/source-wordpress-event/tarball/master```
  
More info [here](https://stackoverflow.com/questions/13300137/how-to-edit-a-node-module-installed-via-npm)

## Usage

```
module.exports = {
  plugins: [
    {
      use: '@gridsome/source-wordpress-event',
      options: {
        baseUrl: 'WEBSITE_URL', // required
        apiBase: 'wp-json',
        typeName: 'WordPress',
        perPage: 100,
        concurrent: 10,
        routes: {
          post: '/:year/:month/:day/:slug',
          post_tag: '/tag/:slug'
        }
      }
    }
  ]
}
```

Refer to the [original project](https://github.com/gridsome/gridsome/tree/master/packages/source-wordpress) for additional information.


