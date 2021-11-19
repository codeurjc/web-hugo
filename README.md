# Website for CodeURJC built with Hugo

## Development

In order to locally start a server to compile and host the website, issue the following command that will run a Docker container and expose the website at http://localhost:1313/:

```
docker run --rm -it \
  -v $(pwd):/src \
  -p 1313:1313 \
  klakegg/hugo:latest-ext \
  server
```

For building extended Hugo is needed, hence the @latest-ext@ tag, which stands for latest extended hugo version.

## Production

In order to publish this site through GitHub Pages, follow the steps in the [official Hugo documentation](https://gohugo.io/hosting-and-deployment/hosting-on-github/).