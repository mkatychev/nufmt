Steps for `dist` release of `nufmt`:

```sh-session
$ dist init
$ git --all -m 'ci: `dist init`'
$ git remote add mkatychev https://github.com/mkatychev/nufmt
$ git commit --all -m 'doc: dist.md'
$ git tag v0.1.4
$ git push mkatychev fix-extra-rest:main
$ git push --tags mkatychev
```
