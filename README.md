# Noelle Reed's Blog

## Cloning and Running

```shell
git clone --recursive https://github.com/Kobilian98/blog.git
cd blog

# If you have an existing clone
git submodule update --init
```

Next to build the site

```shell
cd noellereedblog
hugo build
```

To make changes to public

```shell
cd noellereedblog/public
git add .
git commit -m "I updated the site with <some> feature/content."
git push

# Now we have to make sure the main repository is pointing at the correct version of public.
cd ../..
git add .
git commit -m "I updated the site with <some> feature/content."
git push
```

To serve the site locally

```shell
cd noellereedblog
hugo serve
```