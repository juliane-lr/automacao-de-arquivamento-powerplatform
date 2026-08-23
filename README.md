# 📂 Automação de Arquivamento Inteligente de Comprovantes com Power Automate

Solução de automação de processos de negócio (*RPA / Cloud Flows*) desenvolvida no ecossistema Microsoft Power Platform para eliminar o trabalho manual de triagem, arquivamento e confirmação de documentos fiscais/comprovantes recebidos por e-mail.

---

## 🎯 O Problema
Em rotinas administrativas e contábeis, o recebimento descentralizado de documentos por e-mail gera:
- Alto tempo gasto em tarefas operacionais repetitivas (abrir e-mails, baixar anexos, renomear e salvar em pastas).
- Risco de extravio de arquivos importantes.
- Falta de confirmação imediata de recebimento para o remetente/cliente.

---

## 💡 A Solução
Desenvolvimento de um **Cloud Flow automatizado no Power Automate** conectado ao **Office 365 Outlook** e **OneDrive for Business**:

1. **Gatilho de Evento:** Monitoramento em tempo real da caixa de entrada para mensagens com filtros específicos de assunto (`[Comprovante]`) e presença obrigatória de anexos.
2. **Iteração e Processamento:** Extração dinâmica do fluxo binário e metadados dos arquivos anexados.
3. **Persistência em Nuvem:** Salvamento e organização automática em diretório centralizado no OneDrive.
4. **Feedback Automático:** Disparo de resposta automática (*thread reply*) confirmando o protocolo e arquivamento com sucesso para o remetente.

---

## 🛠️ Tecnologias e Ferramentas
- **Microsoft Power Automate** (Cloud Flows, Conectores Office 365 e OneDrive)
- **Microsoft 365 / Outlook**
- **OneDrive for Business**

---

## 📊 Arquitetura do Fluxo
`[Novo E-mail com Anexo]` ➔ `[Filtro de Gatilho]` ➔ `[Loop 'Apply to Each']` ➔ `[Criar Arquivo no OneDrive]` ➔ `[Responder ao E-mail]`

---

## 📸 Demonstração
<img width="732" height="366" alt="image" src="https://github.com/user-attachments/assets/dc2da01d-2723-41a5-9e3b-8200fbfe4b6f" />
<img width="642" height="606" alt="image" src="https://github.com/user-attachments/assets/98cd83b8-8eb2-4b73-8c61-e03221508439" />

