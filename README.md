# MCP Artsoft Gateway (Rebortec)

[🇵🇹 Português](#-português) | [🇬🇧 English](#-english)

---

## 🇵🇹 Português

O **MCP Artsoft Gateway** é uma solução de conectividade de nível empresarial desenvolvida pela [Rebortec](https://rebortec.com) que permite ligar assistentes de Inteligência Artificial e modelos de linguagem diretamente ao ecossistema **ARTSOFT ERP** através do standard aberto **Model Context Protocol (MCP)**.

### ✨ Destaques de Engenharia e Capacidades
- **Arquitetura de Elevada Resiliência:** Mecanismos de tolerância a falhas e proteção ativa de ligações para continuidade operacional.
- **Otimização Inteligente de Comunicação:** Processamento de tráfego com elevada densidade informativa e consumo reduzido de contexto nos modelos de IA.
- **Consolidação Temporal Avançada:** Reconciliação unificada e coerência documental contínua ao longo de múltiplos períodos fiscais.
- **Recuperação Guiada e Validação Segura:** Descoberta assistida de alternativas e fluxos protegidos de validação prévia em operações críticas.
- **Interatividade Proativa:** Capacidade de sugestão inteligente de próximos passos operacionais e criação de atalhos e agendamentos práticos.
- **Segurança e Operação Offline:** Validação criptográfica com governação por perfis, salvaguarda de credenciais e operação local protegida.
- **Consola de Gestão Dedicada:** Interface administrativa em `http://127.0.0.1:8766` com gerador automático de configurações prontas a utilizar.

---

### 🚀 Instalação Rápida (Windows Server / Windows 10/11)

1. Aceda à secção de [Releases](https://github.com/ruibarbosareb/artsoft-mcp-gateway/releases/latest) e descarregue o pacote `ArtsoftMcpGateway_vX.X.X_Windows_x64.zip`.
2. Extraia o conteúdo para uma pasta temporária (ex: `C:\Temp\ArtsoftMcp`).
3. Abra a pasta, clique com o botão direito sobre o ficheiro **`instalar.bat`** e selecione **"Executar como Administrador"**.
4. O instalador configura o serviço Windows (`ArtsoftMcpService`) e inicializa a pasta de dados em `C:\ProgramData\ArtsoftMcp`.
5. Abra o navegador em `http://127.0.0.1:8766` (login inicial: utilizador `admin` / senha `admin`).
6. No separador **Empresas ARTSOFT**, configure a ligação ao XMLServices (`Host`, `Porta 2604`, utilizador e senha).

---

### 🤖 Como Ligar aos Clientes de IA (Claude Desktop, Cursor, Antigravity)

**Não precisa de escrever JSON manualmente!** O Backoffice gera a configuração exata pronta a copiar:

1. Aceda ao Backoffice em `http://127.0.0.1:8766`.
2. Vá ao separador **Tokens de Acesso MCP** e clique em **"+ Emitir Novo Token"**.
3. Selecione o utilizador, as empresas autorizadas e as permissões pretendidas.
4. Ao clicar em **"Gerar Token"**, o Backoffice apresenta de imediato:
   - O **JSON de configuração completo** pronto a colar no seu cliente (ex.: `claude_desktop_config.json`).
   - O **URL Direto MCP** para clientes remotos.
5. Basta clicar no botão **"Copiar Configuração Claude"** e colar no seu assistente de IA.

---

### 🛡️ Licenciamento & Suporte
- **Modo Freemium:** Até 50 pedidos ao ERP por dia gratuitamente.
- **Modo Comercial (PRO):** Pedidos diários ilimitados, multi-empresa e suporte prioritário. Contacte a Rebortec em [comercial@rebortec.com](mailto:comercial@rebortec.com).

---

## 🇬🇧 English

**MCP Artsoft Gateway** is an enterprise-grade connectivity solution developed by [Rebortec](https://rebortec.com) that connects AI assistants and LLMs directly to the **ARTSOFT ERP** ecosystem using the open **Model Context Protocol (MCP)** standard.

### ✨ Engineering Highlights & Key Capabilities
- **High-Resilience Architecture:** Fault-tolerant mechanisms and proactive connection safeguards for continuous operation.
- **Intelligent Communication Optimization:** High-density payload processing with significantly reduced token overhead for AI models.
- **Advanced Temporal Consolidation:** Unified reconciliation and document flow coherence across multiple fiscal periods.
- **Guided Recovery & Safe Validation:** Assisted discovery of valid operational alternatives and protected pre-commit flows for critical actions.
- **Proactive Interactivity:** Smart next-step operational guidance with support for shortcuts and automated routines.
- **Security & Offline Operation:** Cryptographic verification, granular scope-based governance, and protected local operation.
- **Dedicated Management Console:** Clean management interface at `http://127.0.0.1:8766` with built-in client configuration generator.

---

### 🚀 Quick Installation (Windows Server / Windows 10/11)

1. Go to the [Releases](https://github.com/ruibarbosareb/artsoft-mcp-gateway/releases/latest) section and download `ArtsoftMcpGateway_vX.X.X_Windows_x64.zip`.
2. Extract the archive into a temporary folder (e.g., `C:\Temp\ArtsoftMcp`).
3. Right-click on **`instalar.bat`** and choose **"Run as Administrator"**.
4. The installer automatically registers and starts the Windows Service (`ArtsoftMcpService`) and sets up data storage in `C:\ProgramData\ArtsoftMcp`.
5. Open your browser and navigate to `http://127.0.0.1:8766` (default login: `admin` / `admin`).
6. In the **Empresas ARTSOFT** tab, set up your XMLServices connection details (`Host`, `Port 2604`, credentials).

---

### 🤖 Connecting to AI Clients (Claude Desktop, Cursor, Antigravity)

**No need to write JSON manually!** The Backoffice generates the ready-to-use configuration for you:

1. Open the Backoffice at `http://127.0.0.1:8766`.
2. Go to the **Tokens de Acesso MCP** tab and click **"+ Emitir Novo Token"**.
3. Choose the user, authorized companies, and scopes.
4. Click **"Gerar Token"** — the Backoffice immediately displays:
   - The **complete configuration JSON** ready to paste into your AI client (e.g., `claude_desktop_config.json`).
   - The **Direct MCP URL** for remote clients.
5. Simply click **"Copiar Configuração Claude"** (or Copy Direct URL) and paste it into your AI assistant.

---

### 🛡️ Licensing & Support
- **Freemium Tier:** Up to 50 ERP queries per day at no cost.
- **Commercial Tier (PRO):** Unlimited daily requests, multi-company support, and priority SLA. Contact Rebortec at [comercial@rebortec.com](mailto:comercial@rebortec.com).
