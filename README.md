# DataSciLabs Site

## Uma descrição do Projeto

## 1: Instalando o Blogdown

Apenas rode o seguinte comando no R

```
install.packages(‘blogdown’)
```

## 2: Clonando o projeto do git (Usando o RStudio)

File > New Project > Version Control > Git

Em Repository URL vai o link do repositório do GitHub, o nome e local do diretório fica à sua escolha

Feito isso o RStudio vai criar a pasta e clonar o repositório, e então na janelinha onde fica o Environment também vai aparecer a aba Git para trabalhar com o controle de versão

## 3: Configurando o Personal Access Token

Para trabalhar com o Git vai ser necessário configurar o PAT, apenas siga [essas instruções](https://docs.github.com/en/enterprise-server@3.6/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) e salve seu PAT em um local seguro, você só pode ver ele uma vez.

Agora é só colocar o PAT no RStudio, usando os seguintes comandos:

```
usethis::use_git_config(user.name = "SeuNome", user.email = "seu@email.com")

credentials::set_github_pat("seuPAT")
```

caso não haja o pacote usethis, basta:

```
install.packages(“usethis”)
```

Feito isso, o Git no RStudio deve estar funcionando perfeitamente.
