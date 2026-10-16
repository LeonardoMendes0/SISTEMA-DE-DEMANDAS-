# Sistema de Gestão de Demandas

Protótipo de sistema web para **organizar, distribuir e acompanhar demandas de atendimento** de uma equipe: cada atendente vê e atualiza as próprias demandas, e o administrador acompanha tudo em um painel com indicadores e gráficos.

Criei o projeto para resolver um problema real de rotina administrativa: demandas recebidas por vários canais, controladas em planilhas soltas, sem visão clara de quem está cuidando de quê, do que é urgente e do que já foi concluído.

> **Status:** protótipo funcional de front-end. Os dados ficam no navegador (`localStorage`) e vêm com exemplos fictícios. A próxima etapa é a integração com Google Sheets (veja [Próximos passos](#próximos-passos)).

## Funcionalidades

**Acesso por perfil**
- Login com dois perfis: **atendente** e **administrador**
- Cada atendente vê apenas as demandas atribuídas a ele

**Gestão das demandas**
- Tabela com data de recebimento, solicitante, contato, resumo, urgência, atendente responsável e status
- Status em três etapas: **Aberta → Em andamento → Concluída**, com atualização em um clique
- Destaque visual para demandas urgentes
- Filtros por status, atendente, urgência e data
- Anexos por demanda (simulados no protótipo)

**Painel administrativo**
- Indicadores: total de demandas, urgentes, taxa de conclusão e demandas do mês
- Gráficos com Chart.js: demandas por status, por atendente, evolução mensal e urgências por atendente
- Visão consolidada de todas as demandas da equipe

## Tecnologias

- HTML5, CSS3 (layout responsivo com Flexbox e Grid)
- JavaScript puro (sem framework)
- [Chart.js](https://www.chartjs.org/) para os gráficos
- Font Awesome para os ícones
- `localStorage` para manter sessão e dados no navegador

## Como rodar

Não precisa instalar nada.

1. Baixe ou clone o repositório
2. Abra o arquivo HTML da pasta `PROJETO PESSOAL - NOVO` no navegador

**Usuários de demonstração** (fictícios, definidos no próprio código):

| Perfil | E-mail | Senha |
|---|---|---|
| Administrador | `admin@humanizacao.com` | `admin123` |
| Atendente | `maria@humanizacao.com` | `senha123` |

## Próximos passos

- [ ] Integrar com **Google Sheets via Google Apps Script**, usando a planilha como base de dados compartilhada pela equipe
- [ ] Trocar o login de demonstração por autenticação real
- [ ] Cadastro de novas demandas pela própria interface
- [ ] Filtro de data completo e indicadores calculados a partir das datas reais
- [ ] Upload real de anexos
- [ ] Publicar uma demonstração online com GitHub Pages

## Autor

**Leonardo Candido Mendes**
[LinkedIn](https://www.linkedin.com/in/leonardo-candido-mendes-74952719b/) · [GitHub](https://github.com/LeonardoMendes0)
