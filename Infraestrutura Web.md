# O que é Infraestrutura Web?

Infraestrutura web é um conjunto de tecnologias e recursos necessários para suportar a operação de sites e aplicações na internet. Inclui hardware, software, redes, bancos de dados, servidores, entre outros componentes, necessários para disponibilizar conteúdo e serviços na web.

# Principais características:

* Escalabilidade: Precisa ser capaz de suportar um grande número de usuários e aumentar sua capacidade conforme a demanda cresce;

* Confiabilidade: Deve ser confiável e estar disponível a maior parte do tempo, para que os usuários possam acessar o conteúdo e os serviços;

* Segurança: Precisa ser segura, protegendo os dados dos usuários e evitando ataques de hackers e outras ameaças;

* Desempenho: Deve ter um desempenho adequado para suportar a carga de tráfego e manter a rapidez na entrega de conteúdo e serviços;

* Flexibilidade: Deve ser flexível para atender às necessidades dos usuários e adaptar-se às mudanças de demanda;

* Descentralização: Seus componentes físicos e virtuais estão espalhados ao longo do planeta e até no espaço, em comunicação via satélite.

# Infraestrutura Física e Virtual

* Infraestrutura Física:

A Infraestrutura Física inclui os servidores, equipamentos de rede e outros dispositivos que são instalados em um datacenter ou local físico.

* Infraestrutura Virtual:

A Infraestrutura Virtual inclui serviços de nuvem, como a Amazon Web Services (AWS), Microsoft Azure, Google Cloud Platform, entre outros, que oferecem recuros de infraestrutura virtual sob demanda. Tais serviços são popularmente conhecidos como "nuvens públicas", uma vez que para ter acesso, você só precisa de uma assinatura, sem nenhum tipo pré-requisito específico.

# Sistemas Operacionais para Servidores Web

Para servidores web, a escolha do sistema operacional é uma decisão crucial, pois afeta a segurança, desempenho, escalabilidade e facilidade de gerenciamento. Aqui estão alguns dos sistemas operacionais mais comuns usados para servidores web:

```sh
Windows Server
```

* Vantagens: Integração com produtos Microsoft, suporte técnico oficial robusto, interface gráfica amigável para administração, compatibilidade com software corporativo da Microsoft.

* Desvantagens: Licenciamento pago, requer mais recursos de hardware em comparação com Linux, menos flexibilidade em alguns cenários de automação avançada.

```sh
Linux
```

* Vantagens: Alta estabilidade, segurança robusta, ampla compatibilidade com softwares de servidor, ampla comunidade de suporte, atualizações frequentes e gratuitas, facilidade de automação (scripts, configuração via linha de comando).

* Desvantagens: Alguma curva de aprendizado para administradores sem experiência em Linux, especialmente na configuração inicial.
```sh
Container OS (como CoreOS, RancherOS):
```

* Vantagens: Projetados para rodar containers, eficientes em termos de recursos, fácil escalabilidade, atualizações automatizadas, ideal para arquiteturas baseadas em microservices.

* Desvantagens: Pode ter uma curva de aprendizado para implementar e gerenciar containers se você não estiver familiarizado com essa tecnologia.

# Web Servers

Um servidor web é um software que opera em um servidor e é responsável por receber solicitações HTTP de clientes (navegadores da web ou outras aplicações) e enviar as respostas correspondentes, geralmente páginas web ou outros recursos como imagens, vídeos, arquivos, etc. Existem diversos servidores web populares, cada um com suas características e finalidades específicas:

Apache HTTP Server:

* É um dos servidores web mais antigos e amplamente utilizados.
* Open source e gratuito.
* Suporta uma ampla gama de módulos e extensões.
* Robusto e estável, com boa documentação e suporte da comunidade.

Nginx:

* Conhecido pela sua eficiência e alto desempenho, especialmente em servir conteúdos estáticos.
* Também pode ser usado como proxy reverso e balancer de carga.
* Open source e gratuito.
* Ganhou popularidade significativa devido ao seu consumo reduzido de recursos em comparação com o Apache em certos cenários.

Microsoft IIS (Internet Information Services):
* Desenvolvido pela Microsoft para o sistema operacional Windows Server.
* Suporta várias tecnologias Microsoft como ASP.NET, .NET Core, e outros.
* Integração nativa com outros produtos Microsoft como Active Directory.
* Pode ser configurado tanto para hospedar sites estáticos quanto dinâmicos.

LiteSpeed Web Server:
* Conhecido por seu alto desempenho e eficiência no uso de recursos.
* Focado em ambientes de alta carga e performance exigente.
* Oferece uma versão gratuita com funcionalidades limitadas e uma versão paga com mais recursos e suporte.

Apache Tomcat:
* Mais especificamente um servidor de aplicação web, projetado para executar aplicações Java Servlet e JSP.
* Popular para hospedar aplicações web Java, especialmente em ambientes corporativos.
* Cada servidor web tem suas próprias características, pontos fortes e fracos, e é importante escolher o mais adequado para as necessidades específicas do projeto. Fatores como desempenho, escalabilidade, suporte a tecnologias específicas (como PHP, Java, .NET, etc.), requisitos de segurança e facilidade de administração são todos considerações importantes na escolha do servidor web correto.

# Qual Escolher?

```sh
Depende!
```
A escolha do servidor web dependerá das necessidades e objetivos do projeto. Se você procura estabilidade e flexibilidae, porém deseja simplicidade na configuração, o Apache pode ser a opção ideal. Entretanto, se sua aplicação tiver um volume muito grande de acessos e você se sente confiante para executar configurações mais complexas, o NGINX atenderá sua necessidade. 

# Banco de Dados para Infraestrutura Web

* Banco de Dados Relacional

Os bancos de dados relacionais são os mais populares e amplamente utilizados em aplicações web. Eles utilizam a linguagem SQL para consultar e manipular dados. 
São compostos por tabelas, que são organizadas em linhas e colunas, e estabelecem relações entre elas. Alguns exemplos de bancos de dados relacionais incluem MySQL, PostgreSQL e Oracle.

* Banco de Dados Não-Relacional

Tecnologia mais recente. É uma alternativa aos bancos de dados relacionais, projetados para lidar com grandes quantidades de dados não estruturados. Eles não utilizam a linguagem SQL e não possuem esquema fixo, o que permite maior flexibilidade na estruturação dos dados. Alguns exemplos de bancos de dados NoSQL incluem MongoDB, Cassandra e Redis.

# Protocolo HTTP

A sigla HTTP significa "Hypertext Transfer Protocol" e descreve um protocolo no qual os dados podem ser transmitidos em uma rede IP tanto interna quanto pública (Internet);

Sua principal usabilidade é a transferência de páginas da Internet e dados entre um servidor web e um navegador. No entanto, ele não está restrito a sites, sendo usado, por exemplo, para aplicativos de smartphone;

As respostas HTTP incluem informações como o status da solicitação, os dados do recurso solicitado e cabeçalhos de resposta que fornecem informações adicionais sobre a resposta;

O protocolo HTTP não é criptografado e envia todas as informações em texto aberto. Existe a variante criptografada do protocolo, chamada HTTPS e ela pode ser utilizada para evitar a escuta de conexões.

# HTTPS

É uma forma de proteger a comunicação entre dois sistemas, como servidor e navegador. Ele permite o trânsito de dados confidenciais, como números de cartão de crédito, informações bancárias e credenciais de login. O "S" no final da sigla significa "Secure";

As informações transmitidas pelo HTTPS são criptografadas utilizando algoritmos de criptografia seguros que tornam praticamente impossível para um invasor interceptar e decifrar as informações transmitidas;

Os sites que usam HTTPS geralmente exibem um cadeado verde ao lado da barra de endereço do navegador, indicando que a conexão é segura e que as informações são protegidas.

![alt text](image.png)
