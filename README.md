<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Barbati-hub/Barbati-hub/main/assets/header-dark.svg">
  <img alt="Douglas A. Barbati — Desenvolvedor Full Stack, remoto, Brasil" width="880" src="https://raw.githubusercontent.com/Barbati-hub/Barbati-hub/main/assets/header-light.svg">
</picture>

![Disponível para vagas remotas](https://img.shields.io/badge/Dispon%C3%ADvel%20para%20vagas%20remotas-1A7F37?style=flat-square)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/douglas-barbati-92429b108)

Disponível para vagas 100% remotas · LinkedIn: [linkedin.com/in/douglas-barbati-92429b108](https://linkedin.com/in/douglas-barbati-92429b108) · E-mail: [douglasltda51@gmail.com](mailto:douglasltda51@gmail.com)

Construo e mantenho software que comércio usa para trabalhar todo dia: PDV, delivery e agendamento, com cliente pagante em operação. Faço ponta a ponta — API em Node/TypeScript, front em Next.js, multi-tenant isolado no banco, PIX, bot de WhatsApp e o print-client Electron que imprime a comanda no balcão. Procuro vaga de desenvolvedor pleno, 100% remota.

## Produtos no ar

Software meu, rodando em produção hoje. Os links abrem o sistema real.

### [Cida Lanches](https://cidalanche.com.br)

Loja de delivery de uma lanchonete: cardápio, carrinho, pagamento por PIX e o pedido saindo impresso na cozinha.

Cliente pagante, em operação diária · `Next.js` `Express` `Prisma` `PostgreSQL` `PIX Sicoob` `ESC/POS`

### [Mozza](https://mozza.online)

SaaS de PDV e delivery multi-tenant que fundei e mantenho sozinho desde janeiro de 2024. Cada lojista tem sua loja, seu PWA, seu certificado de PIX e sua impressora, sem um lojista enxergar o dado do outro.

Loja demo: [loja.mozza.online](https://loja.mozza.online) · 1019 testes de backend e 455 de frontend · `Next.js App Router` `React` `Express` `Prisma 6` `PostgreSQL` `Electron` `Baileys` `Railway`

Por dentro: isolamento por `companyId` em toda a camada de dados; PIX Sicoob por lojista, com o certificado `.pfx` da própria loja e confirmação vinda do banco; Mercado Pago para a mensalidade do SaaS; impressão térmica ESC/POS via print-client Electron com fila local, que não perde comanda quando a internet cai; bot de WhatsApp com atendente de IA e revezamento IA ↔ humano; integrações com iFood (Entrega Sob Demanda) e Delivery Much.

### [Ateliê](https://atelie-lovat-three.vercel.app)

SaaS de agendamento para designer de unhas: vitrine pública, painel da profissional e um bot de WhatsApp que fecha o horário dentro da conversa.

`Next 16` `Tailwind 4` `shadcn/ui` `Better Auth` `Prisma 6` `PostgreSQL` `Vitest`

Por dentro: multi-tenant fail-closed em `$extends` do Prisma com AsyncLocalStorage — o slug da URL nunca autoriza nada, e divergência entre slug e sessão responde 404 em vez de 403, para não confirmar que a loja existe; anti-overbooking resolvido no banco com `EXCLUDE USING gist` e `btree_gist` sobre `tstzrange`, e não por checagem na aplicação, que perde a corrida; a fronteira de confiança do bot é limitada a exatamente três ferramentas, como defesa contra prompt injection; Vitest roda contra Postgres real, não contra mock.

## Stack

**Backend** `TypeScript` `Node.js` `Express` `Prisma 6` `Better Auth` `REST` `Vitest` `Jest`

**Frontend** `Next.js App Router` `React` `Tailwind 4` `shadcn/ui` `PWA` `Electron`

**Banco e dados** `PostgreSQL` `SQL` `multi-tenant por linha` `constraints de exclusão` `migrations`

**Infra e integrações** `Railway` `Vercel` `PIX Sicoob` `Mercado Pago` `Baileys (WhatsApp)` `ESC/POS` `iFood` `Delivery Much`

## Por que os repositórios estão privados

O que eu construí é software de cliente pagante: código de PDV, certificado de PIX de lojista e dado de venda de comércio real. Esse código não fica público, e os repositórios abertos aqui são exercícios antigos que não dizem nada sobre o que eu faço hoje.

Em conversa técnica ou entrevista eu abro o que for preciso: rodo o sistema ao vivo, mostro o schema e o isolamento multi-tenant, o fluxo de pagamento de ponta a ponta, a suíte de testes, e leio código junto. Só pedir.

---

![Disponível para vagas remotas](https://img.shields.io/badge/Dispon%C3%ADvel%20para%20vagas%20remotas-1A7F37?style=flat-square)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/douglas-barbati-92429b108)

Melhor canal: LinkedIn — [linkedin.com/in/douglas-barbati-92429b108](https://linkedin.com/in/douglas-barbati-92429b108). Por e-mail também funciona: [douglasltda51@gmail.com](mailto:douglasltda51@gmail.com). Respondo em até um dia útil.
