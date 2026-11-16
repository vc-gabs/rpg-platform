# Instruções para agentes

Este é o projeto RPG Platform. Responda em português do Brasil e leia README.md e docs/ antes de propor implementação.

## Produto

- Diferencie requisito confirmado, proposta, decisão pendente e funcionalidade implementada.
- Registre decisões relevantes em docs/decisions.md e mantenha o plano em docs/roadmap.md.
- Não escolha uma arquitetura distribuída apenas porque o produto pretende crescer. Justifique decisões por necessidades observáveis.
- Considere isolamento entre usuários e campanhas, autorização por recurso e proteção das notas privadas do mestre desde o desenho inicial.
- Peça as referências de sites de Gabriel e extraia os requisitos antes de definir a direção visual. Não copie marcas, código ou materiais de terceiros.
- Não trate mapa interativo, grade, tokens, neblina de guerra ou multiplayer em tempo real como requisitos aprovados: somente adicionar e organizar mapas foi confirmado até agora.

## Homelab

O código do RPG e suas decisões de produto pertencem a este repositório. A documentação de implantação pertence ao repositório canônico do homelab.

Para planejar hospedagem, consulte docs/homelab-integration.md. O clone local conhecido é D:\HOMELAB; HOMELAB_DOCS_PATH pode indicar outro local. A referência não concede acesso automaticamente: confirme a disponibilidade antes de afirmar fatos.

Leia as orientações do clone do homelab, o modelo de status, a topologia, o snapshot mais recente e os inventários pertinentes. Não copie o inventário operacional para este projeto. Não use chats antigos como fonte atual de hosts, portas, capacidade ou Cloudflare.

Se o clone estiver inacessível, continue o trabalho de produto e declare bloqueio apenas nas decisões que dependem da infraestrutura. Não entre nos servidores para contornar a ausência documental.

Nenhuma tarefa de produto autoriza por si só mudanças em servidores, DNS, Cloudflare, redes, volumes ou credenciais. Uma implantação exige proposta concreta com impacto, verificação, rollback e autorização correspondente.

## Segurança e publicação

- Nunca versione credenciais, tokens, cookies, chaves, .env real, dados pessoais, dumps ou uploads de usuários.
- Use dados fictícios e .env.example com placeholders quando houver configuração.
- Não copie configurações privadas do homelab para este repositório.
- Mantenha os originais e alterações do usuário; não faça limpeza destrutiva.
- Antes de tornar o repositório público, revise conteúdo, dados, histórico e licença. O repositório inicial é privado.
