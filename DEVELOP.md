# Initial Setup

Create a directory for caching gems needed by Jekyll:

```
mkdir -p $HOME/jekyll/gem
```

Install the Jekyll container:

```
docker pull jekyll/jekyll
```

# Start Local Jekyll Server

Run a shell in the container from the repository root directory:

```
docker run --rm --volume=$PWD:/srv/jekyll --volume=$HOME/jekyll/gem:/usr/gem --publish 4000:4000 -it jekyll/jekyll /bin/bash
```

In the container shell:

```
PAGES_REPO_NWO=tree-ware/tree-ware.github.io jekyll serve --incremental
```

Open: http://localhost:4000

The server rebuilds the pages whenever a source file changes.

Refresh the browser after a few seconds to see the changes.
