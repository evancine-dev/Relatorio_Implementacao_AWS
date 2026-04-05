# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 04 de abril de 2026
Empresa: Abstergo Industries
Responsável: Consultor de Soluções em Nuvem

---

## Introdução

Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Sayuri Bortoti. O objetivo do projeto foi elencar 3 serviços AWS com a finalidade de realizar diminuição de custos imediatos, otimizando a infraestrutura tecnológica da empresa no setor farmacêutico.

---

## Descrição do Projeto

O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

---

### Etapa 1

- Nome da ferramenta: Amazon S3 (Simple Storage Service)
- Foco da ferramenta: Armazenamento de dados com redução de custo de infraestrutura física
- Descrição de caso de uso:
  A Abstergo Industries lida com grandes volumes de dados regulatórios, resultados de pesquisas clínicas, bulas, laudos laboratoriais e documentação de conformidade (ANVISA, FDA). Atualmente, esses arquivos são armazenados em servidores físicos locais com alto custo de manutenção, energia e escalabilidade limitada.
  
  Com a migração para o Amazon S3, a empresa poderá armazenar todos esses arquivos na nuvem com classes de armazenamento inteligentes, como o S3 Intelligent-Tiering, que move automaticamente os dados para camadas de menor custo quando o acesso não é frequente. Documentos históricos de pesquisa, por exemplo, que raramente são acessados, podem ser arquivados no S3 Glacier, reduzindo o custo de armazenamento em até 80% comparado a servidores locais. Além disso, o S3 oferece durabilidade de 99,99%, eliminando riscos de perda de dados críticos.

---

### Etapa 2

- Nome da ferramenta: AWS Lambda
- Foco da ferramenta: Computação serverless para automação de processos sem custo de servidores ociosos
- Descrição de caso de uso:
  A Abstergo Industries realiza diversas tarefas automatizadas ao longo do dia — como geração de relatórios de controle de qualidade, notificações de vencimento de lotes, integração entre sistemas de ERP e plataformas de distribuição, e validação de dados de entrada em sistemas regulatórios.

  Atualmente, essas tarefas rodam em servidores EC2 que permanecem ligados 24 horas por dia, mesmo quando não há processamento em andamento, gerando custos desnecessários. Com o AWS Lambda, a empresa pagará apenas pelo tempo de execução real das funções, sem custo em períodos de ociosidade. Para workloads intermitentes como as descritas, a economia estimada pode chegar a 60–70% em relação ao modelo de servidor dedicado, além de eliminar a necessidade de gerenciamento de infraestrutura.

---

### Etapa 3

- Nome da ferramenta: Amazon RDS (Relational Database Service) com instâncias Reserved
- Foco da ferramenta: Banco de dados gerenciado com otimização de custos por reserva de capacidade
- Descrição de caso de uso:
  Os sistemas de gestão de estoque, controle de produção e acompanhamento de ensaios clínicos da Abstergo Industries dependem de bancos de dados relacionais robustos. Manter esses bancos em servidores físicos ou em instâncias EC2 não gerenciadas implica custos elevados com licenciamento, patches manuais, backups e alta disponibilidade.

  Com o Amazon RDS, todos esses processos de manutenção passam a ser gerenciados pela AWS, reduzindo a carga da equipe de TI. Ao optar pelas Reserved Instances, a Abstergo Industries pode obter descontos de até 72% em comparação ao preço sob demanda. O RDS também oferece failover automático com Multi-AZ, garantindo disponibilidade dos dados de produção e conformidade com requisitos regulatórios do setor farmacêutico.

---

## Conclusão

A implementação das ferramentas na empresa Abstergo Industries tem como esperado a redução significativa dos custos operacionais de TI, a eliminação de gastos com infraestrutura física ociosa e o aumento da confiabilidade e disponibilidade dos sistemas críticos da empresa. Com o Amazon S3, o AWS Lambda e o Amazon RDS com Reserved Instances, estima-se uma redução de custos de infraestrutura entre 50% e 70% no primeiro ano, além de ganhos em escalabilidade, segurança e conformidade regulatória.

Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa, como a adoção do AWS Cost Explorer para monitoramento contínuo de gastos e o AWS Trusted Advisor para recomendações automáticas de otimização.

---

## Anexos

- Manual de uso do Amazon S3 e política de ciclo de vida de objetos
- Documentação de funções Lambda implementadas e gatilhos configurados
- Comparativo de custos: infraestrutura anterior vs. Amazon RDS Reserved Instances
- Planilha de estimativa de economia anual por serviço
- Relatório de conformidade de segurança (AWS Shared Responsibility Model)

---

Assinatura do Responsável pelo Projeto: Sayuri Bortoti

Sayuri Bortoti
Abstergo Industries — Abril de 2026