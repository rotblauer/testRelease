# testRelease
it tests things and releases



get em

https://medium.com/@jgautheron/publish-your-golang-binaries-in-github-with-circleci-e0b64cb21bf8#.w8m4b47de

```
go get github.com/mitchellh/gox
go get github.com/tcnksm/ghr

```
Set up github token 

```
git config -global github.token "mah token"

```

```
gox -output dist/NAME_{{.OS}}_{{.Arch}}
ghr -u rotblauer v.x.x.xxx ./dist/
```