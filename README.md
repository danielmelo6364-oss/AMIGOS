<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Gestão Comercial</title>

  <style>
    :root {
      --primary: #1d4ed8;
      --primary-dark: #1e3a8a;
      --background: #f3f6fb;
      --card: #ffffff;
      --text: #1f2937;
      --muted: #6b7280;
      --border: #e5e7eb;
      --success: #15803d;
      --success-bg: #dcfce7;
      --warning: #b45309;
      --warning-bg: #fef3c7;
      --danger: #b91c1c;
      --danger-bg: #fee2e2;
      --gray-bg: #f3f4f6;
      --shadow: 0 4px 15px rgba(15, 23, 42, 0.08);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, Helvetica, sans-serif;
    }

    body {
      background: var(--background);
      color: var(--text);
    }

    button,
    input,
    select,
    textarea {
      font: inherit;
    }

    button {
      cursor: pointer;
    }

    .layout {
      display: flex;
      min-height: 100vh;
    }

    .sidebar {
      width: 240px;
      background: var(--primary-dark);
      color: white;
      padding: 22px 14px;
      position: fixed;
      top: 0;
      bottom: 0;
      left: 0;
    }

    .brand {
      font-size: 21px;
      font-weight: bold;
      padding: 0 12px 24px;
      border-bottom: 1px solid rgba(255, 255, 255, 0.18);
      margin-bottom: 18px;
    }

    .menu {
      display: flex;
      flex-direction: column;
      gap: 7px;
    }

    .menu button {
      border: 0;
      color: white;
      background: transparent;
      text-align: left;
      padding: 12px;
      border-radius: 8px;
      transition: 0.2s;
    }

    .menu button:hover,
    .menu button.active {
      background: rgba(255, 255, 255, 0.16);
    }

    .content {
      width: calc(100% - 240px);
      margin-left: 240px;
      padding: 26px;
    }

    .topbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 24px;
      gap: 20px;
    }

    .topbar h1 {
      font-size: 28px;
    }

    .date {
      color: var(--muted);
      font-size: 14px;
    }

    .view {
      display: none;
    }

    .view.active {
      display: block;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 16px;
      margin-bottom: 22px;
    }

    .card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 19px;
      box-shadow: var(--shadow);
    }

    .indicator-title {
      color: var(--muted);
      font-size: 14px;
      margin-bottom: 9px;
    }

    .indicator-value {
      font-size: 28px;
      font-weight: bold;
    }

    .section-title {
      font-size: 21px;
      margin-bottom: 14px;
    }

    .grid-2 {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 18px;
    }

    .form-card,
    .table-card {
      background: var(--card);
      border-radius: 12px;
      padding: 20px;
      border: 1px solid var(--border);
      box-shadow: var(--shadow);
      margin-bottom: 20px;
    }

    form {
      display: grid;
      gap: 13px;
    }

    .form-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 13px;
    }

    .form-group {
      display: flex;
      flex-direction: column;
      gap: 6px;
    }

    .form-group.full {
      grid-column: 1 / -1;
    }

    label {
      font-size: 13px;
      font-weight: bold;
      color: #374151;
    }

    input,
    select,
    textarea {
      width: 100%;
      padding: 10px 11px;
      border: 1px solid #d1d5db;
      border-radius: 7px;
      outline: none;
      background: white;
    }

    input:focus,
    select:focus,
    textarea:focus {
      border-color: var(--primary);
      box-shadow: 0 0 0 3px rgba(29, 78, 216, 0.12);
    }

    textarea {
      min-height: 80px;
      resize: vertical;
    }

    .btn {
      border: 0;
      border-radius: 7px;
      padding: 10px 15px;
      font-weight: bold;
      transition: 0.2s;
    }

    .btn-primary {
      color: white;
      background: var(--primary);
    }

    .btn-primary:hover {
      background: #1e40af;
    }

    .btn-success {
      color: white;
      background: var(--success);
    }

    .btn-warning {
      color: white;
      background: var(--warning);
    }

    .btn-danger {
      color: white;
      background: var(--danger);
    }

    .btn-outline {
      color: var(--primary);
      border: 1px solid var(--primary);
      background: white;
    }

    .btn-small {
      padding: 7px 10px;
      font-size: 12px;
    }

    .actions {
      display: flex;
      flex-wrap: wrap;
      gap: 7px;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      min-width: 700px;
    }

    .table-wrapper {
      overflow-x: auto;
    }

    th,
    td {
      border-bottom: 1px solid var(--border);
      padding: 12px 9px;
      text-align: left;
      font-size: 14px;
      vertical-align: top;
    }

    th {
      font-size: 12px;
      color: var(--muted);
      text-transform: uppercase;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      padding: 5px 8px;
      border-radius: 999px;
      font-size: 12px;
      font-weight: bold;
    }

    .badge-green {
      background: var(--success-bg);
      color: var(--success);
    }

    .badge-yellow {
      background: var(--warning-bg);
      color: var(--warning);
    }

    .badge-red {
      background: var(--danger-bg);
      color: var(--danger);
    }

    .badge-gray {
      background: var(--gray-bg);
      color: #4b5563;
    }

    .alert-list {
      display: grid;
      gap: 10px;
    }

    .alert-item {
      border-left: 5px solid var(--warning);
      background: var(--warning-bg);
      padding: 13px;
      border-radius: 6px;
    }

    .alert-item strong {
      display: block;
      margin-bottom: 4px;
    }

    .timeline {
      position: relative;
      display: grid;
      gap: 14px;
      padding-left: 20px;
    }

    .timeline::before {
      content: "";
      position: absolute;
      left: 5px;
      top: 0;
      bottom: 0;
      width: 2px;
      background: #bfdbfe;
    }

    .timeline-item {
      position: relative;
      background: #f8fafc;
      border: 1px solid var(--border);
      border-radius: 8px;
      padding: 12px;
    }

    .timeline-item::before {
      content: "";
      position: absolute;
      width: 10px;
      height: 10px;
      background: var(--primary);
      border-radius: 50%;
      left: -20px;
      top: 17px;
      border: 3px solid white;
      box-shadow: 0 0 0 1px var(--primary);
    }

    .empty {
      color: var(--muted);
      padding: 18px 0;
      font-size: 14px;
    }

    .search {
      margin-bottom: 15px;
    }

    .abc-bar {
      height: 9px;
      border-radius: 20px;
      background: #dbeafe;
      overflow: hidden;
      min-width: 120px;
    }

    .abc-bar span {
      display: block;
      height: 100%;
      background: var(--primary);
    }

    .modal {
      display: none;
      position: fixed;
      inset: 0;
      background: rgba(15, 23, 42, 0.58);
      z-index: 10;
      align-items: center;
      justify-content: center;
      padding: 20px;
    }

    .modal.open {
      display: flex;
    }

    .modal-content {
      width: min(700px, 100%);
      max-height: 90vh;
      overflow-y: auto;
      background: white;
      border-radius: 12px;
      padding: 22px;
    }

    .modal-header {
      display: flex;
      justify-content: space-between;
      gap: 12px;
      margin-bottom: 18px;
    }

    .close {
      border: 0;
      background: transparent;
      font-size: 25px;
      color: var(--muted);
    }

    @media (max-width: 1050px) {
      .cards {
        grid-template-columns: repeat(2, 1fr);
      }

      .grid-2 {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 750px) {
      .sidebar {
        width: 100%;
        height: auto;
        position: relative;
      }

      .layout {
        display: block;
      }

      .content {
        width: 100%;
        margin-left: 0;
        padding: 18px;
      }

      .menu {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
      }

      .cards {
        grid-template-columns: 1fr;
      }

      .form-grid {
        grid-template-columns: 1fr;
      }

      .topbar {
        display: block;
      }

      .topbar .actions {
        margin-top: 12px;
      }
    }
  </style>
</head>

<body>
  <div class="layout">
    <aside class="sidebar">
      <div class="brand">Gestão Comercial</div>

      <nav class="menu">
        <button class="menu-btn active" data-view="dashboard">Dashboard</button>
        <button class="menu-btn" data-view="clientes">Clientes</button>
        <button class="menu-btn" data-view="produtos">Produtos</button>
        <button class="menu-btn" data-view="fornecedores">Fornecedores</button>
        <button class="menu-btn" data-view="pedidos">Pedidos</button>
        <button class="menu-btn" data-view="financeiro">Financeiro</button>
      </nav>
    </aside>

    <main class="content">
      <div class="topbar">
        <div>
          <h1 id="page-title">Dashboard</h1>
          <div class="date" id="current-date"></div>
        </div>

        <div class="actions">
          <button class="btn btn-success" onclick="carregarDadosFicticios()">
            Carregar dados fictícios
          </button>
          <button class="btn btn-outline" onclick="resetarDados()">
            Limpar dados de teste
          </button>
        </div>
      </div>

      <!-- DASHBOARD -->
      <section id="dashboard" class="view active">
        <div class="cards">
          <div class="card">
            <div class="indicator-title">Clientes cadastrados</div>
            <div class="indicator-value" id="indicator-clientes">0</div>
          </div>

          <div class="card">
            <div class="indicator-title">Produtos cadastrados</div>
            <div class="indicator-value" id="indicator-produtos">0</div>
          </div>

          <div class="card">
            <div class="indicator-title">Pedidos realizados</div>
            <div class="indicator-value" id="indicator-pedidos">0</div>
          </div>

          <div class="card">
            <div class="indicator-title">Faturamento lançado</div>
            <div class="indicator-value" id="indicator-faturamento">R$ 0,00</div>
          </div>
        </div>

        <div class="grid-2">
          <div class="table-card">
            <h2 class="section-title">Pendências de garantia</h2>
            <div id="warranty-alerts" class="alert-list"></div>
          </div>

          <div class="table-card">
            <h2 class="section-title">Aniversários de hoje</h2>
            <div id="birthday-alerts" class="alert-list"></div>
          </div>
        </div>

        <div class="table-card">
          <h2 class="section-title">Curva ABC dos produtos</h2>
          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Classificação</th>
                  <th>Produto</th>
                  <th>Quantidade | Faturamento</th>
                  <th>Participação</th>
                  <th>Visualização</th>
                </tr>
              </thead>
              <tbody id="abc-table"></tbody>
            </table>
          </div>
        </div>

        <div class="table-card">
          <h2 class="section-title">Curva ABC dos clientes</h2>
          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Classificação</th>
                  <th>Cliente</th>
                  <th>Pedidos</th>
                  <th>Faturamento</th>
                  <th>Participação</th>
                  <th>Visualização</th>
                </tr>
              </thead>
              <tbody id="abc-clients-table"></tbody>
            </table>
          </div>
        </div>

        <div class="table-card">
          <h2 class="section-title">Análises para decisão</h2>
          <ul id="decision-analysis" style="padding-left: 20px; line-height: 1.9;"></ul>
        </div>
      </section>

      <!-- CLIENTES -->
      <section id="clientes" class="view">
        <div class="form-card">
          <h2 class="section-title">Cadastrar cliente</h2>

          <form id="client-form">
            <div class="form-grid">
              <div class="form-group">
                <label>Nome do cliente</label>
                <input id="client-name" required />
              </div>

              <div class="form-group">
                <label>Telefone</label>
                <input id="client-phone" placeholder="Ex.: 88999999999" />
              </div>

              <div class="form-group">
                <label>Data de nascimento</label>
                <input id="client-birthday" type="date" />
              </div>

              <div class="form-group">
                <label>Empresa ou cidade</label>
                <input id="client-company" />
              </div>

              <div class="form-group full">
                <label>Observações</label>
                <textarea id="client-notes"></textarea>
              </div>
            </div>

            <button class="btn btn-primary">Salvar cliente</button>
          </form>
        </div>

        <div class="table-card">
          <h2 class="section-title">Clientes cadastrados</h2>
          <input class="search" id="client-search" placeholder="Pesquisar cliente..." />

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Nome</th>
                  <th>Telefone</th>
                  <th>Aniversário</th>
                  <th>Empresa/cidade</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="clients-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- PRODUTOS -->
      <section id="produtos" class="view">
        <div class="form-card">
          <h2 class="section-title">Cadastrar produto</h2>

          <form id="product-form">
            <div class="form-grid">
              <div class="form-group">
                <label>Nome da peça</label>
                <input id="product-name" required />
              </div>

              <div class="form-group">
                <label>Fornecedor</label>
                <select id="product-supplier">
                  <option value="">Selecione</option>
                </select>
              </div>

              <div class="form-group">
                <label>Categoria</label>
                <input id="product-category" placeholder="Ex.: Freio, motor, suspensão" />
              </div>

              <div class="form-group">
                <label>Preço unitário</label>
                <input id="product-price" type="number" min="0" step="0.01" required />
              </div>
            </div>

            <button class="btn btn-primary">Salvar produto</button>
          </form>
        </div>

        <div class="table-card">
          <h2 class="section-title">Produtos cadastrados</h2>

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Código interno</th>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Categoria</th>
                  <th>Preço</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="products-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- FORNECEDORES -->
      <section id="fornecedores" class="view">
        <div class="form-card">
          <h2 class="section-title">Cadastrar fornecedor</h2>

          <form id="supplier-form">
            <div class="form-grid">
              <div class="form-group">
                <label>Nome do fornecedor</label>
                <input id="supplier-name" required />
              </div>

              <div class="form-group">
                <label>Telefone</label>
                <input id="supplier-phone" />
              </div>

              <div class="form-group">
                <label>Documento</label>
                <input id="supplier-document" placeholder="CNPJ ou CPF" />
              </div>

              <div class="form-group">
                <label>Observações</label>
                <input id="supplier-notes" />
              </div>
            </div>

            <button class="btn btn-primary">Salvar fornecedor</button>
          </form>
        </div>

        <div class="table-card">
          <h2 class="section-title">Fornecedores cadastrados</h2>

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Nome</th>
                  <th>Telefone</th>
                  <th>Documento</th>
                  <th>Peças cadastradas</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="suppliers-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- PEDIDOS -->
      <section id="pedidos" class="view">
        <div class="form-card">
          <h2 class="section-title">Lançar pedido do cliente</h2>

          <form id="order-form">
            <div class="form-grid">
              <div class="form-group">
                <label>Cliente</label>
                <select id="order-client" required>
                  <option value="">Selecione</option>
                </select>
              </div>

              <div class="form-group">
                <label>Vendedor</label>
                <input id="order-seller" required />
              </div>

              <div class="form-group">
                <label>Canal da venda</label>
                <select id="order-channel">
                  <option value="Presencial">Presencial</option>
                  <option value="Digital">Digital</option>
                  <option value="WhatsApp">WhatsApp</option>
                </select>
              </div>

              <div class="form-group">
                <label>Observação</label>
                <input id="order-notes" />
              </div>
            </div>

            <div class="form-group">
              <label>Produtos do pedido</label>
              <div id="order-products"></div>
            </div>

            <button class="btn btn-primary">Salvar pedido</button>
          </form>
        </div>

        <div class="table-card">
          <h2 class="section-title">Pedidos lançados</h2>

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Data</th>
                  <th>Cliente</th>
                  <th>Vendedor</th>
                  <th>Canal</th>
                  <th>Produtos</th>
                  <th>Total</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="orders-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- FINANCEIRO -->
      <section id="financeiro" class="view">
        <div class="form-card">
          <h2 class="section-title">Lançar movimentação financeira</h2>

          <form id="finance-form">
            <div class="form-grid">
              <div class="form-group">
                <label>Tipo</label>
                <select id="finance-type">
                  <option value="receber">Conta a receber</option>
                  <option value="pagar">Conta a pagar</option>
                </select>
              </div>

              <div class="form-group">
                <label>Descrição</label>
                <input id="finance-description" required />
              </div>

              <div class="form-group">
                <label>Valor</label>
                <input id="finance-value" type="number" min="0" step="0.01" required />
              </div>

              <div class="form-group">
                <label>Data de vencimento</label>
                <input id="finance-due-date" type="date" required />
              </div>

              <div class="form-group">
                <label>Status</label>
                <select id="finance-status">
                  <option value="pendente">Pendente</option>
                  <option value="pago">Pago</option>
                </select>
              </div>
            </div>

            <button class="btn btn-primary">Salvar lançamento</button>
          </form>
        </div>

        <div class="table-card">
          <h2 class="section-title">Contas a pagar e receber</h2>

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Tipo</th>
                  <th>Descrição</th>
                  <th>Valor</th>
                  <th>Vencimento</th>
                  <th>Status</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="finance-table"></tbody>
            </table>
          </div>
        </div>

        <div class="table-card">
          <h2 class="section-title">DRE simplificada</h2>
          <div id="dre-summary"></div>
        </div>
      </section>
    </main>
  </div>

  <!-- MODAL DE DETALHES DO CLIENTE -->
  <div class="modal" id="client-modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2 id="modal-client-name">Detalhes do cliente</h2>
        <button class="close" onclick="fecharModal()">&times;</button>
      </div>

      <div id="client-details"></div>
    </div>
  </div>

  <script>
    const STORAGE_KEY = "gestao_comercial_v1";

    let db = JSON.parse(localStorage.getItem(STORAGE_KEY)) || {
      clients: [],
      products: [],
      suppliers: [],
      orders: [],
      finances: []
    };

    function salvarDados() {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(db));
    }

    function gerarId(prefixo) {
      return prefixo + "_" + Date.now() + "_" + Math.random().toString(36).substring(2, 8);
    }

    function gerarCodigoProduto() {
      const maior = db.products.reduce((max, produto) => {
        const numero = parseInt(String(produto.internalCode || "").replace(/\D/g, ""), 10);
        return Number.isFinite(numero) && numero > max ? numero : max;
      }, 0);

      return `P-${String(maior + 1).padStart(5, "0")}`;
    }

    function formatarMoeda(valor) {
      return Number(valor || 0).toLocaleString("pt-BR", {
        style: "currency",
        currency: "BRL"
      });
    }

    function formatarData(data) {
      if (!data) return "-";

      return new Date(data + "T00:00:00").toLocaleDateString("pt-BR");
    }

    function dataAtual() {
      const agora = new Date();
      const dois = n => String(n).padStart(2, "0");

      return `${agora.getFullYear()}-${dois(agora.getMonth() + 1)}-${dois(agora.getDate())}`;
    }

    function escaparHTML(texto) {
      return String(texto || "")
        .replaceAll("&", "&")
        .replaceAll("<", "<")
        .replaceAll(">", ">")
        .replaceAll('"', "&quot;")
        .replaceAll("'", "&#039;");
    }

    function obterCliente(id) {
      return db.clients.find(cliente => cliente.id === id);
    }

    function obterProduto(id) {
      return db.products.find(produto => produto.id === id);
    }

    function obterFornecedor(id) {
      return db.suppliers.find(fornecedor => fornecedor.id === id);
    }

    function adicionarTimeline(clienteId, tipo, descricao, dados = {}) {
      const cliente = obterCliente(clienteId);

      if (!cliente) return;

      if (!cliente.timeline) {
        cliente.timeline = [];
      }

      cliente.timeline.unshift({
        id: gerarId("timeline"),
        data: new Date().toISOString(),
        tipo,
        descricao,
        dados
      });
    }

    function mostrarAviso(mensagem) {
      alert(mensagem);
    }

    function renderizarTudo() {
      renderizarIndicadores();
      renderizarSelects();
      renderizarClientes();
      renderizarProdutos();
      renderizarFornecedores();
      renderizarPedidos();
      renderizarFinanceiro();
      renderizarGarantias();
      renderizarAniversarios();
      renderizarCurvaABC();
      renderizarCurvaABCClientes();
      renderizarAnalises();
    }

    function renderizarIndicadores() {
      document.getElementById("indicator-clientes").textContent = db.clients.length;
      document.getElementById("indicator-produtos").textContent = db.products.length;
      document.getElementById("indicator-pedidos").textContent = db.orders.length;

      const faturamento = db.orders.reduce((total, pedido) => {
        return total + calcularTotalPedido(pedido);
      }, 0);

      document.getElementById("indicator-faturamento").textContent =
        formatarMoeda(faturamento);
    }

    function renderizarSelects() {
      const supplierSelect = document.getElementById("product-supplier");
      const clientSelect = document.getElementById("order-client");

      const fornecedorSelecionado = supplierSelect.value;
      const clienteSelecionado = clientSelect.value;

      supplierSelect.innerHTML =
        '<option value="">Selecione</option>' +
        db.suppliers.map(fornecedor =>
          `<option value="${fornecedor.id}">${escaparHTML(fornecedor.name)}</option>`
        ).join("");

      clientSelect.innerHTML =
        '<option value="">Selecione</option>' +
        db.clients.map(cliente =>
          `<option value="${cliente.id}">${escaparHTML(cliente.name)}</option>`
        ).join("");

      supplierSelect.value = fornecedorSelecionado;
      clientSelect.value = clienteSelecionado;

      const productsContainer = document.getElementById("order-products");

      if (!db.products.length) {
        productsContainer.innerHTML =
          '<p class="empty">Cadastre produtos antes de lançar um pedido.</p>';
        return;
      }

      productsContainer.innerHTML = db.products.map(produto => `
        <div style="display:grid; grid-template-columns: 1fr 110px 140px; gap:8px; margin-bottom:8px; align-items:center;">
          <label style="font-weight:normal;">
            <input
              type="checkbox"
              class="order-product-check"
              value="${produto.id}"
              style="width:auto; margin-right:6px;"
            />
            ${escaparHTML(produto.name)} (${escaparHTML(produto.internalCode)})
          </label>

          <input
            type="number"
            min="1"
            value="1"
            class="order-product-quantity"
            data-product-id="${produto.id}"
            placeholder="Quantidade"
          />

          <label style="font-weight:normal;">
            <input
              type="checkbox"
              class="order-product-warranty"
              data-product-id="${produto.id}"
              style="width:auto; margin-right:5px;"
            />
            Ativar garantia
          </label>
        </div>
      `).join("");
    }

    function renderizarClientes() {
      const termo = (document.getElementById("client-search")?.value || "")
        .toLowerCase();

      const clientes = db.clients.filter(cliente =>
        cliente.name.toLowerCase().includes(termo)
      );

      const tbody = document.getElementById("clients-table");

      if (!clientes.length) {
        tbody.innerHTML = `<tr><td colspan="5" class="empty">Nenhum cliente cadastrado.</td></tr>`;
        return;
      }

      tbody.innerHTML = clientes.map(cliente => `
        <tr>
          <td><strong>${escaparHTML(cliente.name)}</strong></td>
          <td>${escaparHTML(cliente.phone || "-")}</td>
          <td>${formatarData(cliente.birthday)}</td>
          <td>${escaparHTML(cliente.company || "-")}</td>
          <td>
            <div class="actions">
              <button class="btn btn-primary btn-small" onclick="verDetalhesCliente('${cliente.id}')">
                Ver timeline
              </button>
              ${
                cliente.phone
                  ? `<button class="btn btn-success btn-small" onclick="enviarWhatsApp('${cliente.id}')">WhatsApp</button>`
                  : ""
              }
              <button class="btn btn-danger btn-small" onclick="excluirCliente('${cliente.id}')">
                Excluir
              </button>
            </div>
          </td>
        </tr>
      `).join("");
    }

    function renderizarProdutos() {
      const tbody = document.getElementById("products-table");

      if (!db.products.length) {
        tbody.innerHTML = `<tr><td colspan="6" class="empty">Nenhum produto cadastrado.</td></tr>`;
        return;
      }

      tbody.innerHTML = db.products.map(produto => {
        const fornecedor = obterFornecedor(produto.supplierId);

        return `
          <tr>
            <td><span class="badge badge-gray">${escaparHTML(produto.internalCode)}</span></td>
            <td><strong>${escaparHTML(produto.name)}</strong></td>
            <td>${escaparHTML(fornecedor?.name || "Não informado")}</td>
            <td>${escaparHTML(produto.category || "-")}</td>
            <td>${formatarMoeda(produto.price)}</td>
            <td>
              <button class="btn btn-danger btn-small" onclick="excluirProduto('${produto.id}')">
                Excluir
              </button>
            </td>
          </tr>
        `;
      }).join("");
    }

    function renderizarFornecedores() {
      const tbody = document.getElementById("suppliers-table");

      if (!db.suppliers.length) {
        tbody.innerHTML = `<tr><td colspan="5" class="empty">Nenhum fornecedor cadastrado.</td></tr>`;
        return;
      }

      tbody.innerHTML = db.suppliers.map(fornecedor => {
        const quantidadeProdutos = db.products.filter(
          produto => produto.supplierId === fornecedor.id
        ).length;

        return `
          <tr>
            <td><strong>${escaparHTML(fornecedor.name)}</strong></td>
            <td>${escaparHTML(fornecedor.phone || "-")}</td>
            <td>${escaparHTML(fornecedor.document || "-")}</td>
            <td>${quantidadeProdutos}</td>
            <td>
              <button class="btn btn-danger btn-small" onclick="excluirFornecedor('${fornecedor.id}')">
                Excluir
              </button>
            </td>
          </tr>
        `;
      }).join("");
    }

    function calcularTotalPedido(pedido) {
      return pedido.items.reduce((total, item) => {
        const produto = obterProduto(item.productId);
        return total + ((produto?.price || 0) * item.quantity);
      }, 0);
    }

    function renderizarPedidos() {
      const tbody = document.getElementById("orders-table");

      if (!db.orders.length) {
        tbody.innerHTML = `<tr><td colspan="7" class="empty">Nenhum pedido lançado.</td></tr>`;
        return;
      }

      tbody.innerHTML = db.orders.map(pedido => {
        const cliente = obterCliente(pedido.clientId);

        const produtos = pedido.items.map(item => {
          const produto = obterProduto(item.productId);
          const garantia = item.warrantyActive
            ? '<span class="badge badge-green">Garantia ativa</span>'
            : "";

          return `
            <div style="margin-bottom:5px;">
              ${item.quantity}x ${escaparHTML(produto?.name || "Produto removido")}
              ${garantia}
            </div>
          `;
        }).join("");

        return `
          <tr>
            <td>${formatarData(pedido.date)}</td>
            <td>${escaparHTML(cliente?.name || "Cliente removido")}</td>
            <td>${escaparHTML(pedido.seller)}</td>
            <td>${escaparHTML(pedido.channel)}</td>
            <td>${produtos}</td>
            <td><strong>${formatarMoeda(calcularTotalPedido(pedido))}</strong></td>
            <td>
              <button class="btn btn-danger btn-small" onclick="excluirPedido('${pedido.id}')">
                Excluir
              </button>
            </td>
          </tr>
        `;
      }).join("");
    }

    function renderizarFinanceiro() {
      const tbody = document.getElementById("finance-table");

      if (!db.finances.length) {
        tbody.innerHTML = `<tr><td colspan="6" class="empty">Nenhum lançamento financeiro.</td></tr>`;
      } else {
        tbody.innerHTML = db.finances.map(item => `
          <tr>
            <td>
              ${
                item.type === "receber"
                  ? '<span class="badge badge-green">A receber</span>'
                  : '<span class="badge badge-red">A pagar</span>'
              }
            </td>
            <td>${escaparHTML(item.description)}</td>
            <td><strong>${formatarMoeda(item.value)}</strong></td>
            <td>${formatarData(item.dueDate)}</td>
            <td>
              ${
                item.status === "pago"
                  ? '<span class="badge badge-green">Pago</span>'
                  : '<span class="badge badge-yellow">Pendente</span>'
              }
            </td>
            <td>
              <button class="btn btn-danger btn-small" onclick="excluirFinanceiro('${item.id}')">
                Excluir
              </button>
            </td>
          </tr>
        `).join("");
      }

      const receber = db.finances
        .filter(item => item.type === "receber")
        .reduce((sum, item) => sum + Number(item.value), 0);

      const pagar = db.finances
        .filter(item => item.type === "pagar")
        .reduce((sum, item) => sum + Number(item.value), 0);

      const resultado = receber - pagar;

      document.getElementById("dre-summary").innerHTML = `
        <div class="cards" style="margin-bottom:0; grid-template-columns: repeat(3, 1fr);">
          <div class="card">
            <div class="indicator-title">Total a receber</div>
            <div class="indicator-value" style="color:var(--success);">
              ${formatarMoeda(receber)}
            </div>
          </div>

          <div class="card">
            <div class="indicator-title">Total a pagar</div>
            <div class="indicator-value" style="color:var(--danger);">
              ${formatarMoeda(pagar)}
            </div>
          </div>

          <div class="card">
            <div class="indicator-title">Resultado simplificado</div>
            <div class="indicator-value" style="color:${resultado >= 0 ? "var(--success)" : "var(--danger)"};">
              ${formatarMoeda(resultado)}
            </div>
          </div>
        </div>
      `;
    }

    function renderizarGarantias() {
      const alertBox = document.getElementById("warranty-alerts");
      const garantias = [];

      db.orders.forEach(pedido => {
        const cliente = obterCliente(pedido.clientId);

        pedido.items.forEach(item => {
          if (item.warrantyActive) {
            const produto = obterProduto(item.productId);

            garantias.push({
              cliente,
              produto,
              pedido,
              item
            });
          }
        });
      });

      if (!garantias.length) {
        alertBox.innerHTML =
          '<div class="empty">Nenhuma pendência de garantia ativa.</div>';
        return;
      }

      alertBox.innerHTML = garantias.map(garantia => `
        <div class="alert-item">
          <strong>
            Pendência: peça ${escaparHTML(garantia.produto?.name || "Produto")}
          </strong>

          <div>
            Cliente: ${escaparHTML(garantia.cliente?.name || "Cliente")}
          </div>

          <div style="font-size:13px; margin-top:5px;">
            Pedido realizado em ${formatarData(garantia.pedido.date)}
          </div>

          <div class="actions" style="margin-top:9px;">
            <span class="badge badge-green">Garantia ativa</span>
            <button
              class="btn btn-success btn-small"
              onclick="finalizarGarantia('${garantia.pedido.id}', '${garantia.item.id}')"
            >
              Finalizar garantia
            </button>
          </div>
        </div>
      `).join("");
    }

    function renderizarAniversarios() {
      const box = document.getElementById("birthday-alerts");
      const hoje = new Date();

      const aniversarios = db.clients.filter(cliente => {
        if (!cliente.birthday) return false;

        const nascimento = new Date(cliente.birthday + "T00:00:00");

        return (
          nascimento.getDate() === hoje.getDate() &&
          nascimento.getMonth() === hoje.getMonth()
        );
      });

      if (!aniversarios.length) {
        box.innerHTML =
          '<div class="empty">Nenhum aniversário hoje.</div>';
        return;
      }

      box.innerHTML = aniversarios.map(cliente => `
        <div class="alert-item" style="border-left-color:var(--success); background:var(--success-bg);">
          <strong>Aniversário de ${escaparHTML(cliente.name)}</strong>
          <div>Hoje é uma boa oportunidade para fortalecer o relacionamento.</div>

          <div class="actions" style="margin-top:9px;">
            ${
              cliente.phone
                ? `<button class="btn btn-success btn-small" onclick="enviarParabens('${cliente.id}')">Enviar parabéns</button>`
                : '<span class="badge badge-gray">Sem telefone cadastrado</span>'
            }
          </div>
        </div>
      `).join("");
    }

    /* ===== CURVA ABC ===== */

    function classificarABC(acumuladoAnterior) {
      if (acumuladoAnterior < 80) return "A";
      if (acumuladoAnterior < 95) return "B";
      return "C";
    }

    function classeBadgeABC(classe) {
      if (classe === "A") return "badge-green";
      if (classe === "B") return "badge-yellow";
      return "badge-red";
    }

    function renderizarCurvaABC() {
      const tbody = document.getElementById("abc-table");
      const vendas = {};

      db.orders.forEach(pedido => {
        pedido.items.forEach(item => {
          const produto = obterProduto(item.productId);
          if (!produto) return;

          if (!vendas[item.productId]) {
            vendas[item.productId] = { produto, quantidade: 0, valor: 0 };
          }

          vendas[item.productId].quantidade += Number(item.quantity);
          vendas[item.productId].valor += Number(item.quantity) * Number(produto.price);
        });
      });

      const ranking = Object.values(vendas).sort((a, b) => b.valor - a.valor);
      const totalValor = ranking.reduce((soma, item) => soma + item.valor, 0);

      if (!ranking.length) {
        tbody.innerHTML =
          '<tr><td colspan="5" class="empty">Lance pedidos para gerar a curva ABC.</td></tr>';
        return;
      }

      let acumulado = 0;

      tbody.innerHTML = ranking.map(item => {
        const participacao = totalValor ? (item.valor / totalValor) * 100 : 0;
        const classe = classificarABC(acumulado);
        acumulado += participacao;

        return `
          <tr>
            <td><span class="badge ${classeBadgeABC(classe)}">${classe}</span></td>
            <td>${escaparHTML(item.produto.name)}</td>
            <td>${item.quantidade} un. | ${formatarMoeda(item.valor)}</td>
            <td>${participacao.toFixed(1)}%</td>
            <td>
              <div class="abc-bar">
                <span style="width:${Math.min(participacao * 4, 100)}%;"></span>
              </div>
            </td>
          </tr>
        `;
      }).join("");
    }

    function renderizarCurvaABCClientes() {
      const tbody = document.getElementById("abc-clients-table");
      const compras = {};

      db.orders.forEach(pedido => {
        const cliente = obterCliente(pedido.clientId);
        if (!cliente) return;

        if (!compras[cliente.id]) {
          compras[cliente.id] = { cliente, pedidos: 0, valor: 0 };
        }

        compras[cliente.id].pedidos += 1;
        compras[cliente.id].valor += calcularTotalPedido(pedido);
      });

      const ranking = Object.values(compras).sort((a, b) => b.valor - a.valor);
      const totalValor = ranking.reduce((soma, item) => soma + item.valor, 0);

      if (!ranking.length) {
        tbody.innerHTML =
          '<tr><td colspan="6" class="empty">Lance pedidos para gerar a curva ABC de clientes.</td></tr>';
        return;
      }

      let acumulado = 0;

      tbody.innerHTML = ranking.map(item => {
        const participacao = totalValor ? (item.valor / totalValor) * 100 : 0;
        const classe = classificarABC(acumulado);
        acumulado += participacao;

        return `
          <tr>
            <td><span class="badge ${classeBadgeABC(classe)}">${classe}</span></td>
            <td>${escaparHTML(item.cliente.name)}</td>
            <td>${item.pedidos}</td>
            <td>${formatarMoeda(item.valor)}</td>
            <td>${participacao.toFixed(1)}%</td>
            <td>
              <div class="abc-bar">
                <span style="width:${Math.min(participacao * 4, 100)}%;"></span>
              </div>
            </td>
          </tr>
        `;
      }).join("");
    }

    function renderizarAnalises() {
      const lista = document.getElementById("decision-analysis");

      const totalVendas = db.orders.length;
      const vendasDigitais = db.orders.filter(
        pedido => pedido.channel === "Digital" || pedido.channel === "WhatsApp"
      ).length;

      const ticketMedio = totalVendas
        ? db.orders.reduce((sum, pedido) => sum + calcularTotalPedido(pedido), 0) / totalVendas
        : 0;

      const produtosSemVenda = db.products.filter(produto => {
        return !db.orders.some(pedido =>
          pedido.items.some(item => item.productId === produto.id)
        );
      });

      const clientesSemCompra = db.clients.filter(cliente => {
        return !db.orders.some(pedido => pedido.clientId === cliente.id);
      });

      lista.innerHTML = `
        <li><strong>Ticket médio atual:</strong> ${formatarMoeda(ticketMedio)}.</li>
        <li><strong>Vendas digitais:</strong> ${vendasDigitais} de ${totalVendas} pedidos.</li>
        <li><strong>Produtos sem venda registrada:</strong> ${produtosSemVenda.length}.</li>
        <li><strong>Clientes sem pedido registrado:</strong> ${clientesSemCompra.length}.</li>
        <li><strong>Garantias ativas:</strong> ${contarGarantiasAtivas()}.</li>
      `;
    }

    function contarGarantiasAtivas() {
      let total = 0;

      db.orders.forEach(pedido => {
        pedido.items.forEach(item => {
          if (item.warrantyActive) total++;
        });
      });

      return total;
    }

    /* ===== CLIENTE / TIMELINE ===== */

    function verDetalhesCliente(clienteId) {
      const cliente = obterCliente(clienteId);

      if (!cliente) return;

      const pedidos = db.orders.filter(pedido => pedido.clientId === clienteId);

      document.getElementById("modal-client-name").textContent =
        cliente.name;

      const timeline = cliente.timeline || [];

      document.getElementById("client-details").innerHTML = `
        <div class="card" style="box-shadow:none; margin-bottom:18px;">
          <p><strong>Telefone:</strong> ${escaparHTML(cliente.phone || "-")}</p>
          <p><strong>Aniversário:</strong> ${formatarData(cliente.birthday)}</p>
          <p><strong>Empresa/cidade:</strong> ${escaparHTML(cliente.company || "-")}</p>
          <p><strong>Observações:</strong> ${escaparHTML(cliente.notes || "-")}</p>
          <p><strong>Total de pedidos:</strong> ${pedidos.length}</p>
        </div>

        <h3 style="margin-bottom:12px;">Timeline do cliente</h3>

        ${
          timeline.length
            ? `<div class="timeline">
                ${timeline.map(item => `
                  <div class="timeline-item">
                    <strong>${escaparHTML(item.tipo)}</strong>
                    <div style="margin-top:4px;">${escaparHTML(item.descricao)}</div>
                    <small style="display:block; margin-top:7px; color:var(--muted);">
                      ${new Date(item.data).toLocaleString("pt-BR")}
                    </small>
                  </div>
                `).join("")}
              </div>`
            : '<div class="empty">Nenhum evento registrado ainda.</div>'
        }
      `;

      document.getElementById("client-modal").classList.add("open");
    }

    function fecharModal() {
      document.getElementById("client-modal").classList.remove("open");
    }

    function enviarWhatsApp(clienteId) {
      const cliente = obterCliente(clienteId);

      if (!cliente?.phone) {
        mostrarAviso("Este cliente não possui telefone cadastrado.");
        return;
      }

      const telefone = cliente.phone.replace(/\D/g, "");
      const mensagem = `Olá, ${cliente.name}! Entramos em contato para falar sobre seu atendimento.`;

      window.open(
        `https://wa.me/55${telefone}?text=${encodeURIComponent(mensagem)}`,
        "_blank"
      );
    }

    function enviarParabens(clienteId) {
      const cliente = obterCliente(clienteId);

      if (!cliente?.phone) {
        mostrarAviso("Este cliente não possui telefone cadastrado.");
        return;
      }

      const telefone = cliente.phone.replace(/\D/g, "");
      const mensagem =
        `Olá, ${cliente.name}! Desejamos a você um feliz aniversário, com muita saúde, felicidade e sucesso!`;

      window.open(
        `https://wa.me/55${telefone}?text=${encodeURIComponent(mensagem)}`,
        "_blank"
      );

      adicionarTimeline(
        clienteId,
        "Contato de aniversário",
        "Mensagem de parabéns preparada para envio pelo WhatsApp."
      );

      salvarDados();
      renderizarTudo();
    }

    function finalizarGarantia(pedidoId, itemId) {
      const pedido = db.orders.find(item => item.id === pedidoId);

      if (!pedido) return;

      const item = pedido.items.find(item => item.id === itemId);

      if (!item) return;

      item.warrantyActive = false;
      item.warrantyFinishedAt = new Date().toISOString();

      adicionarTimeline(
        pedido.clientId,
        "Garantia finalizada",
        `Garantia finalizada para o produto ${obterProduto(item.productId)?.name || ""}.`
      );

      salvarDados();
      renderizarTudo();
    }

    /* ===== EXCLUSÕES ===== */

    function excluirCliente(id) {
      if (!confirm("Deseja excluir este cliente?")) return;

      db.clients = db.clients.filter(cliente => cliente.id !== id);
      salvarDados();
      renderizarTudo();
    }

    function excluirProduto(id) {
      if (!confirm("Deseja excluir este produto?")) return;

      db.products = db.products.filter(produto => produto.id !== id);
      salvarDados();
      renderizarTudo();
    }

    function excluirFornecedor(id) {
      if (!confirm("Deseja excluir este fornecedor?")) return;

      db.suppliers = db.suppliers.filter(fornecedor => fornecedor.id !== id);
      salvarDados();
      renderizarTudo();
    }

    function excluirPedido(id) {
      if (!confirm("Deseja excluir este pedido?")) return;

      db.orders = db.orders.filter(pedido => pedido.id !== id);
      salvarDados();
      renderizarTudo();
    }

    function excluirFinanceiro(id) {
      if (!confirm("Deseja excluir este lançamento?")) return;

      db.finances = db.finances.filter(item => item.id !== id);
      salvarDados();
      renderizarTudo();
    }

    function resetarDados() {
      if (!confirm("Todos os dados deste navegador serão apagados. Continuar?")) {
        return;
      }

      localStorage.removeItem(STORAGE_KEY);
      location.reload();
    }

    /* ===== DADOS FICTÍCIOS ===== */

    function escolherPonderado(lista) {
      const total = lista.reduce((soma, item) => soma + item.peso, 0);
      let sorteio = Math.random() * total;

      for (const item of lista) {
        sorteio -= item.peso;
        if (sorteio <= 0) return item;
      }

      return lista[lista.length - 1];
    }

    function carregarDadosFicticios() {
      if (db.clients.length || db.products.length || db.orders.length) {
        if (!confirm("Já existem dados cadastrados. Os dados fictícios serão adicionados aos atuais. Continuar?")) {
          return;
        }
      }

      const agora = new Date();
      const dois = n => String(n).padStart(2, "0");

      // Fornecedores
      const fornecedores = ["Moto Parts Brasil", "Speed Peças Ltda", "Nordeste Motopeças"].map(nome => ({
        id: gerarId("fornecedor"),
        name: nome,
        phone: "88999990000",
        document: "00.000.000/0001-00",
        notes: "Dado fictício",
        createdAt: agora.toISOString()
      }));

      db.suppliers.push(...fornecedores);

      // Produtos: nome, categoria, preço e peso (quanto maior, mais vende)
      const catalogo = [
        ["Pastilha de freio dianteira", "Freio", 38.9, 30],
        ["Kit relação completo", "Transmissão", 189.9, 22],
        ["Vela de ignição", "Motor", 19.9, 20],
        ["Filtro de óleo", "Motor", 24.5, 16],
        ["Pneu traseiro 90/90-18", "Pneus", 219.0, 10],
        ["Amortecedor traseiro", "Suspensão", 245.0, 6],
        ["Cabo de embreagem", "Controles", 27.5, 5],
        ["Retrovisor par", "Acessórios", 59.9, 4],
        ["Bateria 5Ah", "Elétrica", 169.9, 3],
        ["Lâmpada de farol", "Elétrica", 14.9, 2],
        ["Corrente de comando", "Motor", 89.9, 1.5],
        ["Disco de freio", "Freio", 129.9, 1]
      ];

      const produtos = catalogo.map(([name, category, price, peso], indice) => {
        const produto = {
          id: gerarId("produto"),
          internalCode: gerarCodigoProduto(),
          name,
          supplierId: fornecedores[indice % fornecedores.length].id,
          category,
          price,
          createdAt: agora.toISOString()
        };

        db.products.push(produto);

        return { ...produto, peso };
      });

      // Clientes: nome e peso (clientes com peso alto compram mais)
      const listaClientes = [
        ["Oficina do Zé", 30], ["Moto Center Silva", 25], ["Auto Moto Cariri", 18],
        ["Mecânica Rápida", 12], ["Box Moto Peças", 8], ["Garagem do Beto", 6],
        ["Moto Service Norte", 5], ["Oficina Dois Irmãos", 4], ["Moto Fácil", 3],
        ["Renato Mototáxi", 2], ["Cleiton Entregas", 1.5], ["Lucas Motoboy", 1]
      ];

      const clientes = listaClientes.map(([name, peso], indice) => {
        const nascimento = indice === 0
          ? `1985-${dois(agora.getMonth() + 1)}-${dois(agora.getDate())}`
          : `1990-${dois((indice % 12) + 1)}-${dois((indice % 27) + 1)}`;

        const cliente = {
          id: gerarId("cliente"),
          name,
          phone: "88999991111",
          birthday: nascimento,
          company: "Juazeiro do Norte",
          notes: "Cliente fictício",
          createdAt: agora.toISOString(),
          timeline: [{
            id: gerarId("timeline"),
            data: agora.toISOString(),
            tipo: "Cliente cadastrado",
            descricao: "Cadastro inicial (dado fictício)."
          }]
        };

        db.clients.push(cliente);

        return { id: cliente.id, peso };
      });

      // Pedidos dos últimos 180 dias
      const vendedores = ["Carlos", "Ana", "Roberto"];
      const canais = ["Presencial", "Digital", "WhatsApp"];

      for (let i = 0; i < 90; i++) {
        const clienteSorteado = escolherPonderado(clientes);
        const clienteReal = db.clients.find(c => c.id === clienteSorteado.id);

        const dataPedido = new Date(agora);
        dataPedido.setDate(dataPedido.getDate() - Math.floor(Math.random() * 180));

        const dataTexto = `${dataPedido.getFullYear()}-${dois(dataPedido.getMonth() + 1)}-${dois(dataPedido.getDate())}`;

        const itens = [];
        const quantidadeItens = 1 + Math.floor(Math.random() * 3);

        for (let j = 0; j < quantidadeItens; j++) {
          const produto = escolherPonderado(produtos);

          if (itens.some(item => item.productId === produto.id)) continue;

          const garantia = Math.random() < 0.06;

          itens.push({
            id: gerarId("item"),
            productId: produto.id,
            quantity: 1 + Math.floor(Math.random() * 6),
            warrantyActive: garantia,
            warrantyActivatedAt: garantia ? dataPedido.toISOString() : null
          });
        }

        const vendedor = vendedores[Math.floor(Math.random() * vendedores.length)];
        const canal = canais[Math.floor(Math.random() * canais.length)];

        const pedido = {
          id: gerarId("pedido"),
          clientId: clienteReal.id,
          seller: vendedor,
          channel: canal,
          notes: "Pedido fictício",
          date: dataTexto,
          items: itens
        };

        db.orders.push(pedido);

        clienteReal.timeline.unshift({
          id: gerarId("timeline"),
          data: dataPedido.toISOString(),
          tipo: "Pedido lançado",
          descricao: `Pedido lançado pelo vendedor ${vendedor}, pelo canal ${canal}.`
        });

        itens.filter(item => item.warrantyActive).forEach(item => {
          const produto = obterProduto(item.productId);

          clienteReal.timeline.unshift({
            id: gerarId("timeline"),
            data: dataPedido.toISOString(),
            tipo: "Garantia ativada",
            descricao: `Garantia ativada para o produto ${produto?.name || ""}.`
          });
        });
      }

      db.orders.sort((a, b) => b.date.localeCompare(a.date));

      salvarDados();
      renderizarTudo();
      mostrarAviso("Dados fictícios carregados. Veja o Dashboard para conferir as curvas ABC.");
    }

    /* ===== MENU E FORMULÁRIOS ===== */

    document.querySelectorAll(".menu-btn").forEach(button => {
      button.addEventListener("click", () => {
        document.querySelectorAll(".menu-btn").forEach(btn =>
          btn.classList.remove("active")
        );

        document.querySelectorAll(".view").forEach(view =>
          view.classList.remove("active")
        );

        button.classList.add("active");

        const viewId = button.dataset.view;
        document.getElementById(viewId).classList.add("active");

        const titles = {
          dashboard: "Dashboard",
          clientes: "Clientes",
          produtos: "Produtos",
          fornecedores: "Fornecedores",
          pedidos: "Pedidos",
          financeiro: "Financeiro"
        };

        document.getElementById("page-title").textContent = titles[viewId];
      });
    });

    document.getElementById("client-form").addEventListener("submit", event => {
      event.preventDefault();

      const cliente = {
        id: gerarId("cliente"),
        name: document.getElementById("client-name").value.trim(),
        phone: document.getElementById("client-phone").value.trim(),
        birthday: document.getElementById("client-birthday").value,
        company: document.getElementById("client-company").value.trim(),
        notes: document.getElementById("client-notes").value.trim(),
        createdAt: new Date().toISOString(),
        timeline: []
      };

      cliente.timeline.push({
        id: gerarId("timeline"),
        data: new Date().toISOString(),
        tipo: "Cliente cadastrado",
        descricao: "Cadastro inicial realizado no sistema."
      });

      db.clients.push(cliente);
      salvarDados();
      event.target.reset();
      renderizarTudo();
      mostrarAviso("Cliente cadastrado com sucesso.");
    });

    document.getElementById("supplier-form").addEventListener("submit", event => {
      event.preventDefault();

      db.suppliers.push({
        id: gerarId("fornecedor"),
        name: document.getElementById("supplier-name").value.trim(),
        phone: document.getElementById("supplier-phone").value.trim(),
        document: document.getElementById("supplier-document").value.trim(),
        notes: document.getElementById("supplier-notes").value.trim(),
        createdAt: new Date().toISOString()
      });

      salvarDados();
      event.target.reset();
      renderizarTudo();
      mostrarAviso("Fornecedor cadastrado com sucesso.");
    });

    document.getElementById("product-form").addEventListener("submit", event => {
      event.preventDefault();

      const codigo = gerarCodigoProduto();

      db.products.push({
        id: gerarId("produto"),
        internalCode: codigo,
        name: document.getElementById("product-name").value.trim(),
        supplierId: document.getElementById("product-supplier").value,
        category: document.getElementById("product-category").value.trim(),
        price: Number(document.getElementById("product-price").value),
        createdAt: new Date().toISOString()
      });

      salvarDados();
      event.target.reset();
      renderizarTudo();
      mostrarAviso(`Produto cadastrado com o código interno ${codigo}.`);
    });

    document.getElementById("order-form").addEventListener("submit", event => {
      event.preventDefault();

      const clientId = document.getElementById("order-client").value;
      const seller = document.getElementById("order-seller").value.trim();
      const channel = document.getElementById("order-channel").value;
      const notes = document.getElementById("order-notes").value.trim();

      if (!clientId) {
        mostrarAviso("Selecione um cliente.");
        return;
      }

      const checkedProducts = Array.from(
        document.querySelectorAll(".order-product-check:checked")
      );

      if (!checkedProducts.length) {
        mostrarAviso("Selecione pelo menos um produto.");
        return;
      }

      const items = checkedProducts.map(check => {
        const productId = check.value;
        const quantityInput = document.querySelector(
          `.order-product-quantity[data-product-id="${productId}"]`
        );
        const warrantyInput = document.querySelector(
          `.order-product-warranty[data-product-id="${productId}"]`
        );

        return {
          id: gerarId("item"),
          productId,
          quantity: Number(quantityInput.value) || 1,
          warrantyActive: warrantyInput.checked,
          warrantyActivatedAt: warrantyInput.checked
            ? new Date().toISOString()
            : null
        };
      });

      const pedido = {
        id: gerarId("pedido"),
        clientId,
        seller,
        channel,
        notes,
        date: dataAtual(),
        items
      };

      db.orders.unshift(pedido);

      adicionarTimeline(
        clientId,
        "Pedido lançado",
        `Pedido lançado pelo vendedor ${seller}, pelo canal ${channel}.`,
        { orderId: pedido.id }
      );

      items.forEach(item => {
        if (item.warrantyActive) {
          const produto = obterProduto(item.productId);

          adicionarTimeline(
            clientId,
            "Garantia ativada",
            `Garantia ativada para o produto ${produto?.name || ""}.`,
            { orderId: pedido.id, productId: item.productId }
          );
        }
      });

      salvarDados();
      event.target.reset();
      renderizarTudo();
      mostrarAviso("Pedido lançado com sucesso.");
    });

    document.getElementById("finance-form").addEventListener("submit", event => {
      event.preventDefault();

      db.finances.push({
        id: gerarId("financeiro"),
        type: document.getElementById("finance-type").value,
        description: document.getElementById("finance-description").value.trim(),
        value: Number(document.getElementById("finance-value").value),
        dueDate: document.getElementById("finance-due-date").value,
        status: document.getElementById("finance-status").value,
        createdAt: new Date().toISOString()
      });

      salvarDados();
      event.target.reset();
      renderizarTudo();
      mostrarAviso("Lançamento financeiro salvo.");
    });

    document.getElementById("client-search").addEventListener("input", () => {
      renderizarClientes();
    });

    document.getElementById("current-date").textContent =
      new Date().toLocaleDateString("pt-BR", {
        weekday: "long",
        year: "numeric",
        month: "long",
        day: "numeric"
      });

    renderizarTudo();
  </script>
</body>
</html>
