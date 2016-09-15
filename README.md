heshed.github.io
==

# Refer

- https://gohugo.io/tutorials/automated-deployments/

# Setup

```bash
# install hugo
brew install hugo

# create hugo site
hugo new site heshed.github.io

# install theme
cd themes
git clone https://github.com/parsiya/Hugo-Octopress.git

cd ../..
echo themes > .gitignore

# create first post
hugo new about.md

# undraft
hugo undraft post/about.md

# 
git submodule add https://github.com/heshed/heshed.github.io.git public

echo "User-agent: *\nDisallow:" > static/robots.txt
```

# deploy to https://heshed.github.io

```bash
sh deploy.sh
```
