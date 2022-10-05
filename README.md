# mkdocs-example-demo
Example of good open-source documentation for developers. 

If you find it tricky to keep on top of documentation between repositories - this guide should be helpful to resolve your documentation woes within your teams. 

Imagine different project teams with their own repositories contributing to a centralised document store; Frontend and backend co-existing in harmony, allowing new recruits to learn at a lightening fast pace etc.
## Prerequisite

### Resources used in this demo
### Technical:
- Ensure Docker is installed
- Ensure Python is installed
- Ensure NPM is installed


## What is MKdocs? 

To quote them: 

`MkDocs is a fast, simple and downright gorgeous static site generator that's geared towards building project documentation.`

## Why MKdocs and not Confluence/Gitbook/Github Page/Readme.io? 

To be consice it isn't a question of using one or the other but using them in conjuction with one another. 

However, I will list the pros and cons of Mkdocs as well as other documentation solutions.

### Mkdocs Pros

- Free and opensource, no monthly rising fees
- Lives closest to the source of truth - which is the repository
- Very flexible in terms of scripting and custom functionality
- Especially useful for poly repositories
- Can be deployed as a site (Netlify, Cloudfront etc.)
- Truly gives you a manual to your code base

### Mkdocs Cons

- Without docker it is tempermental in terms of python environments
- No GUI interfaces (requires markdown editor in code)
- Requires knowledge of Mkdocs documentation and associated plugins


### Pros and Cons of alternative solutions

- Confluence is great for higher level specifications (e.g. Product owners, stakeholders and customers)
- Github/Readme.io is great for an easy to use interface with fantastic editors
- The other solutions are fine and I'd still use them for specific use cases.

*However*,
- They become stale too quickly - an article written 5 months ago must be read with caution as it may no longer be factual.
- They are hard to manage, it is great when people write articles and documentation but maintenance is often neglected.


In this quick tutorial I want to show you the benefits of writing your documentation in MKDocs + plugins + vscode + drawio.


# Let's begin

```console
$ npm i -g meta
$ cd docs
$ docker-compose up -d
```

Visit http://localhost:8124 and continue the tutorial