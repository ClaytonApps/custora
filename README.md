# Custora — Recibo Digital de Custódia

Aplicação web 100% offline para mototaxistas, motoboys e entregadores registrarem **coleta** e **entrega** de objetos com validade jurídica: assinatura digital, foto, GPS e notificação automática via WhatsApp.

> Tudo roda no navegador. Sem servidor, sem cadastro, sem mensalidade.

---

## ✨ Funcionalidades

- 📦 **Protocolo de Coleta** — dados do remetente, descrição e estado do item, **foto do objeto**, assinatura digital
- ✅ **Protocolo de Entrega** — vinculação por número de protocolo, dados do recebedor, **foto da entrega**, assinatura, captura de GPS
- 💬 **Notificação WhatsApp automática** — abre conversa com o remetente já preenchida (item, recebedor, data, link do mapa)
- 📊 **Dashboard** com KPIs (total, entregues, pendentes, criados hoje) e atividade recente
- 🗂️ **Histórico** pesquisável e filtrável
- 📈 **Relatório mensal** com exportação em PDF
- 🧾 **PDF individual** por protocolo (com fotos e assinaturas)
- 💾 **Backup CSV** e armazenamento local (localStorage)
- 📱 **PWA-ready** — funciona em mobile e desktop, instalável como app
- ⚙️ **Configurável** — nome da empresa, slogan, telefone e mensagem WhatsApp personalizados

---

## 🚀 Como usar

1. Baixe o arquivo `index.html`
2. Abra-o no navegador (Chrome, Edge, Safari, Firefox)
3. Pronto — não precisa instalar nada

Para usar como app no celular: abra no Chrome/Safari → menu → **"Adicionar à tela inicial"**.

---

## 📋 Fluxo de uso

### Coleta
1. Toque em **"Nova Coleta"**
2. Preencha os dados do remetente
3. Descreva o item e seu estado
4. **Tire uma foto** do objeto (recomendado)
5. Capture a assinatura do remetente
6. Registre — um protocolo `CST-AAAAMMDD-XXXX` é gerado

### Entrega
1. Vá em **"Protocolo de Entrega"**
2. Informe o número do protocolo (ou clique em "Entregar" no Dashboard)
3. Preencha dados do recebedor
4. **Tire a foto da entrega** (recomendado)
5. Capture a assinatura do destinatário
6. Confirme — o WhatsApp do remetente abre automaticamente com a confirmação + GPS

---

## 🛠️ Stack

- HTML5 + CSS3 + JavaScript vanilla (sem frameworks)
- [jsPDF](https://github.com/parallax/jsPDF) para geração de PDFs
- Canvas API para assinaturas digitais
- File API + Camera (`capture="environment"`) para fotos
- Geolocation API para coordenadas GPS
- localStorage para persistência

**Tudo em um único arquivo `index.html`.**

---

## 🔒 Privacidade

- Nenhum dado sai do dispositivo
- Não há rastreamento, telemetria ou analytics
- Não há dependência de servidor próprio
- A única requisição externa é o carregamento do jsPDF via CDN (uma única vez, depois fica em cache)

---

## ⚠️ Limitações

- Os dados ficam apenas no navegador onde foram criados (use o backup CSV regularmente)
- O `localStorage` tem limite de ~5–10 MB (fotos são comprimidas para ~1280px JPEG 72%)
- Se limpar os dados do navegador, os registros são perdidos

---

## 🗺️ Roadmap

- [ ] Importação de backup CSV
- [ ] Sincronização opcional via Google Drive/Dropbox
- [ ] Modo escuro
- [ ] PWA com Service Worker (offline 100%)
- [ ] Múltiplas fotos por protocolo

---

## 🤝 Contribuindo

Issues e PRs são bem-vindos! Como tudo está em um único arquivo, basta editar `index.html` e abrir no navegador para testar.

---

## 📄 Licença

MIT — use, modifique e distribua livremente.

---

## ☕ Apoie o projeto

Se o Custora te ajuda no dia a dia e você quer manter o projeto **gratuito e em código aberto**, considere fazer uma contribuição. Qualquer valor faz a diferença!

### 👉 [**Apoiar via Mercado Pago**](https://mpago.la/2z5Uj6E)

Sua contribuição ajuda a manter o desenvolvimento, novas funcionalidades e a infraestrutura do projeto.

**Obrigado pelo apoio! 🧡**
