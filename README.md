# NEX NetOps Portal

Painel de diagnóstico e documentação de rede da NexTelecom.

## Acesso

URL: https://netops.nextelecom.com.br
Auth: Basic Auth (usuários configurados no servidor)

## Estrutura

```
sites/
├── index.html              ← Portal principal
├── favicon/                ← Ícones
├── rede/
│   └── escritorio-pqs-1andar/
│       ├── index.html      ← Dashboard rack + patch panels
│       ├── mapa.html       ← Mapa interativo de rede
│       └── mapa_rede_1andar.png
└── ferramentas/            ← Em desenvolvimento
```

## Deploy

Os arquivos são servidos diretamente via nginx (volume bind-mount em /opt/netops/sites).
Não é necessário build — editar e salvar já reflete no portal.

## Tecnologias

- HTML5 / CSS3 / JavaScript (vanilla)
- Nginx (Docker) com Basic Auth e SSL
