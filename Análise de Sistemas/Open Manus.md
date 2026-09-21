[FoundationAgents/OpenManus: No fortress, purely open ground. OpenManus is Coming.](https://github.com/FoundationAgents/OpenManus/tree/main)

Estou tentando criar um ambiente virtual porém o CMD responde que não conhece esse comando.

O comando que você tentou (`uv venv --python 3.12`) não existe no **CMD do Windows**. Esse formato parece vir de instruções para Unix/macOS ou de ferramentas específicas que não estão instaladas no seu sistema.

No Windows, para criar e ativar um ambiente virtual em Python 3.12, você deve usar:

### Passo 1 – Criar o ambiente virtual

No CMD ou PowerShell:

Código

```
python -m venv .venv
```

> Certifique-se de que o Python 3.12 está instalado e acessível pelo comando `python --version`.

### Passo 2 – Ativar o ambiente

No **CMD**:

Código

```
.venv\Scripts\activate
```

No **PowerShell**:

Código

```
.venv\Scripts\Activate.ps1
```

No **Git Bash** (ou similar):

Código

```
source .venv/Scripts/activate
```

### Passo 3 – Conferir se deu certo

Depois de ativar, o prompt deve mostrar algo como:

Código

```
(.venv) C:\Users\Flavio\projeto>
```

👉 Se o CMD disser que não conhece o comando, provavelmente o Python não está no PATH. Nesse caso, você precisa instalar o Python 3.12 e garantir que a opção **“Add Python to PATH”** esteja marcada na instalação.

Quer que eu te mostre como verificar se o Python está corretamente instalado e disponível no CMD?
