# Brazil Travel Tips - Staging Package

Data: 2026-06-14

## Objetivo

Esta pasta contem uma versao de staging do `braziltraveltips.com` para teste visual, tecnico e editorial antes de apontar o dominio oficial.

Esta versao serve para:

- testar navegacao;
- testar mobile;
- validar Age Gate 18+ em Premium Services;
- revisar links internos;
- medir Core Web Vitals;
- testar `robots.txt`, `sitemap.xml` e `llms.txt`;
- preparar Search Console e analytics;
- revisar trust pages antes da publicacao oficial.

## Arquivos Incluidos

Páginas publicaveis em staging:

- `index.html`
- `homepage-braziltraveltips-hybrid.html`
- `page-brazil-travel-braziltraveltips.html`
- `page-rio-de-janeiro-braziltraveltips.html`
- `page-rio-nightlife-braziltraveltips.html`
- `page-rio-business-travel-braziltraveltips.html`
- `page-sao-paulo-braziltraveltips.html`
- `page-sao-paulo-business-travel-braziltraveltips.html`
- `page-sao-paulo-nightlife-braziltraveltips.html`
- `page-hotels-and-areas-braziltraveltips.html`
- `page-safety-and-etiquette-braziltraveltips.html`
- `page-premium-services-braziltraveltips.html`
- `page-about-braziltraveltips.html`
- `page-editorial-policy-braziltraveltips.html`
- `page-privacy-braziltraveltips.html`
- `page-terms-braziltraveltips.html`
- `page-contact-braziltraveltips.html`

Arquivos tecnicos:

- `robots.txt`
- `sitemap.xml`
- `llms.txt`
- `trust-pages-braziltraveltips.css`
- `assets/images/`

Arquivos de validacao:

- `age-gate-premium-validation.png`
- `age-gate-premium-validation-mobile-v5.png`

## Nao Incluido

Ficaram fora do staging:

- relatorios internos;
- matrizes editoriais;
- briefs;
- arquivos QA;
- proposta visual antiga;
- design system;
- componente isolado do Age Gate;
- documentos markdown internos.

## Status Atual

Pode subir para staging:

`Sim`

Pode apontar dominio oficial como lancamento publico:

`Ainda nao recomendado`

## Pendencias Antes de Lancamento Oficial

- escolher stack/hospedagem final;
- configurar dominio `braziltraveltips.com`;
- configurar CDN/cache;
- configurar analytics;
- configurar Google Search Console e Bing Webmaster Tools;
- medir Core Web Vitals em ambiente publicado;
- revisar links internos;
- validar links externos para parceiros;
- revisar juridicamente Privacy Policy e Terms of Use;
- decidir se `/premium-services/` sera indexavel no lancamento inicial;
- criar regra final para links externos adultos exigirem Age Gate antes da saida;
- definir se staging deve ter senha ou `noindex`.

## Recomendacao de Hospedagem Staging

Para teste, usar uma destas opcoes:

1. Netlify ou Vercel com URL temporaria e sem apontar dominio principal.
2. Cloudflare Pages com branch/preview.
3. Subdominio temporario como `staging.braziltraveltips.com`, preferencialmente com `noindex`.

Recomendacao:

Subir primeiro em URL temporaria privada ou semi-privada. Depois de validar mobile, velocidade, links, Age Gate e politicas, decidir o lancamento oficial.

## Testes Minimos no Staging

- abrir homepage;
- navegar para Rio, Sao Paulo, Safety, Hotels, Premium Services, About, Privacy, Terms e Contact;
- confirmar se Premium Services mostra Age Gate;
- clicar `I am 18 or older`;
- recarregar Premium Services e confirmar que o gate nao reaparece durante a validade;
- limpar localStorage e confirmar que o gate reaparece;
- testar mobile;
- testar sitemap;
- testar robots;
- rodar Lighthouse/Core Web Vitals;
- revisar se nenhuma pagina interna de planejamento ficou acessivel.
