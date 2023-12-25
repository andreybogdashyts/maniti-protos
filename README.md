# maniti-protos

### Push tag
```
git tag v{version}
git push origin v{version}

Ex: version: 0.0.1
```

### Resolve ssh login issue

```
eval `ssh-agent -s`
ssh-add {name of private ssh key}
```

## Linux

### Install brew (package manager)

```
1. sudo apt update
2. sudo apt-get install build-essential
3. /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
4. (echo; echo 'eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"') >> /home/$USER/.bashrc
5. eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
```

### Install task
```
brew install go-task
```
### Insall Code generators
```
go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest
```

### Run Task
```
task generate
```

## Windows
### Run TaskFile
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