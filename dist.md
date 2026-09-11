Steps for `dist` release of `nufmt`:

```sh-session
$ dist init
$ git --all -m 'ci: `dist init`'
```

Add windows ARM workaround:
https://github.com/mkatychev/nufmt/blob/067eb8b55a8167a2b01ad9e8ba2e3bff4ef7f4aa/dist-workspace.toml#L19-L20



```sh-session
$ git remote add mkatychev https://github.com/mkatychev/nufmt
$ git commit --all -m 'doc: dist.md'
$ git tag v0.1.4
$ git push mkatychev fix-extra-rest:main
$ git push --tags mkatychev
```
