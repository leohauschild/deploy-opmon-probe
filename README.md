# Instalação Opmon probe com Ansible

Projeto usando Ansible para automatizar a instalação de uma probe do sistema de monitoramento Opmon. 

Sistema de monitoramento Opmon, Links para conhecê-lo:
https://www.opservices.com.br/
https://www.opservices.com.br/monitoramento-real-time/


## O que foi utilizado utilizadas:

- Centos Stream 8 (SO compatível com o sistema de monitoramento)
- 2 VMs rodando em ambiente virtualizado VMware: 
  - Master: VM principal onde roda o sistema de monitoramento
  - Probe: VM que fará a coleta de informações de uma rede externa (filial, ou alguma rede com alta latência.)
- Ansible

## Como que funciona?

O funcionamento é simples tendo em vista que o Master já esteja com a sua configuração totalmente operante. Desta forma é necessário apenas ajustar as variáveis que estão no arquivo "install-opmon-probe/group_vars/all". Com isso feito é só rodar o playbook "install.yml".

