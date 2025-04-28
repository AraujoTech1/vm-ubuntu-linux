
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=azure" width="180" />
  </a>
</p>

---

<h1 align="center">VM Ubuntu Linux em Cloud</h1>

Este projeto visa a criação e configuração de uma **máquina virtual Ubuntu 24.04 LTS** na plataforma **Azure**. O objetivo principal é fornecer um ambiente de desenvolvimento **Linux** acessível remotamente **via SSH**. A VM foi criada para ser usada como um ambiente de aprendizado e para implementar aplicativos, com a configuração de segurança e rede padrão para ambientes de produção.
A máquina virtual foi configurada usando o **Azure for Students**, e está configurada para ser acessada por meio de chave SSH, com um **endereço IP público** atribuído. O sistema operacional utilizado é o **Ubuntu 24.04 LTS**, uma distribuição Linux popular para servidores.

---

## Funcionalidades 
- Criação e configuração de uma **máquina virtual** com Ubuntu no **Azure**.
- Acesso remoto via **SSH** com segurança configurada através de **chaves SSH**.
- **Configuração de rede** e atribuição de **endereço IP público**.
- Possibilidade de expandir a configuração com **discos adicionais** e **aplicações de segurança**.

---

## Testes de Software
Os testes realizados incluem:
1. **Teste de Conexão SSH**:
   - Verificação da conectividade da máquina local com a VM no Azure usando a chave SSH.
   - **Resultado**: Conexão bem-sucedida, acesso ao terminal da VM.
   
2. **Teste de Desempenho**:
   - Execução de comandos simples para avaliar o desempenho da VM.
   - **Resultado**: Respostas rápidas e confiáveis.

3. **Teste de Segurança**:
   - Configuração de **Firewall** para garantir que apenas a porta SSH (22) está aberta para acessos externos.
   - **Resultado**: Acesso controlado via SSH e bloqueio de acessos indesejados.
---
 
## Tecnologias  

- ![Azure Badge](https://img.shields.io/badge/Microsoft_Azure-555555?style=flat-square&logo=microsoft-azure)  - Plataforma de cloud
- ![Ubuntu Badge](https://img.shields.io/badge/Ubuntu-555555?style=flat-square&logo=ubuntu)  - Sistema operacional que foi criado
- ![SSH Badge](https://img.shields.io/badge/SSH-555555?style=flat-square&logo=ssh)  - Protocolo para acessar a VM
- ![Git Bash Badge](https://img.shields.io/badge/Git_Bash-555555?style=flat-square&logo=gitbash)  - Ferramentas para conectar via SSH


---

## Pré-requisitos e Instalações
1. Conta no **Azure**.
2. **Git Bash** ou **PowerShell** instalado no computador local.
3. **Chave SSH** gerada durante a criação da VM.

---

## Instruções de Uso
1. **Acesse o portal do Azure** e crie uma máquina virtual Ubuntu.
2. Baixe e salve a chave privada SSH gerada durante a criação da VM.
3. Abra o **Git Bash** ou **PowerShell** e navegue até o diretório onde a chave SSH foi salva.
4. Conecte-se à VM com o comando:
   ```bash
   ssh -i "caminho/para/sua/chave_privada" azureuser@<IP_PUBLICO_DA_VM>
5. Após a conexão, você estará dentro da VM e poderá executar comandos Linux.
   
