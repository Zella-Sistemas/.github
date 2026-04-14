# 🛡️ Padrões e Automações - Zella Sistemas

Bem-vindo ao repositório central de configurações da organização! 

Este repositório (`.github`) é um recurso especial do GitHub. Os arquivos de configuração, templates e fluxos de trabalho (workflows) armazenados aqui são **herdados automaticamente** por todos os outros repositórios da organização (a menos que o repositório tenha o seu próprio arquivo para sobrescrever).

## 🎯 Objetivo
Com o foco em escalabilidade e na qualidade dos nossos projetos, manter a padronização do código é fundamental. Este repositório central serve para:

1. **Reduzir a carga cognitiva:** Automatizar tarefas repetitivas para que a equipe foque no que importa: a lógica de negócio.
2. **Centralizar padrões:** Garantir que todos os projetos sigam as mesmas regras básicas de Code Review e governança.
3. **Facilitar o Onboarding:** Novos membros já encontram a "casa arrumada" e guiada por templates desde o primeiro Pull Request.

## 📂 O que temos aqui?

* 📄 **`pull_request_template.md`**: O formulário base carregado automaticamente sempre que alguém abre um Pull Request em qualquer repositório nosso. Ele traz o "Checklist do Autor", garantindo que verificações básicas (como rodar o lint, limpar `console.log` e testar localmente) sejam feitas antes de consumir o tempo de um revisor.

## 🚀 Próximos Passos (Em breve)
Estamos evoluindo nossa esteira de integração. Em breve, este repositório também hospedará **Workflows do GitHub Actions**, como:
* 🤖 **Bot de Linting Automático:** Para barrar código fora da formatação padrão do projeto ou com erros de sintaxe (acionando o Prettier/ESLint).
* 🔒 **Automações de Segurança:** Verificações adicionais no fluxo de CI/CD.

---
*Nota: Este repositório é a base da nossa governança técnica. Sugestões de melhorias nos templates ou novas ideias de automação são muito bem-vindas!*
