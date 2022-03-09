# INFRAESTRUTURA E SERVIÇOS DE REDES

## Dados da equipe e do professor

```
Dupla: Tayllane Barbosa Santos
       Wildimyla Karolayne Dantas de Oliveira Leite
Turma: 924
Professor: Alaelson Jatobá
```

## Implementação dos servidores Samba e DNS Master

### Objetivo: 

Fazer a instalação dos servidores Samba e DNS Master, bem como a implementação do ip do ns1 no Windowa para acessar os arquivos do samba pelo nome e não somente pelo ip. 

#### Samba

* É um software usado para Linux e também outros sistemas derivados de Unix, é usado para compartilhar e administrar os recursos nas redes que são formadas por máquinas com Windows. Dessa maneira possibilita o uso de Linux como servidor de impressão e de arquivos além de vários outros.


#### DNS 

* O DNS Master e o DNS Slave são servidores responsáveis por fazer a tradução dos nomes dos sites que são pesquisados nos navegadores para os endereços IPs desses sites. No momento só será abordado a instalação e configuração do DNS Master.


## Definições de rede

   * Antes de tudo é preciso definir duas tabelas: uma com as definições de ips usados e outra com os domínios a serem utilizados também.

```
Tabela 1: Definições da rede interna

--------------------------------
|  DESCRICAO  |  IP            |
--------------------------------
| rede        | 10.9.24.121    |
| máscara     | 255.255.255.0  |
| Gateway     | 10.9.24.1      |
| Broadcast   | 10.9.24.255    |
| Samba-SRV   | 10.9.24.121    |
| NameServer1 | 10.9.24.121    |
| NameServer2 | 10.9.24.124    |
--------------------------------
```      

OBS: na tabela acima estão os nameservers 1 e 2, DNS Master e o Slave, respectivamente. Como a instalação será do DNS Master, apenas será utilizado o nameserver 1 e seu ip correspondente. 

```
Tabela 2: Nomes FQDN dos hosts


|      Apelido      |               NOME                                     |
|:------------------|:-------------------------------------------------------|
| gateway (gw)      | gw.tayllanewildimyla924.labredes.ifalarapiraca.local   |
| nameserver1 (ns1) | ns1.tayllanewildimyla924.labredes.ifalarapiraca.local  |
| nameserver2 (ns2) | ns2.tayllanewildimyla924.labredes.ifalarapiraca.local  |
| vm da dupla (vm2) | vm2.tayllanewildimyla924.labredes.ifalarapiraca.local  |
| vm1               | ns1.tayllanewildimyla924.labredes.ifalarapiraca.local  |
| samba             | ns1.tayllnewildimyla924.labredes.ifalarapiraca.local   |
```
### Configuração do SAMBA

* Para realizar a configuração de um servidor de arquivos com Samba, 

### Configuração do Bind9 (DNS Master)

* Para realizar a configuração os servidores DNS Master, 
