
<center> Máquina Virtual Ubuntu no Azure </center>

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=azure" />
  </a>
</p>


## Descrição do Projeto
Este projeto visa a criação e configuração de uma **máquina virtual Ubuntu 24.04 LTS** na plataforma **Microsoft Azure**. O objetivo principal é fornecer um ambiente de desenvolvimento Linux acessível remotamente via SSH. A VM foi criada para ser usada como um ambiente de aprendizado e para implementar aplicativos, com a configuração de segurança e rede padrão para ambientes de produção.

A máquina virtual foi configurada usando o **Azure for Students**, com uma assinatura gratuita, e está configurada para ser acessada por meio de chave SSH, com um **endereço IP público** atribuído. O sistema operacional utilizado é o **Ubuntu 24.04 LTS**, uma distribuição Linux popular para servidores.

## Funcionalidades do Projeto
- Criação e configuração de uma **máquina virtual** com Ubuntu no **Azure**.
- Acesso remoto via **SSH** com segurança configurada através de **chaves SSH**.
- **Configuração de rede** e atribuição de **endereço IP público**.
- Possibilidade de expandir a configuração com **discos adicionais** e **aplicações de segurança**.

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

4. **Captura de Teste**:
   - Captura de comandos e saídas realizadas durante os testes de conexão SSH.

## Tecnologias e Linguagens
- **Microsoft Azure** (Plataforma de cloud)
- **Ubuntu 24.04 LTS** (Sistema operacional)
- **SSH** (Protocolo para acessar a VM)
- **PowerShell** / **Git Bash** (Ferramentas para conectar via SSH)

## Bibliotecas e Frameworks
- Nenhum framework ou biblioteca adicional foi necessário para este projeto.

## Pré-requisitos e Instalações
1. Conta no **Azure for Students**.
2. **Git Bash** ou **PowerShell** instalado no computador local.
3. **Chave SSH** gerada durante a criação da VM.

## Instruções de Uso
1. **Acesse o portal do Azure** e crie uma máquina virtual Ubuntu.
2. Baixe e salve a chave privada SSH gerada durante a criação da VM.
3. Abra o **Git Bash** ou **PowerShell** e navegue até o diretório onde a chave SSH foi salva.
4. Conecte-se à VM com o comando:
   ```bash
   ssh -i "caminho/para/sua/chave_privada" azureuser@<IP_PUBLICO_DA_VM>
