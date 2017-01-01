# Programando em Go: crie aplicações com a linguagem do Google

Repositório onde colocarei tudo o que for desenvolvido ao estudar o [livro] da Casa do Código.

## Como configurar o Go

* Adicionar um *alias* chamado **go** no arquivo *~/.bash_aliases* utilizando a imagem Docker *golang:alpine*
```sh
alias go='export WORKDIR=/go/src/github.com/danielfs/${PWD##*/} && docker run --rm -i -t -p 8080:8080 -v "$PWD":${WORKDIR} -w ${WORKDIR} golang:alpine go'
```

* Abrir uma nova sessão no terminal e executar *go version*, como abaixo:
```sh
daniel@danieltux:~$ go version
go version go1.7.4 linux/amd64
daniel@danieltux:~$
```

## Referências

* Utilizei este [artigo] do blog do Todd Rafferty como referência para adicionar o *alias*.

[livro]: <https://www.casadocodigo.com.br/products/livro-google-go>
[artigo]: <http://web-rat.com/posts/2016/09/06/compiling-go-for-alpine/>
