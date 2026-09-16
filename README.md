# 8 Automações de IA — Scripts n8n

Templates de workflow para o n8n (https://n8n.io), prontos para importar e adaptar.
Cada arquivo .json corresponde a uma das 8 automações do carrossel.

## Como importar
1. Abra o n8n (self-hosted ou n8n.cloud).
2. Crie um novo workflow em branco.
3. Menu (⋮) → "Import from File" → selecione o .json correspondente.
4. Configure as credenciais de cada nó (OpenAI, Google, Gmail, HubSpot, HeyGen, Apify etc.)
   nos campos indicados — os nós vêm com URLs/placeholders genéricos que você troca
   pelas suas chaves de API.
5. Ajuste os prompts e os campos de dados (`{{$json...}}`) conforme sua base de dados.

## O que cada script faz

| Arquivo | Automação | Principais integrações |
|---|---|---|
| 01_agente_chamadas_voz_ia.json | Agente de chamadas de voz com IA | Webhook, OpenAI Realtime, Google Calendar, Gmail, HubSpot |
| 02_ia_geracao_leads.json | IA para geração de leads | Apify, OpenAI, Gmail |
| 03_gerador_spy_anuncios_ugc.json | Spy de anúncios UGC com IA | OpenAI (visão + texto), Google Sheets |
| 04_videos_ia_sem_rosto.json | Vídeos animados de IA sem rosto | OpenAI, provedor de vídeo (HeyGen/Creatify), agregador social |
| 05_agente_criacao_conteudo.json | Agente de criação de conteúdo | OpenAI, provedor de vídeo, agregador social (multi-plataforma) |
| 06_chatbot_multilingue_faq.json | Chatbot multilíngue de FAQ | Webhook, OpenAI |
| 07_gerador_ideias_youtube.json | Gerador de ideias virais do YouTube | YouTube API, OpenAI, Google Sheets |
| 08_gerador_avatar_ia.json | Gerador de avatar com IA | OpenAI, HeyGen |

## Importante
Estes workflows são **pontos de partida**: os nós de HTTP Request para serviços como
HeyGen, Apify, agregadores de redes sociais etc. usam URLs de exemplo — troque pela
documentação oficial de cada API e pelas suas credenciais antes de ativar o workflow.

— @techleadsacademy
