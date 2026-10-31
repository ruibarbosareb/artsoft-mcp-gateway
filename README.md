# MCP Artsoft Gateway (Rebortec)

[🇵🇹 Português](#-português) | [🇬🇧 English](#-english)

---

## 🇵🇹 Português

O **MCP Artsoft Gateway** é um servidor bridge oficial desenvolvido pela [Rebortec](https://rebortec.com) que permite ligar modelos e assistentes de Inteligência Artificial (Claude Desktop, Cursor, Antigravity, ChatGPT, agentes autónomos) diretamente ao **ARTSOFT ERP** através do protocolo standard **MCP (Model Context Protocol)**.

### ✨ Principais Funcionalidades
- **Gestão Comercial & Faturação:** Consulta de clientes, propostas, encomendas, guias e faturas.
- **Stocks & Armazém:** Saldos físicos, artigos sem rotação, necessidades de aprovisionamento e artigos críticos.
- **Contabilidade & Tesouraria:** Extratos de contas correntes, pendentes de fornecedores/clientes e previsão de tesouraria.
- **Operação 100% Offline:** Validação criptográfica assíncrona (Ed25519) com Hardware Binding (App ID) — requer ligação à internet apenas na ativação inicial.
- **Multi-Empresa & Multi-Utilizador:** Gestão centralizada de bases de dados ARTSOFT com prompts de IA personalizados por empresa e por colaborador.
- **Consola Web Local:** Interface administrativa em `http://127.0.0.1:8766` para gestão simples de tokens, auditoria e empresas.

---

### 🚀 Instalação Rápida (Windows Server / Windows 10/11)

1. Aceda à secção de [Releases](https://github.com/ruibarbosareb/artsoft-mcp-gateway/releases/latest) e descarregue o pacote `ArtsoftMcpGateway_vX.X.X_Windows_x64.zip`.
2. Extraia o conteúdo para uma pasta temporária (ex: `C:\Temp\ArtsoftMcp`).
3. Abra a pasta, clique com o botão direito sobre o ficheiro **`instalar.bat`** e selecione **"Executar como Administrador"**.
4. O instalador configura automaticamente o serviço de sistema Windows (`ArtsoftMcpService`) e inicializa a pasta de dados em `C:\ProgramData\ArtsoftMcp`.
5. Abra o seu navegador em `http://127.0.0.1:8766` (login inicial: utilizador `admin` / senha `admin`).
6. Configure as coordenadas do seu ARTSOFT XMLServices (`IP`, `Porta 2604`, `ADMIN`).

---

### 🤖 Como Ligar aos Clientes de IA

No ficheiro de configuração MCP do seu cliente de IA (ex: Claude Desktop ou Cursor), adicione:

```json
{
  "mcpServers": {
    "artsoft": {
      "command": "C:\\Program Files\\Rebortec\\ArtsoftMcp\\bin\\ArtsoftMcpService.exe",
      "args": ["mcp"],
      "env": {
        "ARTSOFT_TOKEN": "O_SEU_TOKEN_MCP_GERADO_NO_BACKOFFICE"
      }
    }
  }
}
```

---

### 🛡️ Licenciamento & Suporte
- **Modo Freemium:** Até 50 pedidos ao ERP por dia gratuitamente.
- **Modo Comercial (PRO):** Pedidos ilimitados e suporte multi-empresa. Contacte a Rebortec em [comercial@rebortec.com](mailto:comercial@rebortec.com).

---

## 🇬🇧 English

**MCP Artsoft Gateway** is an enterprise-grade bridge server developed by [Rebortec](https://rebortec.com) that connects AI agents and LLMs (Claude Desktop, Cursor, Antigravity, autonomous agents) directly to **ARTSOFT ERP** using the open **Model Context Protocol (MCP)** standard.

### ✨ Key Features
- **Sales & Invoicing:** Query customers, sales proposals, orders, delivery notes, and invoices.
- **Stock & Warehouse:** Physical stock levels, dead stock analysis, replenishment needs, and critical items.
- **Accounting & Treasury:** Current account statements, overdue debts, open balance reconciliation, and cashflow forecast.
- **100% Offline Capability:** Ed25519 cryptographic lease verification with Hardware Binding (App ID) — requires internet connection only for the initial activation.
- **Multi-Company & Multi-User:** Centralized management of multiple ARTSOFT companies with tailored AI prompt engineering per company and user.
- **Local Web Backoffice:** Clean management UI running on `http://127.0.0.1:8766` for tokens, audit trails, and connectivity.

---

### 🚀 Quick Installation (Windows Server / Windows 10/11)

1. Go to the [Releases](https://github.com/ruibarbosareb/artsoft-mcp-gateway/releases/latest) section and download `ArtsoftMcpGateway_vX.X.X_Windows_x64.zip`.
2. Extract the archive into a temporary folder (e.g., `C:\Temp\ArtsoftMcp`).
3. Right-click on **`instalar.bat`** and choose **"Run as Administrator"**.
4. The installer automatically registers and starts the Windows Service (`ArtsoftMcpService`) and sets up data storage in `C:\ProgramData\ArtsoftMcp`.
5. Open your browser and navigate to `http://127.0.0.1:8766` (default login: `admin` / `admin`).
6. Enter your ARTSOFT XMLServices connection details (`Host`, `Port 2604`, `ADMIN`).

---

### 🤖 Connecting to AI Clients (Claude Desktop / Cursor)

Add the following configuration to your AI client's MCP configuration file:

```json
{
  "mcpServers": {
    "artsoft": {
      "command": "C:\\Program Files\\Rebortec\\ArtsoftMcp\\bin\\ArtsoftMcpService.exe",
      "args": ["mcp"],
      "env": {
        "ARTSOFT_TOKEN": "YOUR_TOKEN_GENERATED_IN_BACKOFFICE"
      }
    }
  }
}
```

---

### 🛡️ Licensing & Support
- **Freemium Tier:** Up to 50 ERP queries per day at no cost.
- **Commercial Tier (PRO):** Unlimited daily requests, multi-company support, and priority SLA. Contact Rebortec at [comercial@rebortec.com](mailto:comercial@rebortec.com).
