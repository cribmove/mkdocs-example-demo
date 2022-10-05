# Welcome

You have successfully started mkdocs.

## Tutorial 1.1 Creating a new file in the root directory

1. Create a new file called `example.md` in the root docs folder either through your code editor or console:

```console
$ cd docs
$ echo 'testing' > example.md
```

2. Update the root mkdocs.yml's Nav  to the following:

```yaml
nav:
  - Intro: 'index.md'
  - Example: 'example.md'
```

The mkdocs.yml always looks for the closest sibling docs folder by default.

After saving you should see the new article [> here <](http://localhost:8123/example/). Once you have visited return to this page.

## Tutorial 1.2 Linking Mkdocs.yml files

I have already created the sub folders and initialised mkdocs within them (by using `mkdocs new .`). We just have to link them to the root mkdocs.yml

Simply add the following to your mkdocs.yml navigation (Nav:)

```yaml
nav:
  - Intro: 'index.md'
  - Example: 'example.md'
  - SubPages: '*include ./example-subpage/*/mkdocs.yml'

```

So now you have linked subfolders - useful for monorepos.


## Tutorial 1.3 Linking an entirely separate repository

Let's do an example where you want to have another repository added to your centralised documentation. Simply modify the root mkdocs.yml of this repo to read as follows:

In the root repository run:
```console
$ meta git update
```

```yaml
nav:
  - Intro: 'index.md'
  - Example: 'example.md'
  - SubPages: '*include ./example-subpage/*/mkdocs.yml'
  - External Repository: '*include ./second-repo/mkdocs.yml'
```

!!! note

    In a real-world application you would have the external repository outside of the root directory and not as a sub folder as shown in this example.

## That concludes the basic tutorial

So you can now document various parts of your application, collaborate with other repositories that utilise Mkdocs. Cartman says it best:

<div class="tenor-gif-embed" data-postid="21268967" data-share-method="host" data-aspect-ratio="1.77778" data-width="100%"><a href="https://tenor.com/view/we-need-to-work-together-eric-cartman-kenny-mccormick-south-park-s11e7-gif-21268967">We Need To Work Together Eric Cartman GIF</a>from <a href="https://tenor.com/search/we+need+to+work+together-gifs">We Need To Work Together GIFs</a></div> <script type="text/javascript" async src="https://tenor.com/embed.js"></script>

## Wait, is that it? 

NO! If you want to see other amazing features click the following:

### Using draw.io for diagrams 
[>Click Here< for draw IO Tutorial](./diagram.io.md)


### Using Mermaid for amazing project design

[>Click Here< for mermaid Tutorial](./mermaid.md)


### Openapi Example

[>Click Here< for openapi Tutorial](./openapi.md)