heshed.github.io
==

# Refer

- https://gohugo.io/tutorials/automated-deployments/

# Setup

```bash
# install hugo
brew instal hugo

# create hugo site
hugo new site grace

# install theme
cd grace/themes
git clone https://github.com/aerohub/hugrid
git clone https://github.com/jnjosh/internet-weblog.git
git clone https://github.com/parsiya/Hugo-Octopress.git

cd ../..
echo grace/themes > .gitignore

# create first post
cd grace
hugo new about.md

# undraft
hugo undraft content/about.md

# 
echo grace/public >> ../.gitignore

echo "User-agent: *\nDisallow:" > static/robots.txt
```
