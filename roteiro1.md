# Roteiro 1
## Objetivo
- Entender os conceitos básicos sobre uma plataforma de gerenciamento de hardware.
- Introduzir conceitos básicos sobre redes de computadores.
## Montagem do roteiro
### Tarefa 1: Instalar o MaaS
O MaaS um software de código aberto e suportado pela Canonical. O MAAS trata servidores físicos como máquinas virtuais ou instâncias na nuvem. 
Esse software possui diversas versões, mas para esse projeto iremos utilizar a versão stable 3.5.3.

Primeiro atualizamos os pacotes do sistema:

```sudo apt update && sudo apt upgrade -y```
   
Em seguida fazemos a instalação:

```
sudo snap install maas --channel=3.5/stable
sudo snap install maas-test-db
```

Ainda conectado a máquina local pelo cabo Ethernet podemos acessar a máquina main através da nossa máquina pessoal utilizando o SSH:

```
ssh cloud@172.16.0.3
```
