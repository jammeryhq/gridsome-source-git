<div align="center">

<a href="https://www.jammeryhq.com" title="JammeryHQ" target="_blank">

  <img src="https://jammeryhq.com/jammeryhq.png" width="128" />
  
</a>

<p>
Fast-track your JAMstack development & learning
</p>
</div>

<hr />

# About this plugin

Gridsome source to fetch data from a remote git repository.

## Installation

```bash
npm install --s @noxify/gridsome-source-git
```

## How to use

```js
//gridsome.config.js

module.exports = {
  plugins: [
    {
      use: '@noxify/gridsome-source-git',
      options: {
        remote: 'https://github.com/noxify/test.git',
        target: 'git-source/noxify-test/',
        typeName: 'GitPost',
        route: '/gitpost/:id'
      }
    }
  ]
}
```

## Documentation

You can find the complete documentation here: https://webstone.info/documentation/gridsome-source-git

## Credits

This is a port from Gatsby: https://github.com/stevetweeddale/gatsby-source-git
But extended to enable the clone of private git repositories.
