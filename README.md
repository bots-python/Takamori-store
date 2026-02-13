# 🤖 VIREX STORE - Bot Discord Completo

Bot Discord profissional com sistema de vendas e logs integrados.

## 📋 Funcionalidades

### 💰 Sistema de Vendas
- Criar produtos com imagens
- Painéis dropdown com múltiplas opções
- Sistema de carrinho automático
- Integração com PIX
- Aprovação de pagamentos
- Gestão de comprovantes

### 📊 Sistema de Logs
- Logs de entradas e saídas
- Logs de mensagens (edição e deleção)
- Logs de bans
- Logs de alterações em cargos
- Logs de canais
- Logs de movimentação de voz

### 🛠️ Utilidades
- Bot em canal de voz (24/7 mutado)
- Ban fake (brincadeira)
- Painel de configuração completo

## 🚀 Deploy no Railway

### 1. Criar conta no Railway
Acesse: https://railway.app/

### 2. Criar novo projeto
- Clique em "New Project"
- Selecione "Deploy from GitHub repo" (ou "Empty Project")

### 3. Fazer upload dos arquivos
Faça upload destes arquivos:
- `bot_virex_store.py`
- `requirements.txt`
- `Procfile`

### 4. Configurar variáveis de ambiente
No Railway, vá em Settings > Variables e adicione:

```
DISCORD_TOKEN=SEU_TOKEN_AQUI
```

**⚠️ IMPORTANTE:** Nunca compartilhe seu token!

### 5. Deploy
- O Railway fará o deploy automaticamente
- Aguarde alguns minutos
- Verifique os logs em "Deployments"

## 🔑 Como obter o Token do Discord

1. Acesse: https://discord.com/developers/applications
2. Clique em "New Application"
3. Dê um nome ao bot (ex: VIREX STORE)
4. Vá em "Bot" no menu lateral
5. Clique em "Reset Token" e copie o token
6. **Habilite as Intents:**
   - Presence Intent
   - Server Members Intent
   - Message Content Intent
7. Vá em "OAuth2" > "URL Generator"
8. Selecione:
   - Scopes: `bot` e `applications.commands`
   - Bot Permissions: `Administrator`
9. Copie a URL gerada e convide o bot ao servidor

## 📝 Comandos Disponíveis

### Comando Principal
```
/ajudavirexstore - Ver todos os comandos
```

### Sistema de Vendas
```
/setup - Painel de configuração
/botvoz <canal> - Bot entra em voz
/banfake <membro> - Ban fake (brincadeira)
```

### Sistema de Logs
```
/setuplogs <tipo> <canal> - Configurar logs
```

Tipos de log disponíveis:
- 📥 Entradas
- 📤 Saídas
- 💬 Mensagens
- ✏️ Edição
- 🗑️ Delete
- 🔨 Ban
- 🎭 Cargos
- 📁 Canais
- 🔊 Voz

## ⚙️ Configuração Inicial

1. Use `/setup` para acessar o painel
2. Configure a categoria onde serão criados os carrinhos
3. Configure as informações do PIX
4. Crie seus produtos
5. Envie os painéis nos canais desejados

## 🎨 Imagem para /botvoz

Você pode usar qualquer imagem. Exemplos:
```
https://i.imgur.com/exemplo.gif
https://cdn.discordapp.com/attachments/...
```

## 🐛 Solução de Problemas

### Bot não responde aos comandos
- Verifique se o bot está online
- Confirme que todas as Intents estão habilitadas
- Use `/ajudavirexstore` para testar

### Erro ao conectar em voz
- O PyNaCl já está instalado no requirements.txt
- Reinicie o bot após o deploy

### Token inválido
- Gere um novo token no Discord Developer Portal
- Atualize a variável DISCORD_TOKEN no Railway

## 📞 Suporte

Para suporte, entre em contato com o desenvolvedor.

## ⚠️ Segurança

**NUNCA compartilhe seu token Discord!**

O token está protegido usando variáveis de ambiente. Certifique-se de:
- Não commitar o token no GitHub
- Não compartilhar screenshots com o token visível
- Regenerar o token se ele for exposto

## 📄 Licença

Este bot é fornecido como está, sem garantias.

---

**Desenvolvido para VIREX STORE** 🚀
