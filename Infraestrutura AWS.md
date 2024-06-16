# IAAS x PAAS x SAAS

Infraestrutura as a Service: 

* Computação cloud é exemplo de infraestrutura como Serviço - onde os provedores disponibilizam toda a Infraestrutura por meio da nuvem, e o cliente cria os recursos sob demanda sempre e somente quando precisar, não precisando se preocupar com questões de infraestrutura física.

Platform as a Service:

* A solução PaaS permite ao usuário desenvovler, executar e gerenciar aplicações sem o trabalho de criar e manter a infraestrutura ou plataforma que normalmente está associada a esses processos. O objetivo é se preocupar somente com o código. 

> Ex.: _AWS Elastic BeanStalk._

Software as a Service:

* A solução de SaaS consiste em ser disponibilizado o Software como Serviço, ou seja, o cliente não precisa se preocupar em manter o software nem gerenciar atualizações, economizando tempo e esforço. 

> Ex.: _Google Drive, Dropbox, Salesforce, Slack, Zoom._

# Modelo de Resposabilidade Compartilhada

* Segurança da Nuvem:

A AWS é responsável por proteger a infraestrutura que executa todos os serviços oferecidos na Nuvem AWS. Essa infraestrutura é composta por hardware, software, redes e instalações que executam os Serviços de nuvem AWS.

* Segurança na Nuvem:

A responsabilidade do cliente será determinada pelos Serviços de nuvem AWS selecionados por ele. Isso determina a quantidade de operações de configuração que o cliente deverá executar como parte de suas responsabilidades de segurança.

# Infraestrutura Global da AWS

Regiões:

Uma Região é um local físico em todo o mundo onde são agrupados os datacenters - Zonas de Disponibilidade.

Cada região da AWS consiste no mínimo em três AZs isoladas e separadas fisicamente em uma área geográfica. As regiões de infraestrutura da AWS atendem aos mais altos níveis de segurança, conformidade e proteção de dados.

Zonas de Disponibilidade:

É um ou mais datacenters distintos com energia, rede e conectividade redundantes em uma região da AWS.

Características:

Todo o tráfego entre as AZs é criptografado;

Todas as AZs em uma região da AWS estão interconectadas por redes de alta largura de banda e baixa latência, usando fibra metropolitana dedicada e totalmente redundante para proporcionar redes de alto throughput e baixa latência entre AZs;

As AZs são fisicamente separadas por uma distância significativa (vários quilômetros) das outras AZs.

# AWS Well-Architected Framework

O AWS Well-Architected Framework ajuda a entender os prós e contras das decisões que você toma ao criar sistemas na AWS. Ao usar o framework, você terá acesso à práticas recomendadas de arquitetura para projetar e operar sistemas confiáveis, seguros, eficientes, econômicos e sustentáveis na nuvem.

# Serviço DNS / Amazon Route 53

O que é um "Domínio"?

* O domínio serve para localizar e identificar conjuntos de computadores e serviços na Internet. O nome de domínio foi concebido com o objetivo de facilitar a memorização desses endereços, pois sem ele, teríamos que memorizar uma sequência grande de números, e dar flexibilidade para que o operador desses serviços altere sua infraestrutura com maior agilidade.

E também é sua identidade!

> Ex.: _www.google.com_, _ada.tech_.

# DNS

O DNS (Domain Name System - Sistema de nome de domínio) converte nomes de domínio legíveis por humanos (por exemplo, www.amazon.com) em endereços IP legíveis por máquina (por exemplo, 192.0.2.44).

* Principal comando:
```sh
nslookup <nomedodominio.com>
```

Este comando é utilizado para _consultar servidores DNS_ para obter informações sobre registros de DNS, como endereços IP associados a nomes de domínio ou informações sobre servidores de nomes. Este comando é amplamente utilizado para diagnósticos de rede e resolução de problemas relacionados à tradução de nomes de domínio em endereços IP e vice-versa.

* Amazon Route 53

O serviço de DNS oferecido pela AWS é o Amazon Route 53, altamente disponível e escalável. Ao utilizá-lo, é possível criar entradas apontando para serviços da AWS, como instâncias EC2, Load Balancer, entre outros.

