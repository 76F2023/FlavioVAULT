## 🚶‍➡️Passos a seguir para configurar seu próprio repositório no GitHub


[](https://gist.github.com/aleduca/c5a22199d35d8e158cb4a187435d4171#%E2%80%8D%EF%B8%8Fpassos-a-seguir)

- Criar conta no [github](https://github.com/)
- Criar repositório privado no github
- Pegar link gerado e guardar
- Instale o [git](https://git-scm.com/downloads)
- Abra o terminal
- [[#✉️Configure o name e email]]
    - Email tem que ser o mesmo do github
- Instalar a extensão no obsidian
- Vai dizer que ainda tem que configurar
- Abra seu terminal novamente
- Vá até onde está seu cofre
- [[#💻Iniciar repositório local e enviar para o remoto]]
- Voltar para o obsidian e entrar nas configurações da extensão
- Colocar name e email e tempo de intervalo de envio.
- Se quiser posso mandar manualmente através da próprio extensão que fica na sidebar direita.
- Posso baixar o vault direto pelo github quando quiser usar ele em outro computador.

#### ✉️Configure o name e email

[](https://gist.github.com/aleduca/c5a22199d35d8e158cb4a187435d4171#%EF%B8%8Fconfigure-o-name-e-email)

```shell
git config --global user.name "Seu nome"
git config --global user.email seuemail-da-conta-do-github
git config --list 👉para ver se está configurado certo
```

#### 💻Iniciar repositório local e enviar para o remoto

[](https://gist.github.com/aleduca/c5a22199d35d8e158cb4a187435d4171#iniciar-reposit%C3%B3rio-local-e-enviar-para-o-remoto)

```shell
git init 👉 Inicia repositório local
git remote add origin git@github.com:aleduca/obsidian.git 👉 liga co repositório local com o remoto - foi gerado pelo github ao criar o repositório remoto.
git add . 👉 Prepara para enviar com as modificações
git commit -m "Primeiro commit" 👉 Mensagem que vai aparecer no github
git push origin master 👉 Envia para o repositório remoto
```