# Integração com o homelab

## Contrato entre os projetos

O RPG é um produto independente. Hospedagem no homelab é uma opção planejada, não uma implantação existente. O produto deve documentar suas necessidades sem presumir hosts, portas, domínios ou recursos disponíveis.

| Responsabilidade | Fonte |
|---|---|
| Produto, funcionalidades, interface, código e testes | Repositório RPG Platform |
| Arquitetura e configuração parametrizada da aplicação | Repositório RPG Platform |
| Host, ingresso Cloudflare, redes e exposição efetiva | Documentação canônica do homelab |
| Volumes, destinos de backup, monitoramento e recuperação do ambiente | Documentação canônica do homelab |
| Instruções de operação específicas da aplicação | Repositório RPG Platform, referenciado pelo homelab |

## Como carregar o contexto

O clone conhecido nesta máquina é D:\HOMELAB. HOMELAB_DOCS_PATH pode ser usado para indicar outro clone. Não é requisito de execução do aplicativo e não concede acesso por si só.

Antes de propor hospedagem, ler no clone canônico: AGENTS.md, docs/index.md, docs/governance/status-model.md, docs/governance/agent-operating-guide.md, docs/governance/source-of-truth.md, docs/architecture/canonical-topology.md, o snapshot mais recente e os documentos de data/, hosts, ingresso web e backups pertinentes.

Informar a revisão e as datas consultadas. Capacidade e estado atuais exigem evidência recente. Não copiar o inventário para este repositório nem usar conversas antigas como substituto.

## Decisões necessárias antes da implantação

- Tamanho, tipos e retenção dos mapas e outros arquivos.
- Requisitos de colaboração em tempo real e número de sessões simultâneas.
- Persistência, armazenamento de arquivos e processo de restauração.
- Autenticação, autorização, convites e exposição pública/administrativa.
- Recursos mínimos, limites, observabilidade e orçamento.
- Escolha de hospedagem, estratégia de publicação e rollback.

Após definição, registrar a implantação real no inventário do homelab, com link para este repositório e sem duplicação de procedimentos. Não alterar servidores, DNS, Cloudflare ou volumes durante a descoberta do produto.
