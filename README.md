## The change-maker website

[![Circle CI](https://circleci.com/gh/Joe8Bit/change-maker-website.svg?style=svg)](https://circleci.com/gh/Joe8Bit/change-maker-website)

http://change-maker.io

This repos contains the (currently very basic) website for the change make project. It is a static site that is generated using the static site generator [Harp](https;//harpjs.com). It is hosted on S3.

## Development

```
npm install -g harp
git clone https://github.com/Joe8Bit/change-maker-website.git
cd change-maker-website
harp server
```

## Compiling the site

The site is generated into the `./www` directory.

```
harp compile
```

## Deployment

The site is continuously deployed in the following way:

1. A commit happens on this repos `master` branch
2. The static site is built on [CircleCI](https://circleci.com/gh/Joe8Bit/change-maker-website)
3. CircleCI pushes the built assets to Amazon S3

## Contrubuting

All contributors will abide by the `CODE_OF_CONDUCT.md`.

## License

MIT
