# Mercado Koala — Site de Divulgação

Site institucional desenvolvido como projeto escolar para a disciplina de **Desenvolvimento Frontend para Web** (A2 · 2026.2), sob orientação do Prof. Cid Andrade.

---

## 👥 Integrantes do Grupo

| Nome | RGM |
|------|----|
| Vitor Arruda Dos Santos | — |
| Marcelo Gabriel Alves | — |
| Veronica dos Santos Lima | — |
| Victor Correa | 47093102 |
| Felipe de Oliveira Brito | — |

---

## 🏪 Introdução — A Organização

O **Mercado Koala** é um mercado de bairro localizado na:

> **Rua Dr. Cristiano Altenfelder Silva, 515 — Vila Carrão, São Paulo - SP, CEP 03448-010**

Trata-se de um negócio familiar, fundado com o objetivo de oferecer aos moradores da Vila Carrão produtos frescos, atendimento próximo e preços justos. O mercado conta com seções de hortifrúti, açougue, padaria artesanal, mercearia, bebidas, laticínios e produtos de limpeza e higiene.

O site foi desenvolvido para **divulgar o mercado digitalmente**, apresentando a história da empresa, seus produtos e serviços, canais de contato e formulários de orçamento — tudo com estrutura semântica em HTML5 puro, conforme os requisitos da Entrega 1.

---

## 🗂️ Estrutura do Projeto

```
Koala Anúnco/
├── index.html               # Página Inicial
├── contato.html             # Página de Contato (formulário)
├── orcamento.html           # Página de Orçamento/Solicitação
├── paginas/
│   ├── sobre.html           # Quem Somos
│   ├── produtos.html        # Produtos & Serviços
│   ├── faq.html             # Perguntas Frequentes
│   ├── depoimentos.html     # Depoimentos & Avaliações
│   ├── trabalhe-conosco.html# Trabalhe Conosco
│   ├── parceiros.html       # Parceiros & Marcas
│   └── politica.html        # Política de Privacidade
├── assets/
│   ├── img/                 # Imagens (a adicionar)
│   ├── audio/               # Áudio (a adicionar no próximo commit)
│   └── video/               # Vídeo (a adicionar no próximo commit)
└── README.md
```

---

## 🔗 Link do Site Hospedado

> *(A ser preenchido após deploy no Netlify)*

---

## 🛠️ Desenvolvimento

### Contato com a Organização

O Mercado Koala é o negócio do pai de um dos integrantes do grupo (Marcelo Gabriel Alves),
o que garantiu acesso direto ao responsável para levantamento de informações reais sobre
endereço, funcionamento, serviços, produtos e diferenciais do estabelecimento.

A entrevista foi realizada de forma presencial, com visita ao mercado para coleta de informações.

> 📷 **Foto comprobatória do contato com o responsável:** *(a ser adicionada no próximo commit)*

### Processo de Desenvolvimento

#### Decisões de Estrutura

- Optamos por 10 páginas interligadas conforme o requisito, com páginas adicionais de conteúdo relacionadas aos serviços reais do mercado.
- A estrutura de pastas separa as páginas de conteúdo (`/paginas/`) dos arquivos raiz (`index.html`, `contato.html`, `orcamento.html`), seguindo a sugestão do enunciado.
- Todos os caminhos relativos foram cuidadosamente ajustados para manter a navegação funcional entre as pastas.

#### Semântica HTML5

Todas as páginas utilizam as seguintes tags semânticas obrigatórias:
- `<header>` — cabeçalho do site com nome e descrição
- `<nav>` — menu de navegação principal (com `aria-label`)
- `<main>` — conteúdo principal da página
- `<section>` — seções temáticas com `aria-labelledby`
- `<article>` — artigos/blocos de conteúdo independentes
- `<footer>` — rodapé com copyright e links

#### Formulários com Validação HTML5 Nativa

Três páginas contêm formulários com validação nativa:
- **contato.html** — formulário de contato com `type="email"`, `type="tel"`, `pattern`, `required`, `minlength`, `maxlength`
- **orcamento.html** — formulário de orçamento com campos específicos para pessoa física/jurídica, `type="date"`, `type="tel"`, `pattern` para CNPJ
- **trabalhe-conosco.html** — formulário de cadastro de currículo com `type="number"` (idade com `min`/`max`)

#### Placeholders para Áudio e Vídeo

As tags `<audio>` e `<video>` foram inseridas na página `produtos.html` com `<source>` apontando para arquivos em `assets/audio/` e `assets/video/`. Os arquivos reais serão adicionados em commit posterior.

#### Desafios Técnicos

- **Caminhos relativos:** ajuste dos caminhos (`../`) para as páginas dentro da pasta `/paginas/` acessarem corretamente `index.html`, `contato.html` e `orcamento.html`.
- **Validação W3C:** atenção ao fechamento correto de todas as tags, uso adequado de `aria-label` e `aria-labelledby`, evitar elementos depreciados.
- **Acessibilidade:** uso de `<abbr>` para indicar campos obrigatórios, `aria-current="page"` no menu para indicar a página ativa.

---

## ✅ Checklist da Entrega 1

- [x] 10 páginas HTML interligadas (index, contato, orçamento + 7 de conteúdo)
- [x] Estrutura semântica HTML5 em todas as páginas (`header`, `nav`, `main`, `section`, `article`, `footer`)
- [x] Formulário de contato com validação/máscaras nativas do HTML5
- [x] Tags `<audio>` e `<video>` incorporadas (placeholders — arquivos a adicionar)
- [ ] Código validado no W3C Validator *(a verificar após deploy)*
- [x] Repositório no GitHub, organizado em pastas
- [ ] README com foto do contato com o entrevistado *(a adicionar)*
- [ ] Site hospedado (Netlify) e link disponível no README *(a fazer após deploy)*
- [x] Organização real confirmada — Mercado Koala (será a mesma na Entrega 2)

---

## 📝 Conclusão

A Entrega 1 nos permitiu compreender na prática a importância da marcação semântica HTML5 para estruturar um site real. Trabalhar com uma organização conhecida facilitou o levantamento de informações e o planejamento das páginas.

O principal aprendizado foi perceber que uma boa estrutura HTML — mesmo sem nenhuma estilização — já organiza visualmente o conteúdo de forma compreensível, e que as escolhas semânticas impactam diretamente na acessibilidade e no SEO do site.

Os desafios envolveram principalmente o gerenciamento correto dos caminhos relativos entre arquivos em diferentes pastas e a atenção aos atributos de acessibilidade (`aria-*`). O grupo se organizou bem para dividir as páginas e manter um padrão consistente em todas elas.

Para a Entrega 2, o plano é incorporar o CSS com identidade visual inspirada no nome "Koala" e nas cores do mercado, além de adicionar os arquivos reais de áudio e vídeo.

---

*Projeto desenvolvido para fins acadêmicos — Disciplina de Desenvolvimento Frontend para Web, 2026.*
