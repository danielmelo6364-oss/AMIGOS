<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gestão Comercial</title>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>

  <style>
    :root {
      --black: #090909;
      --black-2: #121212;
      --black-3: #1b1b1b;
      --red: #e50914;
      --red-dark: #a80710;
      --white: #ffffff;
      --gray: #a8a8a8;
      --gray-2: #666;
      --border: #303030;
      --green: #24c77a;
      --yellow: #f2bd38;
      --blue: #4e9cff;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      background: var(--black);
      color: var(--white);
      font-family: Arial, Helvetica, sans-serif;
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

    .app {
      display: flex;
      min-height: 100vh;
    }

    .sidebar {
      width: 245px;
      background: #050505;
      border-right: 1px solid var(--border);
      padding: 22px 14px;
      position: fixed;
      inset: 0 auto 0 0;
      z-index: 10;
    }

    .brand {
      color: var(--red);
      font-size: 23px;
      font-weight: 800;
      margin: 0 10px 28px;
      letter-spacing: .5px;
    }

    .brand small {
      display: block;
      color: var(--gray);
      font-size: 10px;
      font-weight: normal;
      margin-top: 5px;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    .nav-btn {
      width: 100%;
      text-align: left;
      background: transparent;
      color: #bbb;
      border: 0;
      border-radius: 7px;
      padding: 13px 12px;
      margin: 3px 0;
      transition: .2s;
    }

    .nav-btn:hover,
    .nav-btn.active {
      background: var(--red);
      color: white;
    }

    .main {
      margin-left: 245px;
      width: calc(100% - 245px);
      padding: 28px;
    }

    .topbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 15px;
      margin-bottom: 25px;
    }

    h1,
    h2,
    h3 {
      margin: 0;
    }

    h1 {
      font-size: 27px;
    }

    h2 {
      font-size: 20px;
      margin-bottom: 17px;
    }

    h3 {
      font-size: 16px;
      margin-bottom: 12px;
    }

    .muted {
      color: var(--gray);
      font-size: 13px;
    }

    .btn {
      border: 1px solid var(--border);
      border-radius: 6px;
      padding: 10px 14px;
      color: white;
      background: var(--black-3);
    }

    .btn:hover {
      filter: brightness(1.25);
    }

    .btn-primary {
      background: var(--red);
      border-color: var(--red);
    }

    .btn-danger {
      background: #4c0b0f;
      border-color: #8d131a;
    }

    .btn-success {
      background: #095b3a;
      border-color: #18865a;
    }

    .btn-small {
      padding: 6px 9px;
      font-size: 12px;
    }

    .page {
      display: none;
    }

    .page.active {
      display: block;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 15px;
      margin-bottom: 23px;
    }

    .card,
    .panel {
      background: var(--black-2);
      border: 1px solid var(--border);
      border-radius: 9px;
      padding: 18px;
    }

    .metric {
      color: var(--gray);
      font-size: 12px;
      text-transform: uppercase;
      letter-spacing: .6px;
    }

    .metric-value {
      font-size: 27px;
      font-weight: bold;
      margin-top: 10px;
    }

    .red {
      color: var(--red);
    }

    .green {
      color: var(--green);
    }

    .yellow {
      color: var(--yellow);
    }

    .form-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 12px;
    }

    .form-grid.two {
      grid-template-columns: repeat(2, 1fr);
    }

    .form-grid.four {
      grid-template-columns: repeat(4, 1fr);
    }

    .field {
      display: flex;
      flex-direction: column;
      gap: 6px;
    }

    .field.full {
      grid-column: 1 / -1;
    }

    label {
      color: #d4d4d4;
      font-size: 12px;
    }

    input,
    select,
    textarea {
      width: 100%;
      color: white;
      background: #0b0b0b;
      border: 1px solid var(--border);
      border-radius: 5px;
      padding: 10px;
      outline: none;
    }

    input:focus,
    select:focus,
    textarea:focus {
      border-color: var(--red);
    }

    textarea {
      min-height: 76px;
      resize: vertical;
    }

    .form-actions {
      display: flex;
      gap: 9px;
      margin-top: 15px;
      flex-wrap: wrap;
    }

    .toolbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
      margin-bottom: 15px;
      flex-wrap: wrap;
    }

    .toolbar input {
      max-width: 320px;
    }

    .table-wrap {
      overflow-x: auto;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      min-width: 700px;
    }

    th,
    td {
      border-bottom: 1px solid var(--border);
      padding: 12px 9px;
      text-align: left;
      font-size: 13px;
      vertical-align: middle;
    }

    th {
      color: var(--gray);
      font-size: 11px;
      text-transform: uppercase;
    }

    tr.clickable {
      cursor: pointer;
    }

    tr.clickable:hover {
      background: #202020;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      border-radius: 20px;
      padding: 4px 8px;
      font-size: 11px;
      white-space: nowrap;
    }

    .badge-a {
      background: #531116;
      color: #ff7880;
    }

    .badge-b {
      background: #493b0c;
      color: #f4d36a;
    }

    .badge-c {
      background: #173b56;
      color: #7ab9ff;
    }

    .supplier-list {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
    }

    .supplier-chip {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      border-radius: 20px;
      padding: 5px 8px;
      font-size: 11px;
      border: 1px solid #444;
      background: #272727;
    }

    .supplier-chip.inactive {
      color: #777;
      background: #171717;
      border-color: #2e2e2e;
    }

    .dot {
      width: 9px;
      height: 9px;
      border-radius: 50%;
      display: inline-block;
      border: 1px solid #888;
    }

    .alert {
      border-left: 4px solid var(--yellow);
      background: #211b08;
      color: #f2d77a;
      padding: 12px;
      border-radius: 5px;
      margin-bottom: 15px;
      font-size: 13px;
    }

    .danger-alert {
      border-left-color: var(--red);
      background: #270b0d;
      color: #ff9ca1;
    }

    .profile-header {
      display: flex;
      justify-content: space-between;
      gap: 15px;
      align-items: flex-start;
      margin-bottom: 18px;
    }

    .profile-layout {
      display: grid;
      grid-template-columns: 1.1fr .9fr;
      gap: 15px;
    }

    .list {
      display: flex;
      flex-direction: column;
      gap: 8px;
    }

    .list-item {
      border: 1px solid var(--border);
      background: #101010;
      border-radius: 6px;
      padding: 11px;
    }

    .list-item strong {
      display: block;
      margin-bottom: 5px;
    }

    .empty {
      color: var(--gray);
      text-align: center;
      padding: 25px 10px;
      font-size: 13px;
    }

    .modal {
      position: fixed;
      inset: 0;
      background: rgba(0, 0, 0, .78);
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      z-index: 30;
    }

    .modal.show {
      display: flex;
    }

    .modal-box {
      background: var(--black-2);
      border: 1px solid #444;
      border-top: 3px solid var(--red);
      border-radius: 9px;
      width: min(900px, 100%);
      max-height: 92vh;
      overflow: auto;
      padding: 21px;
    }

    .modal-title {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 18px;
    }

    .close {
      background: transparent;
      border: 0;
      color: #aaa;
      font-size: 23px;
    }

    .product-line {
      display: grid;
      grid-template-columns: 1fr 100px 130px 42px;
      gap: 8px;
      margin-bottom: 8px;
      align-items: end;
    }

    .mini-total {
      color: var(--green);
      font-weight: bold;
      padding-bottom: 10px;
    }

    .image-preview {
      max-width: 150px;
      max-height: 100px;
      margin-top: 8px;
      border-radius: 5px;
    }

    @media (max-width: 1000px) {
      .cards {
        grid-template-columns: repeat(2, 1fr);
      }

      .profile-layout {
        grid-template-columns: 1fr;
      }

      .form-grid,
      .form-grid.four {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media (max-width: 700px) {
      .sidebar {
        width: 64px;
        padding: 15px 7px;
      }

      .brand {
        font-size: 0;
        text-align: center;
      }

      .brand::before {
        content: "G";
        font-size: 24px;
      }

      .brand small,
      .nav-btn span {
        display: none;
      }

      .nav-btn {
        text-align: center;
        padding: 12px 5px;
        font-size: 18px;
      }

      .main {
        margin-left: 64px;
        width: calc(100% - 64px);
        padding: 16px;
      }

      .cards {
        grid-template-columns: 1fr 1fr;
        gap: 8px;
      }

      .card {
        padding: 13px;
      }

      .metric-value {
        font-size: 21px;
      }

      .form-grid,
      .form-grid.two,
      .form-grid.four {
        grid-template-columns: 1fr;
      }

      .field.full {
        grid-column: auto;
      }

      .product-line {
        grid-template-columns: 1fr 80px 105px 35px;
      }

      h1 {
        font-size: 22px;
      }
    }
  </style>
</head>

<body>
  <div class="app">
    <aside class="sidebar">
      <div class="brand">
        GESTÃO
        <small>representação comercial</small>
      </div>

      <button class="nav-btn active" data-page="dashboard">▣ <span>Dashboard</span></button>
      <button class="nav-btn" data-page="clientes">♙ <span>Clientes</span></button>
      <button class="nav-btn" data-page="produtos">▤ <span>Produtos</span></button>
      <button class="nav-btn" data-page="fornecedores">◉ <span>Fornecedores</span></button>
      <button class="nav-btn" data-page="abc">▥ <span>Curva ABC</span></button>
    </aside>

    <main class="main">
      <div class="topbar">
        <div>
          <h1 id="pageTitle">Dashboard</h1>
          <div class="muted">Controle comercial e análise de clientes</div>
        </div>
        <button class="btn btn-primary" onclick="openSaleModal()">+ Nova venda</button>
      </div>

      <!-- DASHBOARD -->
      <section class="page active" id="page-dashboard">
        <div id="dashboardAlerts"></div>

        <div class="cards">
          <div class="card">
            <div class="metric">Clientes cadastrados</div>
            <div class="metric-value" id="metricClients">0</div>
          </div>
          <div class="card">
            <div class="metric">Produtos cadastrados</div>
            <div class="metric-value" id="metricProducts">0</div>
          </div>
          <div class="card">
            <div class="metric">Vendas realizadas</div>
            <div class="metric-value" id="metricSales">0</div>
          </div>
          <div class="card">
            <div class="metric">Faturamento total</div>
            <div class="metric-value green" id="metricRevenue">R$ 0,00</div>
          </div>
        </div>

        <div class="profile-layout">
          <div class="panel">
            <h2>Clientes inativos</h2>
            <div id="inactiveClients"></div>
          </div>

          <div class="panel">
            <h2>Produtos sem pedidos</h2>
            <div id="unusedProducts"></div>
          </div>
        </div>
      </section>

      <!-- CLIENTES -->
      <section class="page" id="page-clientes">
        <div class="panel">
          <h2>Cadastrar cliente</h2>

          <form id="clientForm">
            <div class="form-grid">
              <div class="field">
                <label>Nome completo *</label>
                <input id="clientName" required>
              </div>

              <div class="field">
                <label>Telefone / WhatsApp</label>
                <input id="clientPhone">
              </div>

              <div class="field">
                <label>E-mail</label>
                <input id="clientEmail" type="email">
              </div>

              <div class="field">
                <label>Data de nascimento</label>
                <input id="clientBirth" type="date">
              </div>

              <div class="field">
                <label>Cidade</label>
                <input id="clientCity">
              </div>

              <div class="field">
                <label>Observações</label>
                <input id="clientNotes">
              </div>
            </div>

            <div class="form-actions">
              <button class="btn btn-primary">Salvar cliente</button>
            </div>
          </form>
        </div>

        <div class="panel" style="margin-top:15px">
          <div class="toolbar">
            <h2>Clientes cadastrados</h2>
            <input id="clientSearch" placeholder="Buscar cliente..." oninput="renderClients()">
          </div>
          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Cliente</th>
                  <th>Contato</th>
                  <th>Última compra</th>
                  <th>Status</th>
                  <th>Compras</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="clientsTable"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- PRODUTOS -->
      <section class="page" id="page-produtos">
        <div class="panel">
          <h2>Cadastrar produto</h2>

          <form id="productForm">
            <div class="form-grid">
              <div class="field">
                <label>Nome do produto *</label>
                <input id="productName" required>
              </div>

              <div class="field">
                <label>Fornecedor *</label>
                <select id="productSupplier" required></select>
              </div>

              <div class="field">
                <label>Preço de venda *</label>
                <input id="productPrice" type="number" step="0.01" min="0" required>
              </div>

              <div class="field">
                <label>Categoria</label>
                <input id="productCategory">
              </div>

              <div class="field">
                <label>Observações</label>
                <input id="productNotes">
              </div>
            </div>

            <div class="form-actions">
              <button class="btn btn-primary">Salvar produto</button>
            </div>
          </form>
        </div>

        <div class="panel" style="margin-top:15px">
          <div class="toolbar">
            <h2>Produtos cadastrados</h2>
            <input id="productSearch" placeholder="Buscar produto..." oninput="renderProducts()">
          </div>
          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Código</th>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Categoria</th>
                  <th>Preço</th>
                  <th>Quantidade vendida</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="productsTable"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- FORNECEDORES -->
      <section class="page" id="page-fornecedores">
        <div class="panel">
          <h2>Cadastrar fornecedor</h2>

          <form id="supplierForm">
            <div class="form-grid">
              <div class="field">
                <label>Nome do fornecedor *</label>
                <input id="supplierName" required>
              </div>

              <div class="field">
                <label>Contato</label>
                <input id="supplierContact">
              </div>

              <div class="field">
                <label>Cor de identificação</label>
                <input id="supplierColor" type="color" value="#e50914">
              </div>
            </div>

            <div class="form-actions">
              <button class="btn btn-primary">Salvar fornecedor</button>
            </div>
          </form>
        </div>

        <div class="panel" style="margin-top:15px">
          <h2>Fornecedores cadastrados</h2>
          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Fornecedor</th>
                  <th>Contato</th>
                  <th>Cor</th>
                  <th>Produtos</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="suppliersTable"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- ABC -->
      <section class="page" id="page-abc">
        <div class="panel">
          <div class="toolbar">
            <div>
              <h2>Curva ABC de clientes</h2>
              <div class="muted">Clique em um cliente para consultar os pedidos, fornecedores e oportunidades.</div>
            </div>
            <select id="abcPeriod" onchange="renderABC()">
              <option value="all">Todo o período</option>
              <option value="365">Últimos 365 dias</option>
              <option value="90">Últimos 90 dias</option>
              <option value="30">Últimos 30 dias</option>
            </select>
          </div>

          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Cliente</th>
                  <th>Classificação</th>
                  <th>Fornecedores comprados</th>
                  <th>Pedidos</th>
                  <th>Itens</th>
                  <th>Faturamento</th>
                  <th>Última compra</th>
                </tr>
              </thead>
              <tbody id="abcTable"></tbody>
            </table>
          </div>
        </div>

        <div class="panel" style="margin-top:15px">
          <h2>Curva ABC de produtos</h2>
          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Classificação</th>
                  <th>Quantidade</th>
                  <th>Faturamento</th>
                  <th>Clientes</th>
                </tr>
              </thead>
              <tbody id="abcProductsTable"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- PERFIL DO CLIENTE -->
      <section class="page" id="page-profile">
        <div id="clientProfile"></div>
      </section>
    </main>
  </div>

  <!-- MODAL VENDA -->
  <div class="modal" id="saleModal">
    <div class="modal-box">
      <div class="modal-title">
        <h2>Nova venda</h2>
        <button class="close" onclick="closeModal('saleModal')">×</button>
      </div>

      <form id="saleForm">
        <div class="form-grid four">
          <div class="field">
            <label>Cliente *</label>
            <select id="saleClient" required></select>
          </div>

          <div class="field">
            <label>Data *</label>
            <input id="saleDate" type="date" required>
          </div>

          <div class="field">
            <label>Vendedor</label>
            <input id="saleSeller">
          </div>

          <div class="field">
            <label>Canal</label>
            <select id="saleChannel">
              <option>Presencial</option>
              <option>WhatsApp</option>
              <option>Telefone</option>
              <option>Site</option>
              <option>Outro</option>
            </select>
          </div>
        </div>

        <h3 style="margin-top:20px">Produtos do pedido</h3>
        <div id="saleLines"></div>

        <button type="button" class="btn btn-small" onclick="addSaleLine()">+ Adicionar produto</button>

        <div class="field" style="margin-top:15px">
          <label>Observações do pedido</label>
          <textarea id="saleNotes"></textarea>
        </div>

        <div style="text-align:right;margin-top:15px;font-size:18px">
          Total: <strong class="green" id="saleTotal">R$ 0,00</strong>
        </div>

        <div class="form-actions">
          <button class="btn btn-primary">Salvar venda</button>
          <button type="button" class="btn" onclick="closeModal('saleModal')">Cancelar</button>
        </div>
      </form>
    </div>
  </div>

  <!-- MODAL PEDIDO -->
  <div class="modal" id="orderModal">
    <div class="modal-box">
      <div class="modal-title">
        <h2>Detalhes do pedido</h2>
        <button class="close" onclick="closeModal('orderModal')">×</button>
      </div>
      <div id="orderDetails"></div>
    </div>
  </div>

  <script>
    const STORAGE_KEY = "gestao_comercial_black_red_v1";

    let db = JSON.parse(localStorage.getItem(STORAGE_KEY)) || {
      clients: [],
      products: [],
      suppliers: [],
      sales: [],
      attachments: [],
      lowerReasons: []
    };

    function saveDB() {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(db));
    }

    function uid(prefix = "id") {
      return prefix + "_" + Date.now().toString(36) + Math.random().toString(36).slice(2, 7);
    }

    function money(value) {
      return Number(value || 0).toLocaleString("pt-BR", {
        style: "currency",
        currency: "BRL"
      });
    }

    function dateBR(value) {
      if (!value) return "—";
      const parts = value.split("-");
      if (parts.length !== 3) return value;
      return `${parts[2]}/${parts[1]}/${parts[0]}`;
    }

    function today() {
      return new Date().toISOString().slice(0, 10);
    }

    function escapeHTML(value) {
      return String(value ?? "").replace(/[&<>"']/g, char => ({
        "&": "&",
        "<": "<",
        ">": ">",
        '"': "&quot;",
        "'": "&#039;"
      }[char]));
    }

    function getSupplier(id) {
      return db.suppliers.find(s => s.id === id);
    }

    function getProduct(id) {
      return db.products.find(p => p.id === id);
    }

    function getClient(id) {
      return db.clients.find(c => c.id === id);
    }

    function supplierChip(supplier, active = true) {
      if (!supplier) return "";
      return `
        <span class="supplier-chip ${active ? "" : "inactive"}">
          <span class="dot" style="background:${active ? supplier.color : "#555"}"></span>
          ${escapeHTML(supplier.name)}
        </span>
      `;
    }

    function getClientSales(clientId) {
      return db.sales.filter(s => s.clientId === clientId);
    }

    function getSaleTotal(sale) {
      return (sale.items || []).reduce((total, item) => {
        return total + Number(item.quantity || 0) * Number(item.price || 0);
      }, 0);
    }

    function getClientStats(clientId, salesList = db.sales) {
      const sales = salesList.filter(s => s.clientId === clientId);
      const quantities = {};
      let revenue = 0;
      let items = 0;

      sales.forEach(sale => {
        revenue += getSaleTotal(sale);
        (sale.items || []).forEach(item => {
          quantities[item.productId] = (quantities[item.productId] || 0) + Number(item.quantity || 0);
          items += Number(item.quantity || 0);
        });
      });

      const lastSale = sales
        .map(s => s.date)
        .sort()
        .reverse()[0] || "";

      return {
        sales,
        quantities,
        revenue,
        items,
        lastSale
      };
    }

    function daysWithoutPurchase(client) {
      const stats = getClientStats(client.id);
      if (!stats.lastSale) return Infinity;

      const last = new Date(stats.lastSale + "T12:00:00");
      return Math.floor((new Date() - last) / 86400000);
    }

    function clientStatus(client) {
      const days = daysWithoutPurchase(client);
      if (days === Infinity) return "Nunca comprou";
      if (days > 45) return "Mais de 45 dias";
      if (days > 30) return "Mais de 30 dias";
      if (days > 15) return "Mais de 15 dias";
      return "Ativo";
    }

    function abcClass(index, total) {
      if (!total) return "C";
      const percentage = ((index + 1) / total) * 100;
      if (percentage <= 20) return "A";
      if (percentage <= 50) return "B";
      return "C";
    }

    function abcBadge(letter) {
      return `<span class="badge badge-${letter.toLowerCase()}">Classe ${letter}</span>`;
    }

    function showPage(page) {
      document.querySelectorAll(".page").forEach(el => el.classList.remove("active"));
      document.querySelectorAll(".nav-btn").forEach(el => el.classList.remove("active"));

      const pageElement = document.getElementById("page-" + page);
      if (pageElement) pageElement.classList.add("active");

      const nav = document.querySelector(`[data-page="${page}"]`);
      if (nav) nav.classList.add("active");

      const titles = {
        dashboard: "Dashboard",
        clientes: "Clientes",
        produtos: "Produtos",
        fornecedores: "Fornecedores",
        abc: "Curva ABC",
        profile: "Perfil do cliente"
      };

      document.getElementById("pageTitle").textContent = titles[page] || "Gestão";
    }

    document.querySelectorAll(".nav-btn").forEach(button => {
      button.addEventListener("click", () => {
        showPage(button.dataset.page);
        renderAll();
      });
    });

    function renderAll() {
      renderDashboard();
      renderClients();
      renderProducts();
      renderSuppliers();
      renderABC();
      updateSelects();
    }

    function renderDashboard() {
      const revenue = db.sales.reduce((sum, sale) => sum + getSaleTotal(sale), 0);

      document.getElementById("metricClients").textContent = db.clients.length;
      document.getElementById("metricProducts").textContent = db.products.length;
      document.getElementById("metricSales").textContent = db.sales.length;
      document.getElementById("metricRevenue").textContent = money(revenue);

      const inactive = db.clients
        .map(client => ({ client, days: daysWithoutPurchase(client) }))
        .filter(item => item.days > 15 || item.days === Infinity)
        .sort((a, b) => b.days - a.days);

      document.getElementById("inactiveClients").innerHTML = inactive.length
        ? inactive.map(item => `
          <div class="list-item" style="cursor:pointer" onclick="openClientProfile('${item.client.id}')">
            <strong>${escapeHTML(item.client.name)}</strong>
            <span class="muted">
              ${item.days === Infinity ? "Nunca comprou" : `${item.days} dias sem comprar`}
            </span>
          </div>
        `).join("")
        : `<div class="empty">Nenhum cliente inativo há mais de 15 dias.</div>`;

      const used = {};
      db.sales.forEach(sale => (sale.items || []).forEach(item => {
        used[item.productId] = (used[item.productId] || 0) + Number(item.quantity || 0);
      }));

      const unused = db.products.filter(product => !used[product.id]);

      document.getElementById("unusedProducts").innerHTML = unused.length
        ? unused.map(product => `
          <div class="list-item">
            <strong>${escapeHTML(product.name)}</strong>
            <span class="muted">${escapeHTML(getSupplier(product.supplierId)?.name || "Sem fornecedor")}</span>
          </div>
        `).join("")
        : `<div class="empty">Todos os produtos já possuem pedidos.</div>`;

      const birthdays = db.clients.filter(client => {
        if (!client.birth) return false;
        const birth = client.birth.slice(5);
        return birth === today().slice(5);
      });

      let alerts = "";

      if (birthdays.length) {
        alerts += `<div class="alert">Aniversariantes de hoje: ${birthdays.map(c => escapeHTML(c.name)).join(", ")}</div>`;
      }

      if (inactive.length) {
        alerts += `<div class="alert danger-alert">${inactive.length} cliente(s) precisam de acompanhamento por inatividade.</div>`;
      }

      document.getElementById("dashboardAlerts").innerHTML = alerts;
    }

    document.getElementById("clientForm").addEventListener("submit", event => {
      event.preventDefault();

      db.clients.push({
        id: uid("cli"),
        name: document.getElementById("clientName").value.trim(),
        phone: document.getElementById("clientPhone").value.trim(),
        email: document.getElementById("clientEmail").value.trim(),
        birth: document.getElementById("clientBirth").value,
        city: document.getElementById("clientCity").value.trim(),
        notes: document.getElementById("clientNotes").value.trim(),
        createdAt: today()
      });

      saveDB();
      event.target.reset();
      renderAll();
      alert("Cliente salvo com sucesso.");
    });

    function renderClients() {
      const search = (document.getElementById("clientSearch")?.value || "").toLowerCase();

      const clients = db.clients.filter(client =>
        client.name.toLowerCase().includes(search) ||
        (client.phone || "").toLowerCase().includes(search)
      );

      document.getElementById("clientsTable").innerHTML = clients.length
        ? clients.map(client => {
          const stats = getClientStats(client.id);
          const status = clientStatus(client);

          return `
            <tr class="clickable" onclick="openClientProfile('${client.id}')">
              <td><strong>${escapeHTML(client.name)}</strong><br><span class="muted">${escapeHTML(client.city || "")}</span></td>
              <td>${escapeHTML(client.phone || "—")}<br><span class="muted">${escapeHTML(client.email || "")}</span></td>
              <td>${dateBR(stats.lastSale)}</td>
              <td>
                <span class="badge ${status === "Ativo" ? "badge-c" : "badge-a"}">${status}</span>
              </td>
              <td>${stats.sales.length} pedido(s)</td>
              <td>
                <button class="btn btn-small" onclick="event.stopPropagation();openClientProfile('${client.id}')">Abrir perfil</button>
                <button class="btn btn-small btn-danger" onclick="event.stopPropagation();deleteClient('${client.id}')">Excluir</button>
              </td>
            </tr>
          `;
        }).join("")
        : `<tr><td colspan="6" class="empty">Nenhum cliente cadastrado.</td></tr>`;
    }

    function deleteClient(id) {
      const client = getClient(id);
      if (!client) return;

      if (!confirm(`Excluir o cliente ${client.name}? As vendas também serão removidas.`)) return;

      db.clients = db.clients.filter(c => c.id !== id);
      db.sales = db.sales.filter(s => s.clientId !== id);
      db.attachments = db.attachments.filter(a => a.clientId !== id);
      db.lowerReasons = db.lowerReasons.filter(r => r.clientId !== id);

      saveDB();
      renderAll();
    }

    document.getElementById("supplierForm").addEventListener("submit", event => {
      event.preventDefault();

      db.suppliers.push({
        id: uid("sup"),
        name: document.getElementById("supplierName").value.trim(),
        contact: document.getElementById("supplierContact").value.trim(),
        color: document.getElementById("supplierColor").value
      });

      saveDB();
      event.target.reset();
      document.getElementById("supplierColor").value = "#e50914";
      renderAll();
      alert("Fornecedor salvo com sucesso.");
    });

    function renderSuppliers() {
      document.getElementById("suppliersTable").innerHTML = db.suppliers.length
        ? db.suppliers.map(supplier => {
          const products = db.products.filter(p => p.supplierId === supplier.id);

          return `
            <tr>
              <td>
                <span class="dot" style="background:${supplier.color}"></span>
                <strong>${escapeHTML(supplier.name)}</strong>
              </td>
              <td>${escapeHTML(supplier.contact || "—")}</td>
              <td><span class="supplier-chip"><span class="dot" style="background:${supplier.color}"></span>${supplier.color}</span></td>
              <td>${products.length}</td>
              <td>
                <button class="btn btn-small btn-danger" onclick="deleteSupplier('${supplier.id}')">Excluir</button>
              </td>
            </tr>
          `;
        }).join("")
        : `<tr><td colspan="5" class="empty">Nenhum fornecedor cadastrado.</td></tr>`;
    }

    function deleteSupplier(id) {
      if (db.products.some(product => product.supplierId === id)) {
        alert("Não é possível excluir um fornecedor que possui produtos vinculados.");
        return;
      }

      db.suppliers = db.suppliers.filter(s => s.id !== id);
      saveDB();
      renderAll();
    }

    document.getElementById("productForm").addEventListener("submit", event => {
      event.preventDefault();

      const code = "P" + String(db.products.length + 1).padStart(4, "0");

      db.products.push({
        id: uid("prod"),
        code,
        name: document.getElementById("productName").value.trim(),
        supplierId: document.getElementById("productSupplier").value,
        price: Number(document.getElementById("productPrice").value || 0),
        category: document.getElementById("productCategory").value.trim(),
        notes: document.getElementById("productNotes").value.trim()
      });

      saveDB();
      event.target.reset();
      renderAll();
      alert("Produto salvo com sucesso.");
    });

    function renderProducts() {
      const search = (document.getElementById("productSearch")?.value || "").toLowerCase();

      const products = db.products.filter(product =>
        product.name.toLowerCase().includes(search) ||
        product.code.toLowerCase().includes(search)
      );

      document.getElementById("productsTable").innerHTML = products.length
        ? products.map(product => {
          const supplier = getSupplier(product.supplierId);
          const quantity = db.sales.reduce((sum, sale) => {
            const item = (sale.items || []).find(i => i.productId === product.id);
            return sum + Number(item?.quantity || 0);
          }, 0);

          return `
            <tr>
              <td>${escapeHTML(product.code)}</td>
              <td><strong>${escapeHTML(product.name)}</strong></td>
              <td>${supplier ? supplierChip(supplier) : "—"}</td>
              <td>${escapeHTML(product.category || "—")}</td>
              <td>${money(product.price)}</td>
              <td>${quantity}</td>
              <td>
                <button class="btn btn-small btn-danger" onclick="deleteProduct('${product.id}')">Excluir</button>
              </td>
            </tr>
          `;
        }).join("")
        : `<tr><td colspan="7" class="empty">Nenhum produto cadastrado.</td></tr>`;
    }

    function deleteProduct(id) {
      if (db.sales.some(sale => sale.items.some(item => item.productId === id))) {
        alert("Este produto possui histórico de vendas e não pode ser excluído.");
        return;
      }

      db.products = db.products.filter(product => product.id !== id);
      saveDB();
      renderAll();
    }

    function updateSelects() {
      const productSelect = document.getElementById("productSupplier");
      productSelect.innerHTML = `<option value="">Selecione...</option>` +
        db.suppliers.map(supplier =>
          `<option value="${supplier.id}">${escapeHTML(supplier.name)}</option>`
        ).join("");

      const clientSelect = document.getElementById("saleClient");
      const currentClient = clientSelect.value;

      clientSelect.innerHTML = `<option value="">Selecione...</option>` +
        db.clients.map(client =>
          `<option value="${client.id}">${escapeHTML(client.name)}</option>`
        ).join("");

      if (currentClient) clientSelect.value = currentClient;
    }

    function openSaleModal(clientId = "") {
      updateSelects();
      document.getElementById("saleDate").value = today();
      document.getElementById("saleClient").value = clientId;
      document.getElementById("saleSeller").value = "";
      document.getElementById("saleNotes").value = "";
      document.getElementById("saleLines").innerHTML = "";
      addSaleLine();
      document.getElementById("saleModal").classList.add("show");
    }

    function addSaleLine(productId = "", quantity = 1) {
      const line = document.createElement("div");
      line.className = "product-line";

      line.innerHTML = `
        <div class="field">
          <label>Produto</label>
          <select class="sale-product" onchange="updateSaleTotal()">
            <option value="">Selecione...</option>
            ${db.products.map(product => `
              <option value="${product.id}" ${product.id === productId ? "selected" : ""}>
                ${escapeHTML(product.code)} - ${escapeHTML(product.name)} (${money(product.price)})
              </option>
            `).join("")}
          </select>
        </div>

        <div class="field">
          <label>Quantidade</label>
          <input class="sale-quantity" type="number" min="1" value="${quantity}" oninput="updateSaleTotal()">
        </div>

        <div class="mini-total">R$ 0,00</div>

        <button type="button" class="btn btn-small btn-danger" onclick="this.parentElement.remove();updateSaleTotal()">×</button>
      `;

      document.getElementById("saleLines").appendChild(line);
      updateSaleTotal();
    }

    function updateSaleTotal() {
      let total = 0;

      document.querySelectorAll(".product-line").forEach(line => {
        const product = getProduct(line.querySelector(".sale-product")?.value);
        const quantity = Number(line.querySelector(".sale-quantity")?.value || 0);
        const lineTotal = product ? product.price * quantity : 0;

        total += lineTotal;
        const display = line.querySelector(".mini-total");
        if (display) display.textContent = money(lineTotal);
      });

      document.getElementById("saleTotal").textContent = money(total);
    }

    document.getElementById("saleForm").addEventListener("submit", event => {
      event.preventDefault();

      const clientId = document.getElementById("saleClient").value;
      const lines = [];

      document.querySelectorAll(".product-line").forEach(line => {
        const productId = line.querySelector(".sale-product").value;
        const quantity = Number(line.querySelector(".sale-quantity").value || 0);
        const product = getProduct(productId);

        if (product && quantity > 0) {
          lines.push({
            productId,
            quantity,
            price: product.price,
            guarantee: false
          });
        }
      });

      if (!clientId) {
        alert("Selecione um cliente.");
        return;
      }

      if (!lines.length) {
        alert("Adicione pelo menos um produto.");
        return;
      }

      db.sales.push({
        id: uid("sale"),
        clientId,
        date: document.getElementById("saleDate").value,
        seller: document.getElementById("saleSeller").value.trim(),
        channel: document.getElementById("saleChannel").value,
        notes: document.getElementById("saleNotes").value.trim(),
        items: lines
      });

      saveDB();
      closeModal("saleModal");
      renderAll();
      alert("Venda registrada com sucesso.");
    });

    function renderABC() {
      const period = document.getElementById("abcPeriod")?.value || "all";
      let sales = db.sales;

      if (period !== "all") {
        const limit = new Date();
        limit.setDate(limit.getDate() - Number(period));
        sales = sales.filter(sale => new Date(sale.date + "T12:00:00") >= limit);
      }

      const rows = db.clients.map(client => {
        const stats = getClientStats(client.id, sales);
        const supplierIds = [];

        stats.sales.forEach(sale => (sale.items || []).forEach(item => {
          const product = getProduct(item.productId);
          if (product && !supplierIds.includes(product.supplierId)) {
            supplierIds.push(product.supplierId);
          }
        }));

        return {
          client,
          stats,
          supplierIds
        };
      }).sort((a, b) => b.stats.revenue - a.stats.revenue);

      document.getElementById("abcTable").innerHTML = rows.length
        ? rows.map((row, index) => `
          <tr class="clickable" onclick="openClientProfile('${row.client.id}')">
            <td><strong>${escapeHTML(row.client.name)}</strong></td>
            <td>${abcBadge(abcClass(index, rows.length))}</td>
            <td>
              <div class="supplier-list">
                ${db.suppliers.map(supplier =>
                  supplierChip(supplier, row.supplierIds.includes(supplier.id))
                ).join("") || "—"}
              </div>
            </td>
            <td>${row.stats.sales.length}</td>
            <td>${row.stats.items}</td>
            <td class="green">${money(row.stats.revenue)}</td>
            <td>${dateBR(row.stats.lastSale)}</td>
          </tr>
        `).join("")
        : `<tr><td colspan="7" class="empty">Cadastre clientes e vendas para visualizar a curva ABC.</td></tr>`;

      renderABCProducts(sales);
    }

    function renderABCProducts(sales = db.sales) {
      const rows = db.products.map(product => {
        let quantity = 0;
        let revenue = 0;
        const clients = [];

        sales.forEach(sale => {
          const item = (sale.items || []).find(i => i.productId === product.id);

          if (item) {
            quantity += Number(item.quantity || 0);
            revenue += Number(item.quantity || 0) * Number(item.price || 0);

            if (!clients.includes(sale.clientId)) {
              clients.push(sale.clientId);
            }
          }
        });

        return {
          product,
          quantity,
          revenue,
          clients
        };
      }).sort((a, b) => b.revenue - a.revenue);

      document.getElementById("abcProductsTable").innerHTML = rows.length
        ? rows.map((row, index) => {
          const supplier = getSupplier(row.product.supplierId);

          return `
            <tr>
              <td><strong>${escapeHTML(row.product.name)}</strong><br><span class="muted">${escapeHTML(row.product.code)}</span></td>
              <td>${supplier ? supplierChip(supplier) : "—"}</td>
              <td>${abcBadge(abcClass(index, rows.length))}</td>
              <td>${row.quantity}</td>
              <td class="green">${money(row.revenue)}</td>
              <td>${row.clients.length}</td>
            </tr>
          `;
        }).join("")
        : `<tr><td colspan="6" class="empty">Nenhum produto cadastrado.</td></tr>`;
    }

    function openClientProfile(clientId) {
      const client = getClient(clientId);
      if (!client) return;

      const stats = getClientStats(clientId);
      const boughtProductIds = Object.keys(stats.quantities);
      const boughtSupplierIds = [...new Set(
        boughtProductIds
          .map(productId => getProduct(productId)?.supplierId)
          .filter(Boolean)
      )];

      const globalProductAverage = {};
      db.clients.forEach(otherClient => {
        const otherStats = getClientStats(otherClient.id);

        Object.entries(otherStats.quantities).forEach(([productId, quantity]) => {
          if (!globalProductAverage[productId]) {
            globalProductAverage[productId] = {
              total: 0,
              clients: 0
            };
          }

          globalProductAverage[productId].total += quantity;
          globalProductAverage[productId].clients++;
        });
      });

      const suggestions = db.products
        .filter(product => !boughtProductIds.includes(product.id))
        .map(product => {
          const abcPosition = getProductABCPosition(product.id);
          const avg = globalProductAverage[product.id];
          return {
            product,
            abcPosition,
            avg: avg ? avg.total / avg.clients : 0
          };
        })
        .sort((a, b) => {
          if (a.abcPosition !== b.abcPosition) {
            return a.abcPosition - b.abcPosition;
          }
          return b.avg - a.avg;
        });

      const lowerPurchases = db.products
        .filter(product => boughtProductIds.includes(product.id))
        .map(product => {
          const clientQuantity = stats.quantities[product.id] || 0;
          const average = globalProductAverage[product.id]
            ? globalProductAverage[product.id].total / globalProductAverage[product.id].clients
            : 0;

          const savedReason = db.lowerReasons.find(
            reason => reason.clientId === clientId && reason.productId === product.id
          );

          return {
            product,
            clientQuantity,
            average,
            savedReason
          };
        })
        .filter(row => row.average > row.clientQuantity);

      document.getElementById("clientProfile").innerHTML = `
        <div class="profile-header">
          <div>
            <button class="btn btn-small" onclick="showPage('clientes');renderAll()">← Voltar</button>
            <h2 style="margin-top:15px">${escapeHTML(client.name)}</h2>
            <div class="muted">
              ${escapeHTML(client.phone || "Sem telefone")} ·
              ${escapeHTML(client.email || "Sem e-mail")} ·
              ${escapeHTML(client.city || "Sem cidade")}
            </div>
          </div>

          <div class="form-actions" style="margin-top:0">
            <button class="btn btn-primary" onclick="openSaleModal('${client.id}')">+ Nova venda</button>
            <button class="btn" onclick="document.getElementById('attachmentInput').click()">Anexar arquivo</button>
            <input id="attachmentInput" type="file" hidden onchange="saveAttachment('${client.id}', this.files[0])">
          </div>
        </div>

        <div class="cards">
          <div class="card">
            <div class="metric">Pedidos</div>
            <div class="metric-value">${stats.sales.length}</div>
          </div>
          <div class="card">
            <div class="metric">Itens comprados</div>
            <div class="metric-value">${stats.items}</div>
          </div>
          <div class="card">
            <div class="metric">Faturamento</div>
            <div class="metric-value green">${money(stats.revenue)}</div>
          </div>
          <div class="card">
            <div class="metric">Status</div>
            <div class="metric-value" style="font-size:18px">${clientStatus(client)}</div>
          </div>
        </div>

        <div class="profile-layout">
          <div>
            <div class="panel">
              <h2>Fornecedores comprados pelo cliente</h2>
              <div class="supplier-list">
                ${db.suppliers.map(supplier =>
                  supplierChip(supplier, boughtSupplierIds.includes(supplier.id))
                ).join("") || `<span class="muted">Nenhum fornecedor cadastrado.</span>`}
              </div>

              <div class="muted" style="margin-top:12px">
                <span class="dot" style="background:#555"></span> Cinza: ainda não comprou
                &nbsp;&nbsp;
                <span class="dot" style="background:var(--red)"></span> Cor ativa: já comprou
              </div>
            </div>

            <div class="panel" style="margin-top:15px">
              <h2>Pedidos do cliente</h2>
              <div class="list">
                ${stats.sales.length
                  ? stats.sales.sort((a, b) => b.date.localeCompare(a.date)).map(sale => `
                    <div class="list-item">
                      <strong>Pedido de ${dateBR(sale.date)} — ${money(getSaleTotal(sale))}</strong>
                      <div class="muted">${sale.items.length} produto(s) · ${escapeHTML(sale.channel || "Canal não informado")} · ${escapeHTML(sale.seller || "Vendedor não informado")}</div>
                      <div class="form-actions">
                        <button class="btn btn-small" onclick="openOrder('${sale.id}')">Ver pedido</button>
                        <button class="btn btn-small btn-primary" onclick="downloadOrderPDF('${sale.id}')">Baixar PDF</button>
                      </div>
                    </div>
                  `).join("")
                  : `<div class="empty">Este cliente ainda não possui pedidos.</div>`
                }
              </div>
            </div>

            <div class="panel" style="margin-top:15px">
              <h2>Anexos do cliente</h2>
              <div id="attachments-${client.id}">
                ${renderAttachments(client.id)}
              </div>
            </div>
          </div>

          <div>
            <div class="panel">
              <h2>Sugestões de produtos</h2>
              <div class="muted" style="margin-bottom:12px">
                Produtos que o cliente ainda não comprou, priorizados pela Curva ABC geral.
              </div>

              <div class="list">
                ${suggestions.length
                  ? suggestions.slice(0, 12).map(row => `
                    <div class="list-item">
                      <strong>${escapeHTML(row.product.name)}</strong>
                      <div class="muted">
                        ${abcBadge(row.abcPosition)} ·
                        Média da base: ${row.avg.toFixed(1)} unidade(s)
                      </div>
                    </div>
                  `).join("")
                  : `<div class="empty">Não há sugestões disponíveis.</div>`
                }
              </div>
            </div>

            <div class="panel" style="margin-top:15px">
              <h2>Comprou abaixo da média</h2>
              <div class="muted" style="margin-bottom:12px">
                A média considera os clientes que já compraram cada produto.
              </div>

              <div class="list">
                ${lowerPurchases.length
                  ? lowerPurchases.map(row => `
                    <div class="list-item">
                      <strong>${escapeHTML(row.product.name)}</strong>
                      <div class="muted">
                        Cliente: ${row.clientQuantity} · Média da base: ${row.average.toFixed(1)}
                      </div>

                      <div class="field" style="margin-top:9px">
                        <label>Motivo da compra menor</label>
                        <input
                          value="${escapeHTML(row.savedReason?.reason || "")}"
                          placeholder="Ex.: preço, preferência, baixa procura..."
                          onchange="saveLowerReason('${client.id}','${row.product.id}',this.value)"
                        >
                      </div>
                    </div>
                  `).join("")
                  : `<div class="empty">Nenhum produto abaixo da média identificado.</div>`
                }
              </div>
            </div>
          </div>
        </div>
      `;

      showPage("profile");
    }

    function getProductABCPosition(productId) {
      const rows = db.products.map(product => {
        const revenue = db.sales.reduce((sum, sale) => {
          const item = (sale.items || []).find(i => i.productId === product.id);
          return sum + Number(item?.quantity || 0) * Number(item?.price || 0);
        }, 0);

        return {
          id: product.id,
          revenue
        };
      }).sort((a, b) => b.revenue - a.revenue);

      const index = rows.findIndex(row => row.id === productId);
      return index >= 0 ? abcClass(index, rows.length) : "C";
    }

    function saveLowerReason(clientId, productId, reason) {
      const existing = db.lowerReasons.find(
        item => item.clientId === clientId && item.productId === productId
      );

      if (existing) {
        existing.reason = reason;
      } else {
        db.lowerReasons.push({
          id: uid("reason"),
          clientId,
          productId,
          reason
        });
      }

      saveDB();
    }

    function saveAttachment(clientId, file) {
      if (!file) return;

      const reader = new FileReader();

      reader.onload = () => {
        db.attachments.push({
          id: uid("file"),
          clientId,
          name: file.name,
          type: file.type,
          size: file.size,
          data: reader.result,
          date: today()
        });

        saveDB();
        openClientProfile(clientId);
      };

      reader.readAsDataURL(file);
    }

    function renderAttachments(clientId) {
      const attachments = db.attachments.filter(file => file.clientId === clientId);

      if (!attachments.length) {
        return `<div class="empty">Nenhum arquivo anexado.</div>`;
      }

      return `
        <div class="list">
          ${attachments.map(file => `
            <div class="list-item">
              <strong>${escapeHTML(file.name)}</strong>
              <div class="muted">${dateBR(file.date)} · ${formatBytes(file.size)}</div>
              <div class="form-actions">
                <a class="btn btn-small" href="${file.data}" download="${escapeHTML(file.name)}">Baixar</a>
                ${file.type.startsWith("image/")
                  ? `<img class="image-preview" src="${file.data}" alt="Pré-visualização">`
                  : ""
                }
                <button class="btn btn-small btn-danger" onclick="deleteAttachment('${file.id}','${clientId}')">Excluir</button>
              </div>
            </div>
          `).join("")}
        </div>
      `;
    }

    function formatBytes(bytes) {
      if (!bytes) return "0 B";
      const units = ["B", "KB", "MB", "GB"];
      const index = Math.floor(Math.log(bytes) / Math.log(1024));
      return `${(bytes / Math.pow(1024, index)).toFixed(1)} ${units[index]}`;
    }

    function deleteAttachment(fileId, clientId) {
      if (!confirm("Excluir este anexo?")) return;

      db.attachments = db.attachments.filter(file => file.id !== fileId);
      saveDB();
      openClientProfile(clientId);
    }

    function openOrder(saleId) {
      const sale = db.sales.find(item => item.id === saleId);
      if (!sale) return;

      const client = getClient(sale.clientId);

      document.getElementById("orderDetails").innerHTML = `
        <div class="card" style="margin-bottom:14px">
          <strong>${escapeHTML(client?.name || "Cliente removido")}</strong>
          <div class="muted">
            ${escapeHTML(client?.phone || "")} · ${escapeHTML(client?.email || "")}
          </div>
          <div class="muted" style="margin-top:7px">
            Data: ${dateBR(sale.date)} · Vendedor: ${escapeHTML(sale.seller || "—")} · Canal: ${escapeHTML(sale.channel || "—")}
          </div>
        </div>

        <div class="table-wrap">
          <table>
            <thead>
              <tr>
                <th>Produto</th>
                <th>Fornecedor</th>
                <th>Quantidade</th>
                <th>Preço unitário</th>
                <th>Total</th>
              </tr>
            </thead>
            <tbody>
              ${sale.items.map(item => {
                const product = getProduct(item.productId);
                const supplier = product ? getSupplier(product.supplierId) : null;

                return `
                  <tr>
                    <td>${escapeHTML(product?.name || "Produto removido")}</td>
                    <td>${supplier ? supplierChip(supplier) : "—"}</td>
                    <td>${item.quantity}</td>
                    <td>${money(item.price)}</td>
                    <td class="green">${money(item.quantity * item.price)}</td>
                  </tr>
                `;
              }).join("")}
            </tbody>
          </table>
        </div>

        <div style="text-align:right;font-size:20px;margin-top:18px">
          Total: <strong class="green">${money(getSaleTotal(sale))}</strong>
        </div>

        ${sale.notes ? `
          <div class="card" style="margin-top:15px">
            <strong>Observações</strong>
            <div class="muted" style="margin-top:7px">${escapeHTML(sale.notes)}</div>
          </div>
        ` : ""}

        <div class="form-actions">
          <button class="btn btn-primary" onclick="downloadOrderPDF('${sale.id}')">Baixar pedido em PDF</button>
          <button class="btn" onclick="closeModal('orderModal')">Fechar</button>
        </div>
      `;

      document.getElementById("orderModal").classList.add("show");
    }

    function downloadOrderPDF(saleId) {
      const sale = db.sales.find(item => item.id === saleId);
      if (!sale) return;

      const client = getClient(sale.clientId);
      const jsPDF = window.jspdf?.jsPDF;

      if (!jsPDF) {
        alert("A biblioteca de PDF não foi carregada. Verifique sua conexão com a internet.");
        return;
      }

      const doc = new jsPDF();
      let y = 20;

      doc.setFillColor(229, 9, 20);
      doc.rect(0, 0, 210, 10, "F");

      doc.setTextColor(0, 0, 0);
      doc.setFontSize(18);
      doc.text("PEDIDO COMERCIAL", 15, y);
      y += 10;

      doc.setFontSize(10);
      doc.text(`Cliente: ${client?.name || "—"}`, 15, y);
      y += 6;
      doc.text(`Telefone: ${client?.phone || "—"}`, 15, y);
      y += 6;
      doc.text(`E-mail: ${client?.email || "—"}`, 15, y);
      y += 6;
      doc.text(`Data: ${dateBR(sale.date)}`, 15, y);
      y += 6;
      doc.text(`Vendedor: ${sale.seller || "—"} | Canal: ${sale.channel || "—"}`, 15, y);
      y += 12;

      doc.setFillColor(35, 35, 35);
      doc.setTextColor(255, 255, 255);
      doc.rect(15, y - 5, 180, 8, "F");
      doc.text("Produto", 18, y);
      doc.text("Qtd.", 115, y);
      doc.text("Unitário", 140, y);
      doc.text("Total", 174, y);
      y += 9;

      doc.setTextColor(0, 0, 0);

      sale.items.forEach(item => {
        const product = getProduct(item.productId);
        const name = product?.name || "Produto removido";
        const lineTotal = item.quantity * item.price;

        doc.text(name.substring(0, 48), 18, y);
        doc.text(String(item.quantity), 118, y);
        doc.text(money(item.price), 140, y);
        doc.text(money(lineTotal), 174, y);
        y += 7;

        if (y > 270) {
          doc.addPage();
          y = 20;
        }
      });

      y += 8;
      doc.setFontSize(13);
      doc.text(`TOTAL: ${money(getSaleTotal(sale))}`, 145, y);

      if (sale.notes) {
        y += 12;
        doc.setFontSize(10);
        doc.text("Observações:", 15, y);
        y += 6;
        const notes = doc.splitTextToSize(sale.notes, 175);
        doc.text(notes, 15, y);
      }

      doc.save(`pedido-${client?.name || "cliente"}-${sale.date}.pdf`);
    }

    function closeModal(id) {
      document.getElementById(id).classList.remove("show");
    }

    document.querySelectorAll(".modal").forEach(modal => {
      modal.addEventListener("click", event => {
        if (event.target === modal) {
          modal.classList.remove("show");
        }
      });
    });

    document.getElementById("saleClient").addEventListener("change", updateSaleTotal);

    renderAll();
  </script>
</body>
</html>
