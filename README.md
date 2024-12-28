# Phishing-com-o-Kali-Linux
Este repositório é para um desafio de Phishing utilizando o Kali Linux para a captura de credenciais **(usuários e senhas)**

## Ferramenta Utilizada
- **setoolkit**

## Passo a Passo

1. Acesso ao root: Antes de começar, certifique-se de acessar o usuário root com o comando:
   ```bash
   sudo su
   ```
2. Iniciando o setoolkit: No terminal, execute o comando:
   ```bash
   setoolkit
   ```
   Escolha a opção de **Social-Engineering Attacks** no menu principal.
   
3. Selecionando o Vetor de Ataque: Opte pelo vetor de ataque **Website Attack Vectors**.

4. Escolhendo o Método: Escolha a opção **Credential Harvester Attack Method** e selecione a opção para clonar um site.
   
5. Clonando o Site: Durante o desafio, utilizamos o **Facebook** como exemplo de site a ser clonado. Colocar a URL do site a ser clonado quando solicitado.
   
6. Obtendo o Endereço IP: Para capturar o endereço IP da máquina (necessário para configurar o phishing), use o comando:
   ```bash
   ifconfig
   ```
   Copie o endereço IP e insira-o no navegador para testar o ataque.
   
7. E nisso informe as credencias no formulário que está sendo solicitado ao fazer sua requisição, será retornado no terminal
   ![Imagem de exemplo](Screenshot_9.png)
![Imagem de exemplo](Screenshot_10.png)

OBS: Podemos ter dificuldades na parte de requisição do navegador e ao servidor local, então podemos utilizar o curl:
 ```bash
   curl -X POST -d "email=teste@tste.com&passwordteste2" http://192.168.18.160
   ```
---
