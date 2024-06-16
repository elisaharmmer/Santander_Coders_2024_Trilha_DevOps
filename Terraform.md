# O que é Terraform?

O Terraform, desenvolvido pela HashiCorp, é uma ferramenta de infraestrutura como código (IaC) que permite aos usuários definir e provisionar infraestruturas de TI utilizando uma linguagem declarativa. Com o Terraform, é possível gerenciar a infraestrutura em várias nuvens públicas e privadas de maneira eficiente e repetível.

# Workflow do Terraform:

* _Escrever (Write):_

Os usuários escrevem configurações em arquivos .tf usando a HashiCorp Configuration Language (HCL). Esses arquivos definem os recursos e seus atributos.
Exemplos de recursos podem incluir servidores virtuais, redes, balanceadores de carga, etc.
As configurações podem ser divididas em múltiplos arquivos e diretórios para modularidade e reutilização.

* _Planejar (Plan):_

O comando terraform plan gera um plano de execução que mostra o que o Terraform fará para alcançar o estado desejado.
Ele compara a configuração atual com o estado anterior e a infraestrutura real, mostrando adições, modificações e destruições de recursos.
O plano de execução é revisado pelo usuário para garantir que as mudanças são as esperadas.

* _Aplicar (Apply):_

O comando terraform apply aplica as mudanças descritas no plano de execução.
O Terraform cria, modifica e destrói recursos de acordo com a configuração desejada.
As mudanças são persistidas no estado do Terraform, que é armazenado em um arquivo terraform.tfstate (ou remotamente, dependendo da configuração).


* _Destruir (Destroy):_

O comando terraform destroy é usado para remover todos os recursos definidos na configuração.
Ele é útil para ambientes temporários ou de teste, onde a infraestrutura precisa ser desprovisionada após o uso.

# Lifecycle do Terraform

O lifecycle do Terraform refere-se ao ciclo de vida dos recursos gerenciados e envolve os seguintes estágios:

* _Criação (Create):_

Quando novos recursos são definidos na configuração e aplicados, o Terraform cria esses recursos na infraestrutura.
Exemplos: criação de uma instância EC2 na AWS, provisionamento de um banco de dados, configuração de um load balancer.

* _Leitura (Read):_

O Terraform lê as informações do recurso diretamente da infraestrutura para obter o estado atual.
Isso garante que o Terraform esteja sincronizado com a infraestrutura real.

* _Atualização (Update):_

Quando mudanças são feitas na configuração de recursos existentes, o Terraform aplica essas mudanças atualizando os recursos.
Exemplos: alterar o tamanho de uma instância, modificar regras de firewall, ajustar configurações de rede.

* _Destruição (Delete):_

Recursos podem ser removidos quando não são mais necessários ou quando a configuração é alterada para excluir esses recursos.
O Terraform gerencia a destruição dos recursos de forma ordenada para evitar dependências quebradas.

* _Provisionamento e Desprovisionamento (Provision/Deprovision):_

Scripts de provisionamento, como scripts de inicialização ou ferramentas de configuração (Ansible, Chef, Puppet), podem ser executados durante a criação ou atualização de recursos.

_Desprovisionamento é a remoção dessas configurações quando os recursos são destruídos._

# Exemplos de Comandos:

* _Escrever Configuração:_
```sh
resource "aws_instance" "example" {
  ami           = "ami-0c55b159cbfafe1f0"
  instance_type = "t2.micro"
}
```

* _Plan:_
```sh
terraform plan
```

* _Apply:_
```sh
terraform apply
```

* _Destroy:_
```sh
terraform destroy
```

* O workflow e o lifecycle do Terraform permitem uma gestão eficiente e controlada da infraestrutura, garantindo que as mudanças sejam planejadas, aplicadas e rastreadas de maneira consistente e previsível.