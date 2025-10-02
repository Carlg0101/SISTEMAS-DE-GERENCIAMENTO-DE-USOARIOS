# 🤖 Chatbot no WhatsApp com n8n + Google Gemini

Este repositório contém um **workflow do n8n** para criar um **assistente de chatbot no WhatsApp**, utilizando IA para gerar respostas inteligentes e mantendo o contexto das conversas.

---

## 🔄 Fluxo do Workflow

1. **Webhook** → recebe mensagens do WhatsApp.  
2. **Set** → organiza dados como sessão e ID do chat.  
3. **Switch** → verifica se o evento é realmente uma mensagem.  
4. **AI Agent (Google Gemini Chat)** → gera respostas inteligentes e educadas, com instruções personalizadas (incluindo uso de emojis).  
5. **Redis Chat Memory** → armazena o histórico de conversas.  
6. **Send Seen** → marca a mensagem como lida.  
7. **Send a text message** → envia a resposta de volta ao usuário no WhatsApp.  

---

## ✨ Recursos

- Integração com **WhatsApp**.  
- Motor de IA: **Google Gemini Chat**.  
- **Memória persistente**: Redis.  
- Workflow modular, fácil de adaptar para outros canais.

---

## 🚀 Como usar

1. Clone o repositório:
   ```bash
   git clone https://github.com/Carlg0101/SISTEMAS-DE-GERENCIAMENTO-DE-USOARIOS.git
   cd SISTEMAS-DE-GERENCIAMENTO-DE-USOARIOS
