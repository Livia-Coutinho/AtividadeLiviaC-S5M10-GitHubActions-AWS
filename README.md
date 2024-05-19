# AtividadeLiviaC-S5M10-GitHubActions-AWS

### Enunciado da atividade

Leia o artigo proposto no autoestudo e redija um texto técnico abordando os seguintes temas:
</br>
- TEMA 1 - A importância de CI/CD no desenvolvimento de software e como ele melhora a eficiência dos times de desenvolvimento.
- TEMA 2 - A estrutura e os componentes principais de um workflow do GitHub Actions.
- TEMA 3 - A função e a importância do AWS CloudFormation na automação da infraestrutura. Anexe e explique o template que você está usando no seu projeto para criar a instância EC2.
- TEMA 4 - Discuta como a integração de GitHub Actions com AWS CloudFormation e Amazon EC2 pode ser aplicada em projetos reais. Quais desafios você encontrou no seu projeto e como os solucionou?

#### Link do artigo proposto:
- https://aws.amazon.com/pt/blogs/devops/integrating-with-github-actions-ci-cd-pipeline-to-deploy-a-web-app-to-amazon-ec2/

# Atividade

## A importância de CI/CD no desenvolvimento de software e como ele melhora a eficiência dos times de desenvolvimento.

Abaixo será tratado sobre a importância da prática de CI/CD no dev de software e como ela contribui significativamente para a eficiência dos times de desenvolvimento.

A adoção de práticas de CI/CD permite que as equipes de desenvolvimento automatizem e simplifiquem o processo de desenvolvimento de software e gerenciamento de infraestrutura. Isso vai não apenas acelerar o ritmo de inovação, como também melhorar a qualidade e a consistência dos lançamentos de software. </br>
O CI/CD é uma parte essencial das práticas de DevOps, que visam quebrar as barreiras entre as equipes de desenvolvimento e operações, promovendo uma cultura de colaboração contínua.

- **Continuous Integration** envolve a integração contínua de código em um repositório compartilhado várias vezes ao dia. Isso permite que erros sejam detectados mais cedo, já que cada alteração no código é automaticamente testada. A detecção precoce de erros facilita a correção de problemas antes que eles se tornem grandes e difíceis de resolver.

- **Continuous Delivery**, por outro lado, leva essa automação um passo adiante ao automatizar o processo de liberação do software para um ambiente de produção. Cada mudança de código é preparada para uma possível liberação, permitindo que os desenvolvedores entreguem novas funcionalidades, correções de bugs e melhorias de forma rápida e eficiente.

Um exemplo da implementação de CI/CD é a integração de GitHub Actions com AWS CodeDeploy, conforme descrito no artigo proposto (link acima). Assim, as GitHub Actions são usadas para orquestrar um pipeline de CI/CD que constrói, testa e implanta uma aplicação Java SpringBoot em instâncias do Amazon EC2 em um grupo de autoescalamento.

Essa configuração oferece algumas vantagens, como:

- **Automação completa:** desde quando o código é comitado no repositório GitHub até a implantação na infraestrutura de produção, todos os passos são automatizados. Isso reduz a possibilidade de erros humanos e garante consistência no processo de implantação.

- **Feedback rápido:** com a integração contínua, quem está desenvolvendo, recebe feedback rápido sobre o impacto de suas alterações, o que permite a correção rápida de problemas e a manutenção da qualidade do código.

- **Escalabilidade:** com serviços como AWS Auto Scaling e CodeDeploy, a aplicação pode ser escalada automaticamente de acordo com a demanda, mantendo a disponibilidade e desempenho do serviço.

- **Segurança:** o uso de provedores de identidade como IAM OIDC permite a integração segura entre GitHub e AWS, eliminando a necessidade de manter segredos e credenciais sensíveis no repositório.
