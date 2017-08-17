
# Index

The index is a text file that list plugins, each consisting of the following fields:

```
name
url
plugin description
one or more tags
author
```

For example:

```
fishtape
https://github.com/fisherman/fishtape
TAP producer and test harness
test tap harness runner
bucaran
```

The index powers the [online] search.

## Adding plugins to this list

Create a pull request in this repository.

```bash
git clone https://github.com/argos-scripts/index
cd index
echo -e "$name\n$url\n$info\n$tags\n$author\n" >> index
git push origin master
```

## Test coverage

- [x] Index integrity
- [x] Uniqueness of plugin/prompt name
- [ ] Description
- [x] Integrity of URL
- [x] Uniqueness of URL
- [x] Uniqueness of tags within a plugin/prompt
- [x] Tags are shorter no more than 15 characters
- [x] No more than 4 tags per plugin
- [ ] Author.

## Disclaimer

All the plugins listed in this index are property of their respective owners. Follow the provided URL and see the bundled LICENSE or COPYING file for copyright information.

[online]: https://argos-scripts.github.io
