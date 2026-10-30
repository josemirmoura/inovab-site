# InovaB | Kit editorial para implementação no site público

**Concluído em:** 30/10/2026.  
**Estado:** arquivos-fonte completos já gravados no GitHub; **nenhum conteúdo foi publicado no domínio** por este registro.  
**Escopo exclusivo:** `https://inovab.hubbr.org`. **Não aplicar automaticamente em `admin.inovab.hubbr.org`, `uepb.inovab.hubbr.org` ou `ufcg.inovab.hubbr.org`.**  
**Referência canônica privada:** `josemirmoura/inovab/docs/INOVAB_SITE_PUBLICO_OBSERVACOES_2026-10-30.md`.

## 1. Inventário de arquivos prontos

| Tipo | Título ou função | Arquivo fonte | Recurso visual | Rota sugerida |
|---|---|---|---|---|
| Artigo completo | Como identificar oportunidades de inovação em pesquisas universitárias? | [Artigo 1](blog/como-identificar-oportunidades-inovacao-pesquisas-universitarias.md) | [SVG 1](../imagens/identificar-oportunidades-inovacao.svg) | `/blog/como-identificar-oportunidades-inovacao-pesquisas-universitarias` |
| Artigo completo | O papel da inteligência tecnológica na transferência de conhecimento das universidades | [Artigo 2](blog/inteligencia-tecnologica-transferencia-conhecimento-universidades.md) | [SVG 2](../imagens/inteligencia-tecnologica-transferencia.svg) | `/blog/inteligencia-tecnologica-transferencia-conhecimento-universidades` |
| Artigo completo | Como o InovaB transforma repositórios acadêmicos em fontes de oportunidades de inovação | [Artigo 3](blog/como-inovab-transforma-repositorios-academicos-em-oportunidades.md) | [SVG 3](../imagens/repositorios-oportunidades-inovab.svg) | `/blog/como-inovab-transforma-repositorios-academicos-em-oportunidades` |
| Notícias externas | InovaB na mídia (UEPB + SantoTech, 28/10/2026) | [Página de mídia](inovab-na-midia.md) | [SVG mídia](../imagens/inovab-na-midia.svg) | `/inovab-na-midia` |
| Política legal | Política de Privacidade | [Minuta](politicas/politica-de-privacidade.md) | Não necessário | `/politica-de-privacidade` |
| Política legal | Política de Cookies | [Minuta](politicas/politica-de-cookies.md) | Não necessário | `/politica-de-cookies` |
| Política legal | Termos de Uso | [Minuta](politicas/termos-de-uso.md) | Não necessário | `/termos-de-uso` |

**Os artigos têm texto integral** (não placeholders), frontmatter de SEO, links de referência, FAQ e descrição/alt da imagem. As quatro imagens são **SVGs originais, pequenos e editáveis** (não cópias de reportagens, terceiros ou bancos de imagens). Não substituir por imagens genéricas sem necessidade. O Codex deve validar XML, acessibilidade, nitidez e compressão no build.

**A página de mídia contém as duas referências externas reais:** portal institucional UEPB e SantoTech. Revalidar URLs antes de publicar e evitar copiar fotos ou textos protegidos.

## 2. Como encaixar na home

**Seção:** `Conhecimento & Inovação` (três cards, responsivos, na ordem abaixo).

**Card 1**
- Título: **Como identificar oportunidades de inovação em pesquisas universitárias?**
- Resumo: **Entenda quais resultados acadêmicos merecem atenção, como organizar uma triagem confiável e por que a análise humana continua indispensável.**
- Imagem: `/imagens/identificar-oportunidades-inovacao.svg`.
- Link: `/blog/como-identificar-oportunidades-inovacao-pesquisas-universitarias`.

**Card 2**
- Título: **Inteligência tecnológica e transferência de conhecimento**
- Resumo: **Conheça práticas que ajudam universidades e NITs a conectar resultados científicos, informações tecnológicas e necessidades da sociedade.**
- Imagem: `/imagens/inteligencia-tecnologica-transferencia.svg`.
- Link: `/blog/inteligencia-tecnologica-transferencia-conhecimento-universidades`.

**Card 3**
- Título: **Do repositório acadêmico à triagem de oportunidades**
- Resumo: **Veja como o InovaB organiza registros, aplica classificações exploratórias e apoia a revisão especializada da produção acadêmica.**
- Imagem: `/imagens/repositorios-oportunidades-inovab.svg`.
- Link: `/blog/como-inovab-transforma-repositorios-academicos-em-oportunidades`.

Adicionar link **Ver todos os artigos** somente se a rota `/blog` existir. Caso contrário, criar página índice com cards e links, sem links mortos.

**Seção instituições:** `Instituições que utilizam o InovaB` com card UEPB (instituição atendida). Não incluir UFCG como cliente sem contratação/autorização.

**Seção `Ecossistema de Inovação`:** card pequeno/médio com logomarca **UEPB-INOVATEC colorida**, fundo branco permanente, bordas arredondadas, inclusive em tema escuro. Essa menção INOVATEC é **intencional** e deve permanecer.

## 3. Rodapé: enlaces e identidade a implementar

**Institucional/Produto:**
- `InovaB na mídia` → `/inovab-na-midia` **(REQUISITO NOVO CONFIRMADO em 30/10/2026)**.
- `Como funciona` → `/como-funciona` se rota existente.
- `Instituições atendidas` → âncora ou rota real.
- `Contato e avaliações` → rota real validada.

**Privacidade e uso:**
- `Política de Privacidade` → `/politica-de-privacidade`.
- `Política de Cookies` → `/politica-de-cookies`.
- `Termos de Uso` → `/termos-de-uso`.
- `Preferências de cookies` → ação funcional somente se houver cookies opcionais que exijam consentimento e gerenciamento efetivo.

**Marca do rodapé:** NCTI-PB compacta **colorida no tema claro** / **branca no escuro**, utilizando os arquivos que o usuário anexará ao Codex. Cabeçalho: UEPB + NCTI-PB horizontal nas mesmas duas variantes. Remover INOVATEC **como identidade principal** do site público, mas **preservar INOVATEC** na faixa Ecossistema e referências históricas verdadeiras. Não mexer em nomes de serviços, tabelas, rotas internas de legado.

## 4. Publicação editorial: regras e validações

1. **Detectar o estado real da produção**: `inovab.hubbr.org` pode ainda hospedar a consulta da UEPB. Não substituir, redirecionar ou interromper sem migração/corte autorizados. Preparar site público em staging/branch e apresentar preview verificável.
2. **Artigos:** consumir Markdown/frontmatter (ou converter preservando texto integral), gerar páginas HTML sem conteúdo vazio, URLs estáveis, títulos H1, meta title/description, Open Graph/Twitter, canonical e schema `BlogPosting`/`Article` **somente com campos reais**. Preencher `author`, `datePublished`, `dateModified` apenas depois da aprovação editorial, sem inventar nomes/datas ou publicar datas de criação de arquivo como publicação real.
3. **Metadados e indexação:** sitemap XML e robots, links internos, auditoria de links externos; `noindex` em staging, controle de 404 e redirecionamentos após corte. SEO/AEO é conteúdo útil e rastreável, sem prometer posição ou inclusão em respostas de IA.
4. **Imagens:** servir SVG original no build ou gerar PNG/WebP com transparência se a infraestrutura não aceitar SVG; definir dimensões e `loading=lazy` nos cards, evitar CLS; não bloquear o LCP da home.
5. **Políticas:** os três arquivos são **minutas jurídicas completas, mas dependem de dados específicos para validade**. O Codex deve fazer inventário real de formulários, logs, cookies, scripts/terceiros, responsáveis e retenção. Todos os campos `[VALIDAR]` precisam ser resolvidos por evidência e validados juridicamente; **não publicar texto com placeholders nem afirmar funcionalidades fictícias**. Sem inventário, manter em revisão e reportar pendência.
6. **Mídia:** usar títulos como referência e **resumos originais**. Não reproduzir textos/fotos das reportagens ou afirmar que são material de autoria do InovaB; conferir a disponibilidade dos dois links antes da publicação.
7. **Qualidade:** testar desktop/mobile, tema claro/escuro, navegação por teclado, contraste, suporte a acentos, imagens, links, headings, conteúdo renderizado, logs e desempenho.
8. **Segurança e continuidade:** nenhum comando de deploy, banco, DNS, proxy, mudança da API ou pipeline está autorizado por este kit. Produção deve permanecer funcional, especialmente se os créditos do Codex acabarem.

## 5. Ordem de trabalho recomendada

- **R0:** identificar repositório/branch realmente responsável pelo site público e a situação de `inovab.hubbr.org`; sem mutações.
- **R1:** implementar, em staging, layout e homepage com cards de blog, clientes UEPB, ecossistema INOVATEC, rodapé com InovaB na mídia; anexar logos NCTI-PB fornecidas pelo usuário.
- **R2:** integrar artigos completos, página mídia e imagens; testar URLs e SEO.
- **R3:** auditar tratamento de dados/cookies, preencher minutas legais com dados reais e submeter à revisão; implementar preferências somente quando necessárias.
- **R4:** validar acessibilidade, mobile, temas, links, segurança e SEO; preparar PR e preview, sem cutover até autorização.

**Não há exigência de alterar os portais universitários, a área administrativa ou a área de pesquisa nesta rodada.** O usuário discutirá a área de pesquisa separadamente.

## 6. Referências de implementação

- [Plano de revisão exclusivo do site público](https://github.com/josemirmoura/inovab/blob/main/docs/INOVAB_SITE_PUBLICO_OBSERVACOES_2026-10-30.md) (repositório privado; necessita acesso).
- [Plano técnico de preservação do site e migração](https://github.com/josemirmoura/inovab/blob/main/docs/INOVAB_2_0_RUNBOOK_SEM_INDISPONIBILIDADE.md).
- [Artigo UEPB, 28/10/2026](https://uepb.edu.br/software-desenvolvido-na-uepb-recebe-registro-do-inpi-e-favorece-identificacao-de-pesquisas-com-potencial-inovador/).
- [Reportagem SantoTech, 28/10/2026](https://santotech.com.br/inovab-uepb-identifica-pesquisas-potencial-inovacao/).
- [ANPD: guia de cookies](https://www.gov.br/anpd/pt-br/centrais-de-conteudo/materiais-educativos-e-publicacoes/guia_orientativo_cookies_e_protecao_de_dados_pessoais).
