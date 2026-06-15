# 🎯 LEILÃO IJE - Projeto Completo

## 📋 STATUS DO PROJETO

✅ **HTML**: Completo com Supabase integrado
✅ **Supabase**: Conectado (tabela "bids" criada)
✅ **Google Sheets**: Integrado para backup
❌ **Vercel**: Deployments com erro (em correção)
✅ **GitHub**: Repositório sincronizado

---

## 🔑 CREDENCIAIS CONFIGURADAS

### Supabase
- **URL**: `https://qonoguirtqqjekyjkrif.supabase.co`
- **Projeto**: ije-leilao
- **Tabela**: bids (com colunas: id, user_name, user_cpf, user_email, user_phone, amount, created_at)

### GitHub
- **Repo**: barbaramotta/ije-leilao
- **Token**: Configurado (ghp_...)
- **Branch**: main

### Google Sheets
- **Apps Script**: Configurado para receber dados
- **Planilha**: Coluna A=Nome, B=CPF, C=Email, D=Telefone, E=Valor

---

## 🚀 PRÓXIMOS PASSOS

### 1️⃣ Corrigir Erro do Vercel
- [ ] Verificar logs de erro no Vercel
- [ ] Possível problema: Falta de configuração CORS ou Supabase
- [ ] Solução: Ajustar `vercel.json` se necessário

### 2️⃣ Testar Conexão Supabase
- [ ] Abrir o site
- [ ] Fazer um cadastro
- [ ] Dar um lance
- [ ] Verificar se aparece na tabela "bids" do Supabase

### 3️⃣ Validar Google Sheets
- [ ] Confirmar que dados chegam na planilha
- [ ] Se não, reconfigurar Apps Script

### 4️⃣ Deploy Final
- [ ] Após correções, fazer novo push no GitHub
- [ ] Vercel fará deploy automático
- [ ] Validar em: `https://barbaramotta.github.io/ije-leilao/`

---

## 📝 ARQUIVOS DO PROJETO

```
ije-leilao-completo/
├── index.html              ← Arquivo principal (site completo)
├── vercel.json             ← Configuração Vercel
├── .env.local              ← Credenciais Supabase & Google
├── .gitignore              ← Ignorar arquivos sensíveis
└── README.md               ← Este arquivo
```

---

## 🔧 COMO USAR NO CLAUDE CODE

1. **Abra o Claude Code**
2. **Abra a pasta**: `/home/claude/ije-leilao-completo`
3. **Edite `index.html`** se precisar fazer alterações
4. **Teste localmente** abrindo o arquivo no navegador
5. **Faça commit e push** para GitHub
6. **Vercel** fará deploy automático

---

## 📊 CHECKLIST DE VALIDAÇÃO

- [ ] Site abre sem erros
- [ ] Botão "Cadastrar" funciona
- [ ] Formulário de cadastro aparece
- [ ] Dados salvam no Supabase
- [ ] Painel de lances mostra dados em tempo real
- [ ] Increment de R$100 funciona corretamente
- [ ] Dados também vão para Google Sheets
- [ ] Countdown timer funciona

---

## 🆘 TROUBLESHOOTING

### Problema: Vercel com erro
**Solução**: Verificar logs no painel Vercel → Deployments

### Problema: Dados não aparecem no Supabase
**Solução**: 
1. Abrir F12 no navegador
2. Console (aba preta)
3. Tentar dar um lance
4. Ver mensagem de erro

### Problema: Google Sheets não recebe dados
**Solução**: Reconfigurar Google Apps Script com novo URL

---

## 📞 CONTATO

**Projeto**: Instituto Jardim Europa - Leilão Beneficente  
**Item**: Camisa Autografada Seleção Brasileira (Casemiro)  
**Data Final**: 30/06/2026 às 19h  
**Website**: www.institutojardimeuropa.com.br

---

## ✨ DESENVOLVIDO COM

- HTML5 + CSS3 + JavaScript vanilla
- Supabase (tempo real)
- Google Sheets API
- GitHub Pages + Vercel
- Raleway Font

**Status**: Em desenvolvimento ⚙️
