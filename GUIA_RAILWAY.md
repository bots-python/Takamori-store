# 🚂 GUIA RÁPIDO - Deploy Railway

## Passo a Passo Simples

### 1️⃣ Preparar o Token do Discord

1. Acesse: https://discord.com/developers/applications
2. Crie uma "New Application"
3. Nome: **VIREX STORE**
4. Vá em **Bot** > **Reset Token** > Copie o token
5. Habilite em **Bot**:
   - ✅ Presence Intent
   - ✅ Server Members Intent  
   - ✅ Message Content Intent
6. Em **OAuth2** > **URL Generator**:
   - Marque: `bot` e `applications.commands`
   - Bot Permissions: `Administrator`
7. Copie a URL e convide o bot

### 2️⃣ Deploy no Railway

#### Opção A - GitHub (Recomendado)
1. Crie um repositório no GitHub
2. Faça upload dos arquivos:
   - `bot_virex_store.py`
   - `requirements.txt`
   - `Procfile`
   - `README.md`
3. Acesse https://railway.app/
4. Login com GitHub
5. "New Project" > "Deploy from GitHub repo"
6. Selecione o repositório
7. Em **Variables**, adicione:
   ```
   DISCORD_TOKEN=seu_token_aqui
   ```
8. Aguarde o deploy (2-5 minutos)

#### Opção B - Upload Direto
1. Acesse https://railway.app/
2. "New Project" > "Empty Project"
3. Faça upload dos arquivos pelo painel
4. Configure a variável **DISCORD_TOKEN**
5. Deploy automático

### 3️⃣ Verificar se está funcionando

1. No Railway, clique em "View Logs"
2. Você deve ver:
   ```
   ╔══════════════════════════════════════╗
   ║   🤖 VIREX STORE BOT ONLINE!        ║
   ╚══════════════════════════════════════╝
   ```
3. No Discord, teste: `/ajudavirexstore`

### 4️⃣ Configurar o Bot

1. Use `/setup` no Discord
2. Configure:
   - 📁 Categoria (onde criar carrinhos)
   - 💳 PIX (informações de pagamento)
3. Crie produtos ou dropdowns
4. Envie painéis nos canais

### 5️⃣ Comandos Essenciais

```
/ajudavirexstore     - Ver todos comandos
/setup               - Painel de configuração
/setuplogs           - Configurar logs
/botvoz <canal>      - Bot em voz 24/7
```

## ⚡ Dicas

- O Railway oferece 500 horas grátis/mês
- Mantenha o bot sempre online
- Use `/botvoz` para bot aparecer online 24/7
- Configure logs para monitorar atividades

## 🆘 Problemas Comuns

**Bot offline:**
- Verifique se a variável DISCORD_TOKEN está correta
- Veja os logs no Railway

**Comandos não funcionam:**
- Aguarde 1-2 minutos após o bot ficar online
- Verifique as Intents no Discord Developer Portal

**Erro de permissão:**
- Convide o bot novamente com permissão de Administrator

## 📱 Suporte

Se precisar de ajuda, verifique:
1. Logs no Railway
2. Status do Discord
3. README.md completo

---

**🎉 Pronto! Seu bot está no ar!**
