# 🖥️ Comandos de Limpeza e Performance no Windows

## 🔧 Reparo de Sistema

    
- `dism /online /cleanup-image /restorehealth` → Corrige a imagem do sistema e complementa o SFC.
    
- `sfc /scannow` → Verifica e repara arquivos corrompidos do Windows.
- chkdsk /R C:
## 🌐 Rede e Internet

- `ipconfig /flushdns` → Limpa o cache DNS.
    
- `netsh int ip reset` → Restaura configurações de IP.
    
- `netsh winsock reset` → Corrige problemas de conexão.
    

## 🗑️ Limpeza de Arquivos Temporários

⚠️ **Atenção:** alguns comandos só funcionam no **CMD** e não no PowerShell.

- **CMD (Prompt de Comando):**
    
    cmd
    
    ```
    del /q /f /s %TEMP%\*
    del /q /f /s C:\Windows\Temp\*
    del /q /f /s C:\Windows\Prefetch\*
    ```
    
- **PowerShell (equivalentes):**
    
    powershell
    
    ```
    Remove-Item -Path $env:TEMP\* -Recurse -Force
    Remove-Item -Path "C:\Windows\Temp\*" -Recurse -Force
    Remove-Item -Path "C:\Windows\Prefetch\*" -Recurse -Force
    ```
    

## ⚡ Energia e Performance

- `powercfg -duplicatescheme e9a42b02-d5df-448d-aa00-03f14749eb61` → Ativa plano de energia “Desempenho Máximo”.
    
- `powercfg -h off` → Desativa hibernação e libera espaço.
    

## 🛍️ Outros úteis

- `wsreset.exe` → Limpa cache da Microsoft Store.
    
- `chkdsk /f` → Corrige erros no disco rígido.
    

## 📋 Observações Importantes

- Execute sempre como **Administrador**.
    
- Crie um **ponto de restauração** antes de alterações profundas.
    
- Alguns arquivos não serão apagados porque estão em uso — isso é normal.
    
- **CMD vs PowerShell:**
    
    - Parâmetros como `/q`, `/f`, `/s` funcionam apenas no **CMD**.
        
    - No **PowerShell**, use `Remove-Item` com `-Recurse` e `-Force`.