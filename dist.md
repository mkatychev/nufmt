Steps for `dist` release of `nufmt`:

```sh-session
$ dist init
$ git --all -m 'ci: `dist init`'
```

Add windows ARM workaround:
https://github.com/abrauninger/nufmt/blob/60dfd82a6b21417912e64d3ebd05f0509005e50e/dist-workspace.toml#L19-L20



```sh-session
$ git remote add mkatychev https://github.com/mkatychev/nufmt
$ git commit --all -m 'doc: dist.md'
$ git tag v0.1.4
$ git push mkatychev fix-extra-rest:main
$ git push --tags mkatychev
```
