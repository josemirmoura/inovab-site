# InovaB | Site público e conteúdo editorial

**Escopo:** conteúdo e identidade do site público `inovab.hubbr.org`, separado da área administrativa e dos portais institucionais da UEPB e UFCG.

> **Ponto de entrada obrigatório para o Codex:** **[Índice do kit editorial completo](conteudo/INDICE_PARA_CODEX.md)**. Ali estão os links para os três artigos integrais, as quatro ilustrações SVG, as três minutas legais, a página **InovaB na mídia** (UEPB e SantoTech) e as instruções de rodapé, SEO/AEO, temas claro/escuro e validação.

## Materiais já preparados

- **Três artigos completos**, cada um com imagem original e metadados editoriais, em [`conteudo/blog/`](conteudo/blog/).
- **Três minutas de políticas** (Privacidade, Cookies e Termos de Uso), em [`conteudo/politicas/`](conteudo/politicas/). **Requerem auditoria dos tratamentos/cookies e revisão institucional/jurídica**, com preenchimento dos campos `[VALIDAR]` antes de publicação.
- **Página de cobertura jornalística:** [InovaB na mídia](conteudo/inovab-na-midia.md), com referências externas da [UEPB](https://uepb.edu.br/software-desenvolvido-na-uepb-recebe-registro-do-inpi-e-favorece-identificacao-de-pesquisas-com-potencial-inovador/) e [SantoTech](https://santotech.com.br/inovab-uepb-identifica-pesquisas-potencial-inovacao/).
- **Imagens originais SVG:** [`imagens/`](imagens/). São recursos vetoriais pequenos, sem depender de fotos de terceiros.
- **Identidade visual NCTI-PB:** as quatro versões de logotipo serão anexadas pelo usuário **diretamente ao chat do Codex**; não presumir que arquivos enviados ao ChatGPT já estejam neste repositório.

## Regras fundamentais

1. Aplicar o conteúdo **apenas ao site público `inovab.hubbr.org`**. A UEPB é instituição efetivamente atendida; UFCG ainda não deve constar como cliente contratado.
2. No cabeçalho, UEPB + NCTI-PB horizontal; no rodapé, NCTI-PB compacta. Usar **colorido no tema claro** e **branco sobre fundo transparente no escuro**.
3. Exibir seção **Instituições que utilizam o InovaB** com UEPB. Exibir seção **Ecossistema de Inovação** com logo **INOVATEC colorida**, em card branco arredondado, inclusive no tema escuro. A menção INOVATEC é intencional e não deve desaparecer da seção de parceiros.
4. **Rodapé deve conter o link “InovaB na mídia”** para `/inovab-na-midia`, além das políticas legais validadas e acesso a contato/feedback.
5. **Nenhuma publicação/deploy é autorizada por esses arquivos.** O host raiz pode ainda servir à aplicação UEPB em produção. Fazer inventário e staging primeiro; preservar totalmente a aplicação atual. Trabalhos devem ter PR, testes e aceite antes do corte.
6. Não inventar dados, funcionalidades, autores ou datas. Os artigos estão em formato de rascunho com `datePublished: null`; preencher na publicação real. Não exibir políticas com campos `[VALIDAR]` ao público.

## Relação com os canônicos de desenvolvimento

O repositório **privado** [`josemirmoura/inovab`](https://github.com/josemirmoura/inovab) contém os planos de arquitetura e continuidade. Consultar o documento `docs/INOVAB_SITE_PUBLICO_OBSERVACOES_2026-10-30.md` e o runbook de preservação da produção antes de alterar qualquer serviço.

A área de pesquisa será discutida em etapa posterior e **não faz parte deste pacote editorial**.
