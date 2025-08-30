# Tipos-de-servico-de-nuvem
ReadMe com o resumo do lab de mesmo nome da DIO, na trilha GFT Start

Este repositório documenta a execução e os aprendizados do laboratório prático focado na configuração de Bancos de Dados na plataforma Microsoft Azure, como parte do bootcamp da DIO. O objetivo deste desafio foi consolidar o conhecimento sobre serviços de dados na nuvem, aplicando os conceitos em um ambiente prático e documentando o processo de forma clara e estruturada.

Conceitos Fundamentais Abordados
A aula forneceu uma base conceitual sólida, essencial para entender não apenas o "como", mas o "porquê" por trás das configurações na Azure.

1. Modelos de Serviço em Nuvem
O conceito mais importante abordado foi a divisão de responsabilidades entre o provedor de nuvem (Microsoft) e o cliente. Entendi a diferença fundamental entre os principais modelos de serviço:

PaaS (Platform as a Service - Plataforma como Serviço): Neste modelo, focamos exclusivamente na nossa aplicação e nos nossos dados. A Microsoft gerencia toda a infraestrutura subjacente, incluindo servidores, sistemas operacionais, atualizações e backups. O Banco de Dados SQL do Azure é um exemplo perfeito de PaaS. Ganhamos agilidade e reduzimos a carga de gerenciamento, pois não precisamos nos preocupar com a manutenção da plataforma.

SaaS (Software as a Service - Software como Serviço): Aqui, o provedor gerencia tudo, e nós apenas utilizamos o software pronto. É o modelo mais simples do ponto de vista do usuário. Exemplos clássicos são o Microsoft 365 ou o Gmail, onde apenas consumimos o serviço final.

IaaS (Infrastructure as a Service - Infraestrutura como Serviço): Embora a aula tenha focado em PaaS e SaaS, o conceito de IaaS foi usado como contraponto. Nele, gerenciamos a infraestrutura virtual, como Máquinas Virtuais (VMs) e redes. Temos mais controle, mas também muito mais responsabilidades.

2. O Processo Estruturado de Criação de Recursos na Azure
Notei que o portal da Azure utiliza um fluxo de trabalho consistente e guiado para a criação de diferentes tipos de recursos. Ao criar uma VM, por exemplo, passamos por uma série de abas sequenciais que organizam as decisões de configuração:

Básico: Informações essenciais como nome, região e credenciais.

Discos e Rede: Configurações de armazenamento e conectividade.

Gerenciamento, Monitoramento e Avançado: Opções administrativas e de performance.

Marcas (Tags): Ferramenta fundamental para organização e controle de custos.

Revisar + Criar: Uma validação final antes do provisionamento.

Durante este processo, aprendi como a escolha da Imagem (sistema operacional), Arquitetura (x64, ARM) e, principalmente, o Tamanho (vCPUs, RAM) são os fatores que mais refletem no valor da mensalidade do serviço.

Foco Prático: Criando um Banco de Dados SQL
O objetivo central do laboratório foi provisionar um Banco de Dados SQL do Azure, um serviço PaaS totalmente gerenciado. A explicação foi focada em nos familiarizar com o funcionamento geral do processo de provisionamento.

As etapas principais foram:

Criação do Servidor Lógico: Entendi que um Banco de Dados SQL precisa estar associado a um servidor lógico, que atua como um ponto de administração central. Criei um novo servidor, definindo seu nome, localização e as credenciais de administrador.

Configuração do Banco de Dados: Defini o nome do banco de dados e as configurações de computação e armazenamento, que determinaram o custo mensal estimado, exibido de forma transparente no portal.

Modelos de Redundância: Assim como em outros serviços da Azure, a escolha do modelo de redundância de backup (LRS, ZRS, GRS) é uma decisão crítica que equilibra custo e resiliência (SLA).

Provisionamento: Após a revisão, a Azure provisionou os recursos, deixando o banco de dados pronto para ser conectado por uma aplicação.

Conclusão
Este laboratório final foi crucial para conectar os pontos. A compreensão dos modelos de serviço (IaaS vs. PaaS) deixou clara a vantagem de usar um serviço gerenciado como o Banco de Dados SQL do Azure, que abstrai a complexidade da infraestrutura. O processo prático de criação solidificou minha compreensão sobre como provisionar recursos de dados na nuvem, sempre com atenção aos fatores críticos de custo, segurança e resiliência (SLA). Sinto-me mais preparado para dar os próximos passos na utilização de serviços de dados na Azure.
