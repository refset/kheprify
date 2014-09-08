kheprify
========

A Browserify transform for easily integrating the [Khepri](https://github.com/mattbierner/khepri) language into your projects.

This code is mainly hacked together from `coffeeify` (thanks!).

usage
=====

Install kheprify into your app:

```
$ npm install kheprify
```

When you compile your app, just pass `-t kheprify` to browserify:

```
$ browserify -t kheprify foo.kep > bundle.js
$ node bundle.js
555
```

you can omit the `.kep` extension from your requires if you add the extension to browserify's module extensions:

```
$ browserify -t kheprify --extension=".kep" foo.kep > bundle.js
```
