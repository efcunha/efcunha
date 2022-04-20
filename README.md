👋 ``` Olá, sou Edson F. Cunha ```

👀 ``` Estou aprimorando o máximo possível meus conhecimentos de Desenvolvedor Full Stack / DevOps Engineer ```
``` 
Conhecimentos:

-> Programação 
   -> JavaScript,Node,ESNext,HTML,CSS,Ajax,Angular,Gulp,JQyery,React,VueJS,Express
   -> Python
-> Banco de Dados Relacionais
   -> MySQL / MariaDB
   -> PostgreSQL
-> Banco de Dados não Relacional
   -> MongoDB
   -> NoSQL
-> Kubernetes / Cluster / HA 
-> Docker / Docker Swarm
-> Kasten K10
-> CI/CD (GitLab, ArgoCD, SonarQube, Sentry, Harbor, Jfrog)
-> Rancher
-> AWS / GCP / Azure
-> GitHub / Docker Hub
-> Snyk
-> Linux
-> Virtualização (XCP-NG, XenServer, Xen)
Etc...
```

🌱 ```Atualmente, estou implementando meus conhecimentos adquiridos de como montar uma infraestrutura de Rancher v2.6.x com Kubernetes K8s em Alta Disponibilidade.```

💞️ ```Estou procurando sempre colaborar com bases de conhecimento sobre Docker, Kubernetes, Rancher, etc...```
   
📫 ```Se quiser participar compartilhando conhecimento estou a disposição para ajudar.```

![rancher-kubernetes-producao](https://user-images.githubusercontent.com/52961166/116400929-9fd20000-a7f8-11eb-8e06-fe9cf393e4a9.png)

## Iniciando o dia....

Estes são os itens que ao sentar na cadeira, nós iremos fazer um checklist e verificar TODOS:

* Máquinas estão online no virtualizador ou na nuvem?
* RancherServer está online e acessível?
* Cluster's kubernetes estão todos online e com seus nodes funcionando?
* Monitoramento dos clusters está habilitado e funcionando?
* Sistema de log dos cluster's está habilitado e funcionando?
* Sistema de DNS dos cluster's está habilitado e funcionando?
* Sistema de volumes dos clusters está habilitado e funcionando?
* Ferramenta de Registro de imagens está online e funcionando?
* Revisão dos backups se estão sendo executados.
* Aplicações que fazem a limpeza no cluster estão rodando sem problemas? Verificar os logs.
* Comandos de kubectl respondem normalmente?

Ferramentas periféricas
* Ferramenta de integração contínua, online e funcionando? Se for o pipeline do Rancher, é na lista anterior.
* Ferramenta de repositório de código, git, online e funcionando?

Itens para ficar atento
* Quantidade de espaço em disco disponível nos worker's
* Consumo excessivo de recursos como CPU ou MEMÓRIO por algum container, pois significa que não foi aplicada a política controle de recursos.

CASO todos os itens acima tenham sido revisados e estejam OK, dai então podemos ir para as aplicações rodando dentro do cluster.

## Principais problemas

* Meu cluster não sobe
* Verificar portas abertas
* Verificar logs dos containers nos nós
* DNS, propagação de domínio
* Minha aplicação não sobe
* Os nós do cluster não se comunicam
* Meu pod está online, mas minha aplicação não
* Não consigo acessar minha aplicação
* Onde vejo os logs
* Onde vejo o monitormento?
* Onde acompanho os deployment's?
* Pipeline com problema, como resolvo?

## Referências

[Nirmata - Day 2 Kubernetes!](https://nirmata.com/2020/06/15/what-is-day-2-kubernetes/)

[ITOPS Times - Gerenciando Kubernetes no 2](https://www.itopstimes.com/contain/managing-day-2-kubernetes/)

O Kubernetes passou do Dia 0 e do Dia 1 e agora está na fase do **Dia 2** para a maioria das empresas. De acordo com Tobi Knaup, co-CEO e cofundador da empresa de gerenciamento nativo da nuvem D2IQ, o Dia 0 é a fase de design e prova de conceito, o Dia 1 é a fase de instalação e implantação e o Dia 2 é quando coisas como monitoramento, manutenção e a solução de problemas entram em jogo. O dia 2 também é quando um aplicativo passa de apenas um projeto de desenvolvimento para uma vantagem estratégica real para o negócio.

A **capacidade de monitoramento** também é importante por causa de todas as tecnologias que interagem com o Kubernetes. Quando você está executando clusters do Kubernetes, muitas vezes ele está sendo implantado junto com uma série de outras tecnologias. De acordo com Knaup, você precisa ser capaz de ter **dados de telemetria ao vivo em todas as partes do sistema** e ser capaz de depurar e diagnosticar problemas e encontrar sua causa raiz. “Todas essas são preocupações que, na verdade, o próprio Kubernetes não resolve”, disse Knaup. “Portanto, você precisa reunir uma pilha inteira de outras tecnologias de código aberto no ecossistema nativo da nuvem, para construir, por exemplo, uma pilha de monitoramento ou para construir uma história de segurança forte.”

Existem várias ferramentas que podem ajudar no monitoramento do Kubernetes, como **Prometheus, Jaeger ou Fluentd**, apenas para citar alguns. Pemmaraju recomenda que os administradores de TI não apenas obtenham treinamento no Kubernetes, mas também se familiarizem com o que está acontecendo no ecossistema Kubernetes. “Não se trata apenas do Kubernetes, **mas dos serviços em torno dele**, seja rede, armazenamento, monitoramento, alerta. Todas essas são coisas com as quais você precisa se familiarizar rapidamente ”, disse Pemmaraju.

Outra consideração no Dia 2 é a **escalabilidade**. Quando as empresas começam a usar o Kubernetes, podem ter alguns clusters em execução. Mas, de acordo com Knaup, o uso do Kubernetes pode se espalhar rapidamente por toda a organização depois que esses primeiros projetos forem implantados, portanto, ter a capacidade de escalonar é importante.

Freqüentemente, o Kubernetes é adotado de baixo para cima, o que significa que as equipes adotam o Kubernetes **separadamente**. Eventualmente, as organizações precisam consolidar tudo isso de forma consistente.

### Os operadores do Kubernetes ajudam na automação

Depois que uma empresa aborda essas preocupações gerais, que tipo de ferramenta a ajudará no Dia 2? De acordo com Knaup, os operadores tornam-se essenciais nesta fase. Os operadores do Kubernetes são ferramentas que basicamente automatizam a operação de cargas de trabalho complexas do segundo dia. Mais especificamente, de acordo com OperatorHub, os operadores implementam e automatizam atividades comuns do Dia 1, como instalação e configuração, e atividades do Dia 2, como reconfiguração, atualizações, backups, failovers, etc.

OperatorHub é um índice de operadores da comunidade que são empacotados para implantação em clusters Kubernetes. OperatorHub foi lançado pela Red Hat, os criadores do Operator Framework. Amazon, Microsoft e Google também estavam no grupo inicial de suporte ao OperatorHub.

[Operator Hub](https://operatorhub.io)

**GitOps** surge como uma metodologia poderosa para os desenvolvedores interagirem com o Kubernetes

Outra coisa que Knaup recomenda que as empresas examinem ao entrar no Dia 2 é o GitOps. Por causa da atual pandemia global, a KubeCon EU foi cancelada, mas de acordo com Knaup, cerca de **20%** das negociações programadas eram sobre GitOps.

GitOps é uma metodologia iniciada em 2017 na Weaveworks. De acordo com a Weaveworks, GitOps usa **“Git como uma única fonte de verdade para infraestrutura declarativa e aplicativos. Com o Git no centro de seus canais de entrega, os desenvolvedores podem fazer solicitações pull para acelerar e simplificar as implantações de aplicativos e tarefas operacionais para o Kubernetes.”**
<!---
efcunha/efcunha is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
