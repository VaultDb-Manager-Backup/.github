# VaultDB

**VaultDB** is an open-source backup manager built to structure reliable backup processes for real production systems.

Backup is not a tool. It is a process — and VaultDB exists to make that process predictable, auditable, and automated.

---

## Why VaultDB exists

In many small and medium projects, backups are handled through:
- fragile scripts
- manual routines
- untested processes
- implicit assumptions that “it will work when needed”

VaultDB was created to replace improvisation with a structured backup process, focused on reliability rather than promises.

---

## What VaultDB is

- An **open-source backup manager** for production databases
- A tool to **automate and structure backup processes**
- Designed for **real systems with real data**
- Focused on **process, observability, and predictability**
- Suitable for **small teams and individual projects** growing into production

---

## What VaultDB is not

- A magic solution that guarantees zero data loss
- A replacement for good operational practices
- A generic backup script generator
- A “set and forget” tool without responsibility

---

## Core principles

- **Process over tooling**  
  Backup reliability comes from process, not from scripts alone.

- **Separation of concerns**  
  Backup execution, storage, and restoration should not depend on the same failure domain.

- **Predictable recovery**  
  A backup is only useful if restoration is clear, tested, and repeatable.

- **Transparency**  
  Open source enables review, discussion, and safer defaults.

---

## How VaultDB works (high level)

1. **Secure connection**  
   Configure access to your database or production environment with minimal permissions.

2. **Automated backups**  
   Backups run automatically based on defined strategies, without manual intervention.

3. **Separated storage**  
   Backup data is stored separately from the primary environment to avoid single points of failure.

4. **Controlled restoration**  
   Restoration follows a predictable process, reducing panic and improvisation during incidents.

---

## Observability and analytics

VaultDB uses **server-side analytics** to track real product usage and reliability signals.

- Events are generated **only by the backend**
- No backup content is ever accessed or transmitted
- Events represent **operational outcomes**, not clicks or page views

Example of a real product event:
- `first_backup_success` — fired only when a backup completes successfully for the first time

These events help improve the product without compromising data privacy.

---

## Privacy and responsibility

- VaultDB **does not access backup contents**
- Only minimal operational metadata is processed
- No personal data is sold or shared
- The operator remains responsible for:
  - backup validation
  - restoration testing
  - retention strategies

See:
- [Privacy Policy](https://vaultdb.com.br/privacy)
- [Security Policy](https://vaultdb.com.br/security)
- [SLA](https://vaultdb.com.br/sla)

---

## Open source philosophy

VaultDB is open source because backup processes benefit from:
- transparency
- shared operational knowledge
- community review

Open source improves defaults and patterns —  
**it does not remove operational responsibility**.

---

## Who should use VaultDB

- Developers responsible for production data
- Small teams without a dedicated infrastructure team
- Projects where losing data has real technical or financial impact
- Anyone who needs predictability, not improvisation

---

## Who should not use VaultDB

- Disposable test environments
- Projects without critical data
- Scenarios where backups are treated as an afterthought

---

## Getting started

Documentation and setup guides are evolving.  
For now, VaultDB is intended for users comfortable with production environments and infrastructure concepts.

👉 Visit: https://vaultdb.com.br

---

## Contributing

Contributions are welcome.

Before contributing:
- Understand the project philosophy
- Focus on reliability and clarity
- Avoid adding features that promise guarantees the system cannot provide

More details will be available in `CONTRIBUTING.md`.

---

## License

This project is open source.  
License details will be defined and published soon.

---

## Final note

If losing data is not an option,  
backup must be a process — not an afterthought.


# VaultDB

**VaultDB** é um gerenciador de backup open source criado para estruturar processos de backup confiáveis em sistemas reais de produção.

Backup não é uma ferramenta.  
Backup é um processo — e o VaultDB existe para tornar esse processo previsível, auditável e automatizado.

---

## Por que o VaultDB existe

Em muitos projetos pequenos e médios, backups são tratados como:
- scripts frágeis
- rotinas manuais
- processos não testados
- suposições implícitas de que “vai funcionar quando precisar”

O VaultDB foi criado para substituir improvisos por um **processo estruturado de backup**, focado em confiabilidade — não em promessas.

---

## O que o VaultDB é

- Um **gerenciador de backup open source** para bancos de dados em produção
- Uma ferramenta para **automatizar e estruturar processos de backup**
- Projetado para **sistemas reais com dados reais**
- Focado em **processo, observabilidade e previsibilidade**
- Adequado para **pequenos times e projetos individuais** em crescimento

---

## O que o VaultDB não é

- Uma solução mágica que garante zero perda de dados
- Um substituto para boas práticas operacionais
- Um gerador genérico de scripts de backup
- Uma ferramenta “configurar e esquecer” sem responsabilidade

---

## Princípios fundamentais

- **Processo acima da ferramenta**  
  Confiabilidade vem de processos bem definidos, não apenas de código.

- **Separação de responsabilidades**  
  Execução, armazenamento e restauração não devem depender do mesmo ponto de falha.

- **Restauração previsível**  
  Um backup só é útil se o processo de restauração for claro, testável e repetível.

- **Transparência**  
  O open source permite revisão, discussão e padrões mais seguros.

---

## Como o VaultDB funciona (visão geral)

1. **Conexão segura**  
   Configure o acesso ao banco de dados ou ambiente de produção com permissões mínimas.

2. **Backups automatizados**  
   Backups são executados automaticamente conforme a estratégia definida, sem ações manuais.

3. **Armazenamento separado**  
   Os dados de backup são armazenados fora do ambiente principal, evitando ponto único de falha.

4. **Restauração controlada**  
   O processo de restauração segue fluxos previsíveis, reduzindo improvisos em situações críticas.

---

## Observabilidade e analytics

O VaultDB utiliza **analytics server-side** para acompanhar sinais reais de funcionamento do produto.

- Eventos são gerados **exclusivamente pelo backend**
- O conteúdo dos backups **nunca é acessado**
- Eventos representam **resultados operacionais**, não cliques ou navegação

Exemplo de evento real de produto:
- `first_backup_success` — disparado somente quando um backup é concluído com sucesso pela primeira vez

Esses eventos ajudam a evoluir o produto sem comprometer privacidade ou segurança.

---

## Privacidade e responsabilidade

- O VaultDB **não acessa o conteúdo dos backups**
- Apenas metadados operacionais mínimos são processados
- Nenhum dado pessoal é vendido ou compartilhado
- A responsabilidade operacional permanece com o usuário, incluindo:
  - validação de backups
  - testes de restauração
  - políticas de retenção

Veja também:
- [Política de Privacidade](https://vaultdb.com.br/privacy)
- [Política de Segurança](https://vaultdb.com.br/security)
- [SLA](https://vaultdb.com.br/sla)

---

## Filosofia open source

O VaultDB é open source porque processos de backup se beneficiam de:
- transparência
- conhecimento operacional compartilhado
- revisão pela comunidade

O código aberto melhora padrões e práticas —  
**não elimina a responsabilidade operacional**.

---

## Para quem o VaultDB é indicado

- Desenvolvedores responsáveis por dados em produção
- Pequenos times sem equipe dedicada de infraestrutura
- Projetos onde perder dados gera impacto real
- Quem precisa de previsibilidade, não improviso

---

## Para quem o VaultDB não é indicado

- Ambientes descartáveis de teste
- Projetos sem dados críticos
- Cenários onde backup é tratado como detalhe secundário

---

## Começando

A documentação e os guias de configuração estão em evolução.

Atualmente, o VaultDB é indicado para usuários com familiaridade com:
- ambientes de produção
- bancos de dados
- conceitos básicos de infraestrutura

👉 Saiba mais em: https://vaultdb.com.br

---

## Contribuindo

Contribuições são bem-vindas.

Antes de contribuir:
- compreenda a filosofia do projeto
- priorize confiabilidade e clareza
- evite adicionar promessas que o sistema não pode garantir

Mais detalhes estarão disponíveis em `CONTRIBUTING.md`.

---

## Licença

Este projeto é open source.  
Os detalhes da licença serão definidos e publicados em breve.

---

## Nota final

Se perder dados não é uma opção,  
backup precisa ser um processo — não uma improvisação.
