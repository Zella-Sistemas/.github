📝 O que este Pull Request resolve?
🛠️ Checklist do Autor (Antes de pedir revisão)
Antes de solicitar a revisão do seu código, certifique-se de que sua branch atende aos requisitos básicos do projeto. Isso poupa o tempo do revisor e agiliza a aprovação.

- [ ] A branch foi criada a partir da `stg` e aponta de volta para ela?
- [ ] Os commits possuem a tag do card (ex: SMZ-12: descricao)?
- [ ] O comando `run lint: fix` foi executado?
- [ ] O código foi formatado pelo Prettier no salvamento (imports organizados e sem variáveis não utilizadas)?
- [ ] A funcionalidade foi testada localmente (`npm run debug`) e nenhum erro estourou no console do navegador?
- [ ] Foram removidos todos os `console.log()`, `debugger` e blocos de código comentados deixados durante o desenvolvimento?

🔍 O Que Será Avaliado (Checklist do Revisor)
O revisor focará na arquitetura, aderência aos padrões do projeto e performance.

Arquitetura e Padrões
- [ ] Nomenclatura: Todos os novos arquivos e pastas seguem o padrão kebab-case (ex: `painel-operacao.component.ts`)?
- [ ] Isolamento: Lógicas de negócio complexas, transformações de dados pesadas ou chamadas HTTP estão devidamente isoladas em Services?
- [ ] Standalone Components: O novo componente foi gerado como `standalone: true` para facilitar o lazy loading e melhorar o tree-shaking?

Angular, TypeScript e Estado
- [ ] Sintaxe Moderna: O código novo já está utilizando a sintaxe moderna de controle de fluxo do Angular 21 (`@if`, `@for`, `@switch`)?
- [ ] Tipagem: As variáveis estão tipadas e o uso de `any` foi evitado?

Estilização e UI
- [ ] PrimeFlex: O layout foi construído prioritariamente utilizando as classes do PrimeFlex?
- [ ] CSS Customizado: Códigos CSS/SCSS customizados foram criados apenas quando era impossível resolver com PrimeFlex ou propriedades do PrimeNG?

Tratamento de Erros e Performance
- [ ] Exceções HTTP: As chamadas para a API estão tratando os erros corretamente?
- [ ] Feedback de UI: O usuário recebe um feedback amigável e claro (ex: componente SweetAlert2) quando uma requisição falha?
- [ ] Lazy Loading: Novos módulos ou rotas pesadas foram implementados utilizando lazy loading?
- [ ] Importações: As importações de bibliotecas pesadas estão importando apenas os módulos necessários?

📸 Evidências (Opcional, mas recomendado)
