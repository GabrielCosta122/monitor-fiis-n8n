# 📈 Monitor de FIIs — N8N Agent

Agente de automação criado no N8N que monitora Fundos de Investimento Imobiliário (FIIs) e envia alertas por e-mail quando o preço atinge o valor alvo definido.

## 🚀 Como funciona

1. **Schedule Trigger** — roda automaticamente a cada 1 hora
2. **Code Node** — lista os FIIs monitorados e seus preços alvo
3. **Loop Over Items** — processa um FII por vez
4. **HTTP Request** — busca o preço atual via API da [Brapi.dev](https://brapi.dev)
5. **IF Node** — compara o preço atual com o preço alvo
6. **Gmail** — envia e-mail de alerta quando o preço bate o alvo

## 🛠️ Tecnologias

- [N8N](https://n8n.io) — automação do fluxo
- [Brapi.dev](https://brapi.dev) — API de cotações brasileiras
- Gmail — notificações por e-mail
- JavaScript — estruturação dos dados

## 📦 Como importar o workflow

1. Acesse seu N8N
2. Clique em **"Add workflow"** → **"Import from file"**
3. Selecione o arquivo `.json` deste repositório
4. Configure seu token da Brapi.dev e sua conta Gmail
5. Ative o workflow!

## 📊 FIIs monitorados

| Ticker | Preço Alvo |
|--------|-----------|
| MXRF11 | R$ 9,10 |
| GARE11 | R$ 8,00 |
| KNSC11 | R$ 8,10 |
| BTCI11 | R$ 8,50 |
| VGIR11 | R$ 9,10 |
| VGHF11 | R$ 6,50 |

---
Desenvolvido como projeto da disciplina de Estrutura de Dados.
