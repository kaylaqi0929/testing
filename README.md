# TS Charts Repo

This is an example charts repository.

### How It Works

I set up GitHub Pages to point to the `docs` folder. From there, I can
create and publish docs like this:

```console
$ helm create mychart
$ helm package mychart
$ mv mychart-0.1.0.tgz docs
$ helm repo index docs --url https://kaylaqi0929.github.io/testing
$ git add -i
$ git commit -av
$ git push origin master
```

From there, I can do a `helm repo add testing
https://kaylaqi0929.github.io/testing`
