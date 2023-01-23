# Exame Az-900 Resumo

Prova contem de 40 a 60 questões, podendo ser feita em ENG ou PT-BR

Tempo da prova é de 86 minutos

pontuação da prova vai de 1 - 1000

Nota minima para passar 700 - pontos

Portal Azure -> https://portal.azure.com/?quickstart=true#view/Microsoft_Azure_Resources/QuickstartCenterBlade

### Modelos de cloud's ou Models

![image](https://user-images.githubusercontent.com/44281161/212974626-23ee7418-0c98-43f9-9b83-7b8eb37bd2c0.png)

`Infraestrutura Como Serviço
Iass -> Infraestrutura ou servidor físico, nesse modelo o cliente que contratou gerencia seu servidor`

* IasS
usada para acesso a recursos de computação e armazenamento baseados na Internet. Sendo a categoria mais básica entre os tipos de computação em nuvem, a IaaS permite que você alugue uma infraestrutura de TI (servidores e máquinas virtuais, armazenamento, redes e sistemas operacionais) de um provedor de nuvem em uma base paga conforme o uso.


`Plataforma Como Serviço
Paas -> Modelo pago pelo cliente onde ele utiliza e não precisa se preocupar com licenças da aplicação, apenas se preocupa como utilizar. ("Aplicação da própria Microsoft Azure")`

* PasS
que dá aos desenvolvedores as ferramentas necessárias para criar e hospedar aplicativos Web. A PaaS foi desenvolvida para proporcionar aos usuários o acesso aos componentes necessários para desenvolver e operar rapidamente aplicativos Web ou móveis na Internet, sem se preocupar com a configuração ou gerenciamento da infraestrutura subjacente dos servidores, armazenamento, redes e bancos de dados.


`Software Como Serviço
Saas -> Software da aplicação`

* SasS
usado para aplicativos baseados na Web. O SaaS é um método de entrega de aplicativos de software na Internet, no qual os provedores de nuvem hospedam e gerenciam os aplicativos de software, fazendo com que seja simples ter o mesmo aplicativo em todos seus dispositivos de uma só vez por meio da nuvem.



### Tipos de Cloud

-------------------------------**Private**-------------------------------

Private -> Quando Monta a sua estrutura em um espaço de data center.
OBS: Esse plano tem de a ser muito mais caro em compensação ao public e ao hybrid

Vantagens de uma nuvem privada:

Maior flexibilidade – sua organização pode personalizar seu ambiente de nuvem para atender a necessidades de negócios específicas.

Maior controle – os recursos não são compartilhados com outros usuários, portanto, é possível um nível maior de controle e privacidade.

Maior escalabilidade –nuvens privadas geralmente oferecem mais escalabilidade em comparação com a infraestrutura local.

-------------------------------**Public**-------------------------------

Public -> Quando o cliente aluga maquinas virtuais e soluções em nuvem.
OBS-1: A parte do hardware e a manutenção fica por conta do provedor cloud seja ela "Azure, AWS ou GoogleCloud".
OBS-2: Esse plano tem de a ser mais barato entre todos.

Vantagens das nuvens públicas:

Redução de custos – não há necessidade de comprar hardware ou software e você paga somente pelos serviços que usa.

Sem manutenção – seu provedor de serviços fornece a manutenção.

Escalabilidade quase ilimitada – recursos sob demanda estão disponíveis para atender às suas necessidades de negócios.

Alta confiabilidade – uma ampla rede de servidores assegura contra falhas.

-------------------------------**Hybrid**-------------------------------

Hybrid -> É uma mistura do Private + Public onde uma parte fica privado em seus próprios servidor e outros em nuvem.
OBS-1: Esse plano tem de a ter seu valor intermediário comparado ao private e ao public.
OBS-2: Esse plano vai ter um pouco de investimento pois vai ser levado em conta uma parte da estrutura física e outra parte em nuvem.



### 5 benefícios de Cloud
`{ 1. Flexibilidade 2. Custo-benefício 3. Segurança 4. Prototipagem rápida 5. Melhor colaboração 6. Alta disponibilidade 7. Escalabilidade 8. Alcance global 9. Agilidade 10. Recuperação de desastre 11. Tolerância a falhas 12. Elasticidade 13. Capacidade de latência do cliente }`

### Regions and availability zone

Regions -> *As regiões são formadas por um conjunto de Availability zone's*
  * Fornece uma flexibilidade e escala para reduzir a latência do cliente.
  * As regiões  são compostas de um ou mais datacenters muito proximos.

Availability zone -> *Zona de disponibilidade*

![image](https://user-images.githubusercontent.com/44281161/214054823-f716b109-9fa6-4c10-8528-86390505f67a.png)

![image](https://user-images.githubusercontent.com/44281161/214056786-14fd17c3-e7c2-4dfa-8efe-7a7f13904b93.png)

►  Azure Global Infrastructure
🔗 https://infrastructuremap.microsoft.com/

►  Calculadora do Azure
🔗 https://azure.microsoft.com/pt-br/pricing/calculator/

### Grupo de recursos


Lugar onde associamos tudo que é criado para manter como forma organizacional nossos recursos
Ex: Server e detro de server vai esta uma lista com todos os meus sevidores associados ao Grupo de recurso chamado server;

OBS-1: É possivel visualizar quanto está gastando por grupo de recurso.

OBS-2: Quem gerencia todos os recurso é o ARM -> Azure resource manager


### Azure CLI

Pode ser utilizado para criar ou fazer qualquer alteração via linha de comando, onde o CLI funciona atravez do Power Shell ou pelo cloud Shell

### Azure Marketplace

Area dentro da Azure com soluções pré-criadas

Scale set's

> Scale set ou conjuntos de escalas de máquina virtual -> Em Teoria após configurado ela pode criar novas máquinas dividindo conforme a regra o seu desempenho EX: posso criar uma máquina e um esquema de configuração para criar um clone da minha máquina quando a minha principal atingir 50% da capacidade, fazendo assim com que o fluxo seja dividindo entre as duas e cada uma ficando com 25% do fluxo ao final quando o fluxo normalizar ela pode destruir as maquinas deixando apenas a original.

- OBS-1: Para fazer o Scale set's é necessário no mínimo de 2 maquinas sendo uma original e a sua cópia, com isso é possível fazer a divisão do tráfego de usuários que acessam a página web e o máximo de máquinas são de 1000.

- Ganho do Scale sets -> Economia não fica esperando com máquina montada chegar o tráfico de usuários acessando, só vai montar uma nova maquina virtual caso seja necessário e para montar o scale set não tem custo nenhum o custo só vai começar a ser gerado se a demanda tiver ativa e conforme as necessidades.



### App Service ou Serviço de Aplicativo

É possivel criar códigos sem ter uma máquina física ou virtual, o código poder ser implementado diretamente no server da azure, que tem um alto poder de escalonamento/escalabilidade, onde a forma de cobramça vai ser cobrado a cada acesso de usuário.


### ACI

ACI -> Azure Container instance

> Beneficios do ACI
- Tem uma compatibilidade maior
- Tem uma eficiência maior
- Mantém a consistência do sistema operacional
- Tem portabilidade muito grande
- É possível gerenciar todas as dependências da aplicação dentro do contêiner

***OBS-1: para achar ele dentro do painel da azure basta procurar por instância de contêiner.***

### Azure kubernetes ou AKS

>Responsável por organizar e gerenciar os contêiners
>
>> Sistema de gerenciamento de contêineres ou autotratamento dos contêineres -> Ex: duplicar um contêiner, essa funcionalidade também conto com o auto scaling aumentando ou diminuindo os recursos conforme o configurado, ou necessidade.

- OBS-1: Caso o contêiner seja duplicado para melhorar o desempenho de processamento, ele se torna um POD e o kubernetes gerencia os contêineres que estão dentro do POD.

- OBS-2: Para encontra esse serviço dentro do painel da azure basta procurar por Serviços do kubernetes.

### AVD ou Azure virtual Desktop

> É a área de trabalho virtual da azure
>
>> mite que o usuário consiga acessar a plataforma azure de qualquer lugar e dispõem de internet de no mínimo de 1 giga.
É possivel criar dentro da area de trabalho virtual:

- Pools de hots
- Grupo de aplicativos
- Workspaces
- Plano de escala
- Usuários

***OBS-1: Para encontra esse serviço dentro do painel da azure basta procurar por Área de trabalho virtual do azure.***

### Aplicativo de Funções

Serviço para criar pequenas modulos de funções separadas do seu código onde só vai ser cobrado, quando a funcionalidade de fato for chamada, melhorando também no desempenho da aplicação.

***OBS-1: Para encontra esse serviço dentro do painel da azure basta procurar por Aplicativo de funções.***

### IPV4

>> IPV4 -> Internet protocol version 4
>
>> Ajuda no endereçamento das maquinas e conversação entre elas.

### Redes ou VNET

- Rede virtual -> É possivel criar um arede com Vm's e criar conexões entre elas, apenas utilizando o endereçamento de ip e o bastion host.

### Load Balancer ou Balanceador de carga

É um balanceador de tráfego que faz com que as cargas e tráfegos sejam divididos entre as máquinas virtuais, sendo assim não deixando um servidor sobrecarregado e mantendo o trafego estável entre as VM'S.

***OBS-1: O load Balancer so faz a divisão conforme a regra montado ex -> existem 2 maquinas virtuais onde uma vai receber 60% do tráfego e a outra vai receber os 40% assim elas não sobrecarga e nem chega na sua capacidade máxima.***

***OBS-2: Para encontra esse serviço dentro do painel da azure basta procurar por Balanceador de Carga.***

### VPN Gatewway

Serve para encriptar dados privados de uma empresa, é só é possível acessar utilizando chaves de seguranças: ela é decriptada na entrada e na saída, assim estando na internet mais com arquivos privados sendo guardados com segurança.

### Application Gateway

Controlador de entrega de aplicativo gerenciado por plataforma, escalonável e altamente disponível como serviço

- Entrega de aplicativo Web escalonável e de alta disponibilidade
- Roteamento inteligente da camada 7

### Express Route

É um serviço de rota que faz com que seu tempo seja minimizado para transferências de dados extremamente grandes, ex-> preciso transferir 3TB de vídeos para um servidor na nuvem, com o express router isso é possível ser feito de forma direta e com alta velocidade.

***OBS-1: O valor para o uso de express router é extremamente caro, porem atende a necessidade de uma transferência mais rápida com altas demandas.***

### CDN

CDN -> Content Delivery Network: Após sua ativação é feito uma cópia do conteúdo e distribuído entre as Regions, fazendo com que o usuário que entra no domínio receba o arquivo com uma velocidade quase que instantânea: ele vai apontar para uma cópia do conteúdo que foi distribuído e armazenado na região mais próxima do usuário.

## Armazenamento

#### Blob Storage

Local onde é possivel armazenar arquivos com extensões ex -> .JPG, .MP4, .DOC, .XLS...

Para utilizar dos arquivos basta apontar para o endereço onde os arquivos foram guardados.

Existe 3 tipos de valores que podem ser cobrados pela Microsoft:
- 1º Hot - é muito utilizado para pessoas que acessam com uma frequência muito alto, consequentemente o valor é bem mais caro na hora da cobrança.

- 2º Cool - consegue guardar a mesma quantidade de arquivos que o hot porem é ideal para quem acessa com uma quantidade de frequência menor que o Hot consequentemente o custo se torna um pouco mais atrativo.
OBS-1: No plano Cool os dados tem que ficar lá sem acesso no mínimo por 30 dias, caso coloque o plano como cool e utilize com o prazo menor que 30 dias a cobrança será maior do que o plano "Hot"

- 3º Archive - Custo muito baixo, normalmente utilizados para Backups, pois se entendi que não ira mexer com frequência no arquivo apenas se precisar algum dia ou se necessário.

***OBS-1: Para encontra esse serviço dentro do painel da azure basta procurar por Contas de armazenamento.***

#### Discos

>>Tipos de disco, basicamente existe 4 são eles:
>>
>> - 1º HDD -> É o mais barato dentro da azure e é excelente para backups.
>>
>> - 2º Standard SSD -> É um dos mais caros e é excelente para aplicações que requer uma alta disponibilidade e alta velocidade de leitura e escrita de dados.
>>
>> - 3º Premium SSD ->É muito mais caro, porém é ótimo para aplicações sensitivo a latência.
>>
>> - 4º Ultra disk -> Tem as mesmas especificações do Premium porem ele consegue chegar a 64TB de espaço.
>>
>>> ***OBS-1: Para encontra esse serviço dentro do painel da azure basta procurar por Discos.***

#### Banco de dados suportados pela Azure

- Cosmo DB - Banco Não Relacional
- Azure SQL - Relacional
- PostgreSQL - Objeto-relacional -> _sem relação com linguagens de programação orientadas a objetos_
- MySQL - Relacional

#### Migração

****OBS-1: Para encontra esse serviço dentro do painel da azure basta procurar por Serviço de migração de banco de dados do Azure.****

#### Defense in depth

##### Responsabilidades da Azure e Cliente

**Camada de Estrutura física**
1. Predios
2. Data center's

**Camada de Identidade e acesso**
1. Quem pode logar na sua conta
2. Fator de Login 
- MFA
- SMS
- changes
- Log de eventos
- Topologia de acesso

**Camada de Parâmetros**
1. Firewall

**Camada de Rede**
1. Acess list
2. Acesso de entrada
3. Acesso de Saída

**Camada de Computação**
1. Bastian Host
2. conexão SSH
3. Manter ultimas atualizações de Software e patchs

**Camada de Aplicação**
1. Garantir que tudo está aplicado de forma correta para garantir segurança.

**Camada de Data**
1. Encripitar

***OBS-1: As 7 camadas de segurança mantêm o sua nuvem mais segura.***

### Componentes Essenciais de segurança

#### Firewall

#### Microsoft Defender para Nuvem
`O Defender para Nuvem é uma ferramenta para gerenciamento de postura de segurança e proteção contra ameaças. Ele fortalece a postura de segurança dos seus recursos de nuvem, e, com seus planos integrados do Microsoft Defender, o Defender para Nuvem protege as cargas de trabalho em execução no Azure, em ambiente híbrido e em outras plataformas de nuvem.`

#### Cofre de chaves
**Key vault** -> Responsável por criar credenciais, temporárias, normalmente utilizada por empresas parceiras ou terceiros.

#### Microsoft Sentinel
`O Microsoft Sentinel é uma solução escalonável e nativa de nuvem que oferece SIEM (gerenciamento de eventos de informações de segurança) e SOAR (resposta automatizada para orquestração de segurança) . O Microsoft Sentinel oferece análise inteligente de segurança e inteligência contra ameaças em toda a empresa, com uma solução para detecção de alertas, visibilidade de ameaças, procura proativa e resposta a ameaças.`

***Principais recursos do Sentinel***

1. Colete dados na escala de nuvem de todos os usuários, dispositivos, aplicativos e infraestrutura, local e em múltiplas nuvens.

2. Detecte ameaças que ainda não foram descobertas e minimize falsos positivos usando a análise e a inteligência contra ameaças incomparáveis da Microsoft.

3. Investigue ameaças com inteligência artificial e busque por atividades suspeitas em escala, acessando anos de trabalho sobre segurança cibernética na Microsoft.

4. Responda a incidentes de forma rápida com orquestração interna e automação de tarefas comuns.

#### Internet das Coisas (IoT) do Azure
`A Internet das Coisas (IoT) do Azure é uma coleção de serviços cloud geridos pela Microsoft que ligam, monitorizam e controlam milhares de milhões de recursos de IoT. Em termos mais simples, uma solução IoT é composta por um ou mais dispositivos IoT que comunicam com um ou mais serviços de back-end alojados na cloud.`

#### Assinaturas
Local onde podemos gerenciar as assinaturas de uma conta ex-> Temos duas empreasas Empresa-123 e Empresa-321, lá podemos dividir as assinaturas para cada empresa e assim conseguimos acompanhar os custos da cloud por empresa e saber quanto cada uma está gastando com os recursos.

***OBS-1: Cada assinatura é possível ver alguns detalhes como Análise de custo, criar alerta de custo, ver orçamentos e até ter recomendações de custo***

#### Gerenciamento de custo e orçamentos

Na Analise de custo é possivel ver e ter uma previsão de quanto será cobrado ao final do mês, e caso o usuario queira ver com mais detalhes a analise de custo mostra os gasto por nome do serviço, por localidade e ate mesmo por nome de grupo.

***OBS-1: É recomendado criar orçamentos com alerta pois, quando algum serviço ou assinatura X atingir um percentual proposto no orçamento, o administrador irá receber um alerta via SMS ou via E-mail, isso vai de acordo com o configurado.***

***OBS-2: Caso o orçamento chegue no limite, ele não ira parar os serviços apenas vai ser cobrado mais no faturamento final por isso caso tenha feito orçamentos e não queira passar do proposto é bom se atentar aos alertas criados.***

#### Calculadora de preço azure

[Página de acesso a calculadora](https://azure.microsoft.com/pt-br/pricing/calculator/)

#### Plano de suporte

**Existem 4 tipos de plano de suporte**
1. Básico
2. Developer
3. Standard
4. Professional Direct

#### SLA ou Service Level Agreement

Contrato de tempo de acordo entre o provedor e o cliente para resolução de um serviço.

#### Atualizações do Azure

[Site com as atualizações Azure](https://azure.microsoft.com/pt-br/updates/)

[Resumo Azure Click Aqui!](https://github.com/feliperafa/Azure-Resumo-Nuvem/blob/90add817d0468f555144007305f153c43cfb73ef/Azure%20Anota%C3%A7%C3%B5es.md)
