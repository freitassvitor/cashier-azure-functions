# Delta1 Cashier — Azure Functions

Repositório das Azure Functions (Python, `IoTHubTrigger` — D003, D035): processamento
downstream dos eventos que os hubs enviam ao IoT Hub.

O contexto global do projeto — arquitetura, decisões, status dos módulos e regras para
todos os agentes — vive no repositório irmão `cashier-documentation`, importado abaixo.
Ele fica ao lado deste repo (`../cashier-documentation/`; no dev container,
`/workspaces/cashier-documentation/`), junto com `scope.txt`, `payloads.txt`,
`cloud_scope.txt`, `panel.json` e `decisions-log.md`.

@../cashier-documentation/CLAUDE.md

## Neste repositório

- Agente: `functions` (`.claude/agents/functions.md`, comando `/functions`)
- Dev container: Python 3.12 + Azure Functions Core Tools v4 + Azurite + Azure CLI;
  host local na porta 7071 (`func start`), Azurite com `azurite --location /tmp/azurite`
- O formato dos eventos vem da fila de sync do hub (`events/` no `delta1-cashier`,
  montado em `/workspaces/delta1-cashier`)
- Configuração: `local.settings.json` (não versionado) em desenvolvimento
- O projeto das Functions ainda não foi criado
