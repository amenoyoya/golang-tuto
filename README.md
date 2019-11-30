# Go言語｜入門

## Environment

- OS:
    - Windows 10
    - Ubuntu 18.04
- Editor:
    - VS Code

### Installation

#### on Windows 10
[Chocolatey](https://chocolatey.org/) を使うのが楽

`Win + X` |> `A` キー => 管理者権限PowerShell起動

```powershell
# install golang
> choco install golang
```

#### on Ubuntu 18.04
[最新の公式パッケージ](https://golang.org/dl/) をダウンロードしてインストールする

```bash
# install in home directory
$ cd ~

# download golang binary
$ wget -O - https://dl.google.com/go/go1.13.4.linux-amd64.tar.gz | tar zxvf -

# create symbolic link to /usr/local/bin/ => enable `go`, `gofmt` command
$ sudo ln -s ~/go/bin/go /usr/local/bin/go
$ sudo ln -s ~/go/bin/gofmt /usr/local/bin/gofmt

# confirm version
$ go version
go version go1.13.4 linux/amd64
```