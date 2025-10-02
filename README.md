# SISTEMAS-DE-GERENCIAMENTO-DE-USOARIOS
Uma aplicação console desenvolvida para a gestão de dados de usuários. As funcionalidades incluem registro, visualização e exclusão de informações, demonstrando proficiência em manipulação de arquivos, controle de fluxo e lógica de programação.
# 🤖 n8n Chatbot para WhatsApp

[![n8n](https://img.shields.io/badge/n8n-Workflow-blue?logo=n8n&logoColor=white)](https://n8n.io)  
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)  
[![GitHub](https://img.shields.io/badge/GitHub-Repo-black?logo=github)](https://github.com/SEU_USUARIO/SEU_REPO)

---

## 📌 Resumo
Este projeto contém um **workflow n8n** que implementa um **chatbot inteligente no WhatsApp**.  
Ele utiliza a **IA do Google Gemini Chat** para gerar respostas naturais e educadas, mantendo o **histórico da conversa** através do Redis.

---

## 🔄 Como funciona
1. **Webhook** → recebe mensagens enviadas pelo usuário no WhatsApp.  
2. **Set** → organiza informações como sessão e ID do chat.  
3. **Switch** → garante que apenas mensagens reais sejam processadas.  
4. **AI Agent (Google Gemini Chat)** → gera respostas inteligentes seguindo instruções pré-definidas (com emojis para soar mais humano).  
5. **Redis Chat Memory** → mantém o contexto da conversa armazenado.  
6. **Send Seen** → marca a mensagem como lida.  
7. **Send a text message** → envia a resposta final ao usuário no WhatsApp.  

---

## ✨ Destaques
- Integração direta com **WhatsApp**.  
- Uso de **Google Gemini Chat** como motor de IA.  
- **Memória persistente** com Redis.  
- Estrutura modular, simples de adaptar para outros canais.  

---

## 🚀 Como usar

### 1) Importar no n8n
- Abra seu painel do n8n.  
- Vá em **Workflows → Import from file**.  
- Selecione o arquivo [`My workflow.json`](./My%20workflow.json).  

### 2) Configurar credenciais necessárias
- **WhatsApp API** → configure sua instância (ex: [WhatsApp Business API](https://developers.facebook.com/docs/whatsapp/)).  
- **Redis** → defina conexão com seu banco de memória.  
- **Google Gemini API** → configure chave de acesso ao modelo de IA.  

### 3) Executar
- Ative o workflow.  
- Envie uma mensagem no WhatsApp.  
- O bot irá responder automaticamente com base na IA e manter o contexto da conversa.  

---

## 📂 Estrutura do Repositório
