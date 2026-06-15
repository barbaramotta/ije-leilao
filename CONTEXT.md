# 🎯 CONTEXTO DO PROJETO - LEILÃO IJE

## RESUMO EXECUTIVO

Desenvolvimento de **plataforma de leilão beneficente** para o Instituto Jardim Europa com lances em tempo real via Supabase, sem aparecer nome pessoal na URL.

---

## 🎯 OBJETIVO PRINCIPAL

✅ Website profissional com lances compartilhados em **TEMPO REAL**  
✅ Dados salvos no **Supabase** (sincronismo global)  
✅ Backup em **Google Sheets**  
✅ Deployed no **GitHub Pages** + **Vercel**  
✅ Sem "barbaramotta" no URL  

---

## 📊 ESPECIFICAÇÕES TÉCNICAS

### Item do Leilão
- **Camisa**: Autografada pela Seleção Brasileira (doada por Casemiro)
- **Lance Inicial**: R$ 1.000,00
- **Incremento**: R$ 100,00 (automático)
- **Data Final**: 30/06/2026 às 19h
- **Local Retirada**: Shopping Iguatemi Porto Alegre
- **Envio**: Brasil inteiro (frete por conta do arrematante)
- **Pagamento**: PIX

### Visual
- **Font**: Raleway
- **Cores**: Preto (#1A1A1A), Branco (#FFFFFF), Vermelho (#E63946)
- **Logo**: 160px (Instituto Jardim Europa)
- **Design**: Minimalista, profissional

### Funcionalidades
1. **Cadastro obrigatório** (Nome, CPF, Email, Telefone)
2. **Sistema de lances** com validação automática
3. **Painel ao vivo** mostrando todos os lances
4. **Countdown timer** até data final
5. **Zoom de fotos** (2 imagens da camisa)
6. **Terms & Conditions** integrado

---

## 🔐 CREDENCIAIS (JÁ CONFIGURADAS)

### Supabase
```
URL: https://qonoguirtqqjekyjkrif.supabase.co
Anon Key: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
Tabela: bids
Colunas: id, user_name, user_cpf, user_email, user_phone, amount, created_at
```

### GitHub
```
Repo: barbaramotta/ije-leilao
Token: [REMOVIDO — nunca commitar tokens. Guarde em local seguro / variável de ambiente]
Branch: main
```

### Google Sheets
```
Apps Script URL: https://script.google.com/.../exec
Planilha: [ID na descrição]
Colunas: A=Nome, B=CPF, C=Email, D=Telefone, E=Valor
```

---

## 📁 ESTRUTURA DO PROJETO

```
ije-leilao-completo/
├── index.html          ← ARQUIVO PRINCIPAL (site completo)
├── vercel.json         ← Config Vercel (deploy automático)
├── .env.local          ← Credenciais Supabase & Google
├── .gitignore          ← Não commitar credenciais
├── README.md           ← Documentação
└── CONTEXT.md          ← Este arquivo
```

---

## 🐛 PROBLEMAS CONHECIDOS

### ❌ Vercel Deploy com Erro
- **Status**: Deployments falhando (Error 7s, 6s, 8s)
- **Causa Possível**: CORS ou configuração Supabase
- **Solução**: Verificar logs no Vercel Deployments
- **Ação Necessária**: Debugar e corrigir

### ✅ Supabase Conectado
- Tabela "bids" criada com sucesso
- Permissões RLS configuradas
- Pronto para receber dados

### ✅ GitHub Sincronizado
- Repositório atualizado
- Token funcionando
- Deploy automático ativado

---

## 🚀 FLUXO DE DESENVOLVIMENTO

1. **Editar código** no Claude Code
2. **Testar localmente** abrindo index.html
3. **Fazer commit** com mensagem descritiva
4. **Push no GitHub** (automático com token)
5. **Vercel faz deploy** (após correção de erro)
6. **Validar em produção**

---

## 📋 TAREFAS PENDENTES

### URGENTE 🔴
- [ ] Corrigir erro de deploy no Vercel
- [ ] Validar conexão Supabase (dados não chegando)
- [ ] Testar inserção de dados no site

### IMPORTANTE 🟠
- [ ] Confirmar Google Sheets recebendo dados
- [ ] Fazer teste completo com cadastro + lance
- [ ] Validar painel de lances em tempo real

### MELHORIAS 🟡
- [ ] Adicionar animações CSS
- [ ] Melhorar responsividade mobile
- [ ] Adicionar notificação sonora de novo lance

---

## ✅ CHECKLIST DE VALIDAÇÃO

Antes de considerar PRONTO:

- [ ] Site abre sem console errors (F12)
- [ ] Cadastro funciona e salva no Supabase
- [ ] Lances são dados e aparecem no painel
- [ ] Incremento de R$100 é obrigatório
- [ ] Countdown timer atualiza cada segundo
- [ ] Fotos da camisa fazem zoom
- [ ] Dados também em Google Sheets
- [ ] Layout mobile responsivo
- [ ] Nenhum erro de CORS
- [ ] Deploy automático Vercel funcionando

---

## 🔗 LINKS IMPORTANTES

| Recurso | URL |
|---------|-----|
| **Site (GitHub)** | https://barbaramotta.github.io/ije-leilao/ |
| **Supabase Console** | https://supabase.com/projects/ije-leilao |
| **GitHub Repo** | https://github.com/barbaramotta/ije-leilao |
| **Vercel Dashboard** | https://vercel.com/barbaramotta/ije-leilao |
| **Google Sheets** | [Link para planilha] |
| **Instituto** | www.institutojardimeuropa.com.br |

---

## 💡 NOTAS IMPORTANTES

1. **Credenciais públicas**: As chaves do Supabase/Google neste contexto são seguras (keys públicas apenas, sem permissão de modificar dados sensíveis)

2. **Token GitHub**: Válido por 30 dias. Se expirar, gerar novo.

3. **Deploy**: Vercel está configurado para fazer deploy automático ao fazer push no GitHub

4. **Sincronismo**: Supabase usa Realtime Subscriptions (dados aparecem instantaneamente para todos)

5. **Google Sheets**: Dados são copiados para backup (não é a source of truth)

---

## 🎓 PARA NOVOS DESENVOLVEDORES

Se você é novo no projeto:

1. Leia este arquivo completamente
2. Abra `README.md` para instruções técnicas
3. Revise `index.html` para entender a estrutura
4. Verifique `.env.local` para credenciais
5. Teste o site abrindo `index.html` no navegador
6. Use F12 (console) para debugar problemas

---

## 📞 CONTATO & SUPORTE

**Responsável**: Barbara Motta  
**Repositório**: barbaramotta/ije-leilao  
**Status**: Em desenvolvimento ⚙️  
**Última atualização**: 15/06/2026

---

**Desenvolvido com ❤️ para o Instituto Jardim Europa**
