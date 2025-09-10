# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS #

**Data:** 2025-09-10  
**Empresa:** Abstergo Industries  
**Responsável:** Gustavo [Seu Sobrenome]

## Introdução

Esse relatório apresenta o processo de implementação de ferramentas na empresa **Abstergo Industries**, realizado por **Gustavo [Seu Sobrenome]**. O objetivo do projeto foi identificar e implantar 3 serviços AWS que proporcionem redução imediata de custos operacionais, ao mesmo tempo que aumentem a escalabilidade e segurança da infraestrutura, suportando a operação como revendedora para farmácias e clientes finais.

## Descrição do Projeto

O projeto de implementação foi dividido em 3 etapas, detalhadas a seguir:

### Etapa 1:  
**Nome da Ferramenta:** Amazon EC2 Auto Scaling  
**Foco da ferramenta:** Escalabilidade automática e otimização de custos computacionais  
**Descrição do caso de uso:**  
Implementamos grupos de Auto Scaling que monitoram a carga nas instâncias EC2, ajustando automaticamente a quantidade de servidores em execução conforme a demanda do sistema. Durante picos, novas instâncias são lançadas para garantir desempenho sem interrupções; em períodos de baixa demanda, instâncias desnecessárias são desligadas, evitando gastos desnecessários com infraestrutura ociosa. Essa abordagem promove escalabilidade horizontal eficiente, reduzindo custos fixos e otimizando o uso de recursos computacionais.

### Etapa 2:  
**Nome da Ferramenta:** Amazon S3 com S3 Intelligent-Tiering  
**Foco da ferramenta:** Armazenamento de dados otimizado por custo e desempenho automático  
**Descrição do caso de uso:**  
Utilizamos buckets S3 configurados com a camada Intelligent-Tiering para armazenar dados essenciais como arquivos de clientes, logs transacionais e documentos fiscais. Essa camada monitora automaticamente os padrões de acesso e movimenta os objetos entre camadas de armazenamento com diferentes custos e latências, garantindo custo otimizado sem impacto na disponibilidade ou desempenho. A solução oferece alta durabilidade (99,999999999%) e escalabilidade praticamente ilimitada para suportar o crescimento dos dados da empresa.

### Etapa 3:  
**Nome da Ferramenta:** AWS Lambda  
**Foco da ferramenta:** Computação serverless para automação de processos sob demanda  
**Descrição do caso de uso:**  
Desenvolvemos funções Lambda para automatizar processos críticos como atualização de status de pedidos, notificações para clientes e integração entre sistemas internos. Essas funções são acionadas por eventos (ex: inserção de dados no banco, requisições HTTP) e executadas em ambiente gerenciado, eliminando a necessidade de servidores dedicados. O modelo pay-per-use garante que a empresa pague apenas pelo tempo de execução necessário, otimizando custos e facilitando a manutenção e escalabilidade das aplicações.

## Conclusão

A implementação das ferramentas AWS na **Abstergo Industries** resultou em uma infraestrutura flexível, altamente escalável e econômica, alinhada às necessidades de crescimento e redução de custos da empresa. Com a adoção do Auto Scaling, armazenamento inteligente no S3 e computação serverless via Lambda, a empresa está preparada para atender com eficiência suas demandas comerciais, garantindo agilidade operacional e redução significativa do custo total de propriedade (TCO). Recomenda-se a continuidade no uso dessas tecnologias e o monitoramento constante para identificar novas oportunidades de otimização.

---

**Assinatura do Responsável pelo Projeto:**  
Gustavo [Seu Sobrenome]
