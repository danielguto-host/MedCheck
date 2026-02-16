# 🏥 MedCheck - Verificador de Corantes em Medicamentos

App completo com IA para verificar se medicamentos contêm óxidos de ferro (CI 77491 e CI 77492).

## 📋 O que você vai precisar

1. ✅ Conta GitHub (você já tem!)
2. ✅ Conta Vercel (gratuita) - vamos criar
3. ✅ Chave API do Claude (gratuita para começar)

---

## 🚀 PASSO A PASSO COMPLETO

### PARTE 1: Obter Chave API do Claude (5 minutos)

1. **Acesse:** https://console.anthropic.com/
2. **Faça login** ou crie uma conta
3. **Vá em "API Keys"** no menu lateral
4. **Clique em "Create Key"**
5. **Copie a chave** (começa com `sk-ant-api...`)
   - ⚠️ **GUARDE BEM!** Você só verá ela uma vez
   - Cole num bloco de notas temporariamente

> 💡 **Dica:** Anthropic dá créditos gratuitos para começar!

---

### PARTE 2: Subir Código pro GitHub (3 minutos)

#### Opção A: Pelo Site GitHub (Mais Fácil)

1. **Entre no GitHub:** https://github.com
2. **Clique em "New repository"** (botão verde)
3. **Configure:**
   - Repository name: `medcheck`
   - Description: `Verificador de corantes em medicamentos`
   - ✅ Public
   - ✅ Add README file
4. **Clique em "Create repository"**
5. **Adicione os arquivos:**
   - Clique em "Add file" → "Upload files"
   - Arraste TODOS os arquivos desta pasta:
     - `index.html`
     - `package.json`
     - `vercel.json`
     - Pasta `api/` com o arquivo `check-medication.js`
   - Clique em "Commit changes"

#### Opção B: Por Linha de Comando (Se você usa terminal)

```bash
# No terminal, dentro da pasta medcheck-project:
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/medcheck.git
git push -u origin main
```

---

### PARTE 3: Publicar no Vercel (5 minutos)

1. **Acesse:** https://vercel.com/signup
2. **Faça login com GitHub** (botão "Continue with GitHub")
3. **Autorize o Vercel** a acessar seus repositórios
4. **Clique em "Add New Project"**
5. **Importe seu repositório:**
   - Procure `medcheck` na lista
   - Clique em "Import"
6. **Configure as variáveis de ambiente:**
   - Clique em "Environment Variables"
   - Adicione:
     - **Name:** `ANTHROPIC_API_KEY`
     - **Value:** Cole aqui a chave API que você copiou
     - Selecione: Production, Preview, Development
   - Clique em "Add"
7. **Deploy:**
   - Clique em "Deploy"
   - Aguarde 1-2 minutos ⏳
8. **PRONTO! 🎉**
   - Seu app estará em: `https://medcheck.vercel.app` (ou similar)
   - Copie o link!

---

## 📱 USAR NO IPHONE

### Adicionar à Tela Inicial

1. **Abra o link** do Vercel no Safari do iPhone
2. **Toque no botão Compartilhar** (quadrado com seta ⬆️)
3. **Role para baixo** → toque em "Adicionar à Tela de Início"
4. **Dê um nome:** "MedCheck"
5. **Toque em Adicionar**
6. **Pronto!** Agora funciona como app nativo! 📱

---

## 🔧 Estrutura do Projeto

```
medcheck-project/
├── index.html              # Frontend (interface do app)
├── api/
│   └── check-medication.js # Backend (API que chama Claude)
├── package.json            # Dependências do projeto
├── vercel.json            # Configuração do Vercel
└── README.md              # Este arquivo
```

---

## 💡 Como Funciona

1. **Usuário** digita nome do medicamento ou tira foto
2. **Frontend** (index.html) envia para o backend
3. **Backend** (api/check-medication.js) chama API do Claude
4. **Claude** busca informações e analisa composição
5. **Resultado** volta pro usuário com alerta se contém corantes

---

## 🆘 Problemas Comuns

### ❌ "API Key inválida"
- Verifique se copiou a chave completa
- Recrie a chave no console do Anthropic
- Adicione novamente no Vercel (Settings → Environment Variables)

### ❌ "Erro ao conectar"
- Verifique se o deploy terminou (aguarde 2 minutos)
- Tente abrir em navegador anônimo
- Limpe cache do navegador

### ❌ "Função não encontrada"
- Certifique-se que a pasta `api/` foi enviada pro GitHub
- Verifique se o arquivo está em `api/check-medication.js`
- Faça novo deploy no Vercel

---

## 🔄 Atualizar o App

Quando quiser fazer mudanças:

1. **Edite os arquivos** no seu computador
2. **Suba pro GitHub:**
   - Via site: "Add file" → "Upload files"
   - Via terminal: `git add . && git commit -m "Update" && git push`
3. **Vercel atualiza automaticamente!** 🚀

---

## 💰 Custos

- **GitHub:** Gratuito ✅
- **Vercel:** Gratuito ✅
- **Claude API:** 
  - Créditos gratuitos para começar
  - Depois: ~$0.003 por consulta
  - 1000 consultas = ~$3

---

## 📞 Precisa de Ajuda?

Se algo der errado, me mande:
1. Print do erro
2. Link do seu repositório GitHub
3. Link do app no Vercel

Vou te ajudar a resolver! 😊

---

## 🎉 Está Funcionando?

Parabéns! Agora você tem:
- ✅ App rodando 24/7 na web
- ✅ Funciona no iPhone como app nativo
- ✅ Análise automática com IA
- ✅ Busca na web integrada
- ✅ Análise de fotos de bulas
- ✅ Histórico de consultas

**Bom uso e cuide-se! 🏥💊**




