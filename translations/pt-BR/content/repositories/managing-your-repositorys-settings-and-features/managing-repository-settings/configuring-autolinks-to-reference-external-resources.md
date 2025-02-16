---
title: Configurar links automáticos para fazer referência a recursos externos
intro: Você pode adicionar links automáticos para recursos externos como problemas do JIRA e tíquetes do Zendesk a fim de ajudar a otimizar o fluxo de trabalho.
product: '{% data reusables.gated-features.autolinks %}'
redirect_from:
  - /articles/configuring-autolinks-to-reference-external-resources
  - /github/administering-a-repository/configuring-autolinks-to-reference-external-resources
  - /github/administering-a-repository/managing-repository-settings/configuring-autolinks-to-reference-external-resources
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Repositories
shortTitle: Configurar links automáticos
---

Qualquer pessoa com permissões de administrador para um repositório pode configurar referências de autolink para vincular problemas, pull requests, mensagens do commit e descrições de versões para serviços externos de terceiros.

Se você usa o Zendesk para acompanhar tíquetes relatados pelo usuário, por exemplo, é possível fazer referência a um número de tíquete na pull request que você abre para corrigir o problema.

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-settings %}
{% ifversion fpt or ghec or ghes > 3.4 or ghae-issue-5658 %}
1. In the "Integrations" section of the sidebar, click **{% octicon "cross-reference" aria-label="The cross-reference icon" %} Autolink references**.
{% else %}
1. Na barra lateral esquerda, clique em **Autolink references** (Referências de link automático). ![Guia Autolink references (Referências de link automático) na barra lateral esquerda](/assets/images/help/repository/autolink-references-tab.png)
{% endif %}
1. Clique em **Add autolink reference** (Adicionar referência de link automático). ![Botão para preencher informações de referência de link automático](/assets/images/help/repository/add-autolink-reference-details.png)
5. Em "Reference prefix" (Prefixo da referência), digite um prefixo curto e significativo que os colaboradores devem usar para gerar links automáticos para os recursos externos. ![Campo para digitar abreviação de sistema externo](/assets/images/help/repository/add-reference-prefix-field.png)
6. Em "Target URL" (URL de destino), digite o link para o sistema externo com o qual deseja criar vínculo. Certifique-se de manter `<num>` como uma variável para o número de referência. ![Campo para digitar URL para sistema externo](/assets/images/help/repository/add-target-url-field.png)
7. Clique em **Add autolink reference** (Adicionar referência de link automático). ![Botão para adicionar referência de link automático](/assets/images/help/repository/add-autolink-reference.png)
