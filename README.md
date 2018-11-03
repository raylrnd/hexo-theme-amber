<div align="right">Language: :us:<a title="Chinese" href="README.zh-CN.md">:cn:</a></div>

# Amber

[![Build Status][ci-badge]][ci-url]
[![GitHub Issues][issues-badge]][issues-url]
[![GitHub pull requests][pr-badge]][pr-url]
[![MIT License][license-badge]](LICENSE)

[ci-badge]: https://travis-ci.org/Mitscherlich/hexo-theme-amber.svg?branch=master
[ci-url]: https://travis-ci.org/Mitscherlich/hexo-theme-amber
[license-badge]: https://img.shields.io/badge/license-MIT-blue.svg
[issues-badge]: https://img.shields.io/github/issues/Mitscherlich/hexo-theme-amber.svg
[issues-url]: https://github.com/Mitscherlich/hexo-theme-amber/issues
[pr-badge]: https://img.shields.io/github/issues-pr/Mitscherlich/hexo-theme-amber.svg
[pr-url]: https://github.com/Mitscherlich/hexo-theme-amber/pulls


Hexo theme based on Vue.js and Bootstrap for [mitscherlich.me](https://mitscherlich.me).

![Preview](https://raw.githubusercontent.com/Mitscherlich/hexo-theme-amber/master/docs/assets/Preview.png)

> **⚠️ Note:** This theme cannot be use as a individual Vue.js spa. You need to setup a Hexo blog.

## Install

via this repo:

```bash
$ git clone https://github.com/Mitscherlich/hexo-theme-amber.git themes/amber
```

Then modify you `_config.yml`:

```yml
# ...
## Theme
theme: amber  # this enable your theme config
# ...
```

Enjoy your writing!

```bash
$ hexo clean && hexo serve
```

## Develop

This theme provide prebuild static assets on default branch. You may need to checkout [`master`](https://github.com/Mitscherlich/hexo-theme-amber/tree/master) branch if you want to custom the theme. There is no difference with Vue development you are familiar with:

```bash
$ git clone https://github.com/Mitscherlich/hexo-theme-amber.git -b master themes/amber-dev
$ cd themes/amber-dev && npm install # Also, yarn will be ok
```

Just follow the installation, but notice that you have to run both `hexo serve` and `yarn serve` at the same time. Otherwise you will not get the posts data.

```bash
$ cd /path/to/blog/theme/amber-dev
$ yarn serve
```

Then open another terminal:

```bash
$ cd /path/to/blog
$ hexo clean && hexo serve --port 4000
```

**Note:** hexo server must running on port `4000`. You may need to modifiy the `vue.config.js` under theme root if using other specific port.

## License

[MIT](LICENSE)
