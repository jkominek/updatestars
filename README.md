# updatestars

Worried about people deleting git repos?

Want to ensure you've got a local copy?

This will do a passable job at solving the problem!

# insecure git

The latest version converts insecure git:// URLs into https:// at
clone time. But you might already have a bunch of existing repos
with now-unsupported URLs in them.

```
$ sed -i.bak "s,git://github.com,https://github.com,g" */*/config
```
