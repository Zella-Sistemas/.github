## 📝 O que este Pull Request resolve?
## 🛠️ Checklist do Autor (Antes de pedir revisão)
[cite_start]Antes de solicitar a revisão do seu código, certifique-se de que sua branch atende aos requisitos básicos do projeto[cite: 7]. [cite_start]Isso poupa o tempo do revisor e agiliza a aprovação[cite: 8].

- [ ] [cite_start]A branch foi criada a partir da `stg` e aponta de volta para ela? [cite: 9]
- [ ] [cite_start]Os commits possuem a tag do card (ex: SMZ-12: descricao)? [cite: 10]
- [ ] [cite_start]O comando `run lint: fix` foi executado? [cite: 11]
- [ ] [cite_start]O código foi formatado pelo Prettier no salvamento (imports organizados e sem variáveis não utilizadas)? [cite: 12]
- [ ] [cite_start]A funcionalidade foi testada localmente (`npm run debug`) e nenhum erro estourou no console do navegador? [cite: 13]
- [ ] [cite_start]Foram removidos todos os `console.log()`, `debugger` e blocos de código comentados deixados durante o desenvolvimento? [cite: 14]

## 🔍 O Que Será Avaliado (Checklist do Revisor)
[cite_start]O revisor focará na arquitetura, aderência aos padrões do projeto e performance.

### Arquitetura e Padrões
- [ ] [cite_start]**Nomenclatura:** Todos os novos arquivos e pastas seguem o padrão kebab-case (ex: `painel-operacao.component.ts`)? [cite: 20]
- [ ] [cite_start]**Isolamento:** Lógicas de negócio complexas, transformações de dados pesadas ou chamadas HTTP estão devidamente isoladas em Services? [cite: 22]
- [ ] [cite_start]**Standalone Components:** O novo componente foi gerado como `standalone: true` para facilitar o lazy loading e melhorar o tree-shaking? [cite: 24]

### Angular, TypeScript e Estado
- [ ] [cite_start]**Sintaxe Moderna:** O código novo já está utilizando a sintaxe moderna de controle de fluxo do Angular 21 (`@if`, `@for`, `@switch`)? [cite: 31]
- [ ] [cite_start]**Signals:** O estado do componente está aproveitando o uso de Signals? [cite: 32]
- [ ] [cite_start]**Tipagem:** As variáveis estão tipadas e o uso de `any` foi evitado? [cite: 33, 34]
- [ ] [cite_start]**Memory Leaks:** Os Observables possuem a correta desinscrição ou utilizam o `async` pipe no HTML? [cite: 35]

### Estilização e UI
- [ ] [cite_start]**PrimeFlex:** O layout foi construído prioritariamente utilizando as classes do PrimeFlex? [cite: 26]
- [ ] [cite_start]**CSS Customizado:** Códigos CSS/SCSS customizados foram criados apenas quando era impossível resolver com PrimeFlex ou propriedades do PrimeNG? [cite: 27]

### Tratamento de Erros e Performance
- [ ] [cite_start]**Exceções HTTP:** As chamadas para a API estão tratando os erros corretamente? [cite: 38]
- [ ] [cite_start]**Feedback de UI:** O usuário recebe um feedback amigável e claro (ex: componente SweetAlert2) quando uma requisição falha? [cite: 39]
- [ ] [cite_start]**Lazy Loading:** Novos módulos ou rotas pesadas foram implementados utilizando lazy loading? [cite: 41]
- [ ] [cite_start]**Importações:** As importações de bibliotecas pesadas estão importando apenas os módulos necessários? [cite: 44]

## 📸 Evidências (Opcional, mas recomendado)
