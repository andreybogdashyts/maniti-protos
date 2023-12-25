# maniti-protos

### Push tag
```
git tag v{version}
git push origin v{version}

Ex: version: 0.0.1
```

### Run TaskFile (windows)

#### Installations

##### Install scoop (command line installer)
```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

##### Install task
```
scoop install task
```

##### Generate task
```
task generate_windows
```

### Resolve issue with ssh

eval `ssh-agent -s`
ssh-add ab_github