<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gestão Comercial</title>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>

  <style>
    :root {
      --black: #080808;
      --black-2: #121212;
      --black-3: #1c1c1c;
      --red: #e50914;
      --red-dark: #9f0710;
      --white: #fff;
      --gray: #a9a9a9;
      --border: #333;
      --green: #26c77b;
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
      min-height: 100vh;
      display: flex;
    }

    .sidebar {
      position: fixed;
      inset: 0 auto 0 0;
      z-index: 10;
      width: 245px;
      padding: 22px 14px;
      background: #050505;
      border-right: 1px solid var(--border);
    }

    .brand {
      margin: 0 10px 28px;
      color: var(--red);
      font-size: 23px;
      font-weight: bold;
      letter-spacing: .5px;
    }

    .brand small {
      display: block;
      margin-top: 5px;
      color: var(--gray);
      font-size: 10px;
      font-weight: normal;
      letter-spacing: 1px;
      text-transform: uppercase;
    }

    .nav-btn {
      width: 100%;
      margin: 3px 0;
      padding: 13px 12px;
      border: 0;
      border-radius: 7px;
      background: transparent;
      color: #bbb;
      text-align: left;
      transition: .2s;
    }

    .nav-btn:hover,
    .nav-btn.active {
      background: var(--red);
      color: white;
    }

    .main {
      width: calc(100% - 245px);
      margin-left: 245px;
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
      margin-bottom: 17px;
      font-size: 20px;
    }

    h3 {
      margin-bottom: 12px;
      font-size: 16px;
    }

    .muted {
      color: var(--gray);
      font-size: 13px;
    }

    .page {
      display: none;
    }

    .page.active {
      display: block;
    }

    .panel,
    .card {
      padding: 18px;
      border: 1px solid var(--border);
      border-radius: 9px;
      background: var(--black-2);
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 15px;
      margin-bottom: 23px;
    }

    .metric {
      color: var(--gray);
      font-size: 12px;
      letter-spacing: .5px;
      text-transform: uppercase;
    }

    .metric-value {
      margin-top: 10px;
      font-size: 27px;
      font-weight: bold;
    }

    .green {
      color: var(--green);
    }

    .yellow {
      color: var(--yellow);
    }

    .red {
      color: var(--red);
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
      padding: 10px;
      outline: none;
      border: 1px solid var(--border);
      border-radius: 5px;
      background: #0b0b0b;
      color: white;
    }

    input:focus,
    select:focus,
    textarea:focus {
      border-color: var(--red);
    }

    textarea {
      min-height: 80px;
      resize: vertical;
    }

    .form-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 9px;
      margin-top: 15px;
    }

    .btn {
      padding: 10px 14px;
      border: 1px solid var(--border);
      border-radius: 6px;
      background: var(--black-3);
      color: white;
    }

    .btn:hover {
      filter: brightness(1.25);
    }

    .btn-primary {
      border-color: var(--red);
      background: var(--red);
    }

    .btn-danger {
      border-color: #8d131a;
      background: #4c0b0f;
    }

    .btn-success {
      border-color: #19865c;
      background: #095b3a;
    }

    .btn-small {
      padding: 6px 9px;
      font-size: 12px;
    }

    .toolbar {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      margin-bottom: 15px;
    }

    .toolbar input {
      max-width: 320px;
    }

    .table-wrap {
      overflow-x: auto;
    }

    table {
      width: 100%;
      min-width: 850px;
      border-collapse: collapse;
    }

    th,
    td {
      padding: 12px 9px;
      border-bottom: 1px solid var(--border);
      text-align: left;
      vertical-align: middle;
      font-size: 13px;
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
      padding: 4px 8px;
      border-radius: 20px;
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
      padding: 5px 8px;
      border: 1px solid #444;
      border-radius: 20px;
      background: #272727;
      font-size: 11px;
      white-space: nowrap;
    }

    .supplier-chip.inactive {
      border-color: #2e2e2e;
      background: #171717;
      color: #777;
    }

    .dot {
      display: inline-block;
      width: 9px;
      height: 9px;
      border: 1px solid #888;
      border-radius: 50%;
    }

    .list {
      display: flex;
      flex-direction: column;
      gap: 8px;
    }

    .list-item {
      padding: 11px;
      border: 1px solid var(--border);
      border-radius: 6px;
      background: #101010;
    }

    .list-item strong {
      display: block;
      margin-bottom: 5px;
    }

    .empty {
      padding: 25px 10px;
      color: var(--gray);
      text-align: center;
      font-size: 13px;
    }

    .alert {
      margin-bottom: 15px;
      padding: 12px;
      border-left: 4px solid var(--yellow);
      border-radius: 5px;
      background: #211b08;
      color: #f2d77a;
      font-size: 13px;
    }

    .danger-alert {
      border-left-color: var(--red);
      background: #270b0d;
      color: #ff9ca1;
    }

    .profile-header {
      display: flex;
      align-items: flex-start;
      justify-content: space-between;
      gap: 15px;
      margin-bottom: 18px;
    }

    .profile-layout {
      display: grid;
      grid-template-columns: 1.1fr .9fr;
      gap: 15px;
    }

    .modal {
      position: fixed;
      inset: 0;
      z-index: 30;
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      background: rgba(0, 0, 0, .78);
    }

    .modal.show {
      display: flex;
    }

    .modal-box {
      width: min(950px, 100%);
      max-height: 92vh;
      overflow: auto;
      padding: 21px;
      border: 1px solid #444;
      border-top: 3px solid var(--red);
      border-radius: 9px;
      background: var(--black-2);
    }

    .modal-title {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 18px;
    }

    .close {
      border: 0;
      background: transparent;
      color: #aaa;
      font-size: 23px;
    }

    .product-line {
      display: grid;
      grid-template-columns: 1fr 100px 130px 42px;
      align-items: end;
      gap: 8px;
      margin-bottom: 8px;
    }

    .mini-total {
      padding-bottom: 10px;
      color: var(--green);
      font-weight: bold;
    }

    .image-preview {
      max-width: 150px;
      max-height: 100px;
      margin-top: 8px;
      border-radius: 5px;
    }

    .suggestion-box {
      max-height: 210px;
      overflow: auto;
    }

    @media (max-width: 1100px) {
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
        margin: 0 0 28px;
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
        padding: 12px 5px;
        text-align: center;
        font-size: 18px;
      }

      .main {
        width: calc(100% - 64px);
        margin-left: 64px;
        padding: 16px;
      }

      .form-grid,
      .form-grid.two,
      .form-grid.four {
        grid-template-columns: 1fr;
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
                  <th>Pedidos</th>
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

      <!-- CURVA ABC -->
      <section class="page" id="page-abc">
        <div class="panel">
          <div class="toolbar">
            <div>
              <h2>Curva ABC de clientes</h2>
              <div class="muted">
                Clique em qualquer cliente para abrir seus pedidos, fornecedores, sugestões e análise de compras.
              </div>
            </div>

            <select id="abcPeriod" onchange="renderABC()">
              <option value="all">Todo o período</option>
              <option value="365">Últimos 365 dias</option>
              <option value="90">Últimos 90 dias</option>
              <option value="30">Últimos 30 dias</option>
            </select>
          </div>

          <div class="alert">
            <strong>Classificação ABC:</strong>
            A representa até 80% do faturamento acumulado,
            B representa de 80% a 95%,
            C representa acima de 95%.
          </div>

          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Cliente</th>
                  <th>Classe ABC</th>
                  <th>Fornecedores comprados</th>
                  <th>Produtos comprados</th>
                  <th>Pedidos</th>
                  <th>Itens</th>
                  <th>Faturamento</th>
                  <th>Participação</th>
                  <th>Última compra</th>
                  <th>Ações</th>
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
                  <th>Classe ABC</th>
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

  <!-- MODAL DE VENDA -->
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

        <button type="button" class="btn btn-small" onclick="addSaleLine()">
          + Adicionar produto
        </button>

        <div class="field" style="margin-top:15px">
          <label>Observações do pedido</label>
          <textarea id="saleNotes"></textarea>
        </div>

        <div style="margin-top:15px;text-align:right;font-size:18px">
          Total:
          <strong class="green" id="saleTotal">R$ 0,00</strong>
        </div>

        <div class="form-actions">
          <button class="btn btn-primary">Salvar venda</button>
          <button type="button" class="btn" onclick="closeModal('saleModal')">Cancelar</button>
        </div>
      </form>
    </div>
  </div>

  <!-- MODAL DO PEDIDO -->
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
    const STORAGE_KEY = "gestao_comercial_corrigido_v2";

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

    function uid(prefix) {
      return prefix + "_" + Date.now().toString(36) + Math.random().toString(36).slice(2, 8);
    }

    function today() {
      return new Date().toISOString().slice(0, 10);
    }

    function money(value) {
      return Number(value || 0).toLocaleString("pt-BR", {
        style: "currency",
        currency: "BRL"
      });
    }

    function dateBR(value) {
      if (!value) return "—";

      const parts = String(value).split("-");

      if (parts.length !== 3) {
        return value;
      }

      return parts[2] + "/" + parts[1] + "/" + parts[0];
    }

    function escapeHTML(value) {
      return String(value ?? "").replace(/[&<>"']/g, function(char) {
        return {
          "&": "&",
          "<": "<",
          ">": ">",
          '"': "&quot;",
          "'": "&#039;"
        }[char];
      });
    }

    function getClient(id) {
      return db.clients.find(function(client) {
        return client.id === id;
      });
    }

    function getProduct(id) {
      return db.products.find(function(product) {
        return product.id === id;
      });
    }

    function getSupplier(id) {
      return db.suppliers.find(function(supplier) {
        return supplier.id === id;
      });
    }

    function getClientSales(clientId, salesList) {
      const source = salesList || db.sales;

      return source.filter(function(sale) {
        return sale.clientId === clientId;
      });
    }

    function getSaleTotal(sale) {
      return (sale.items || []).reduce(function(total, item) {
        return total + Number(item.quantity || 0) * Number(item.price || 0);
      }, 0);
    }

    function getProductQuantity(productId, salesList) {
      const source = salesList || db.sales;

      return source.reduce(function(total, sale) {
        return total + (sale.items || []).reduce(function(itemTotal, item) {
          if (item.productId === productId) {
            return itemTotal + Number(item.quantity || 0);
          }

          return itemTotal;
        }, 0);
      }, 0);
    }

    function getProductRevenue(productId, salesList) {
      const source = salesList || db.sales;

      return source.reduce(function(total, sale) {
        return total + (sale.items || []).reduce(function(itemTotal, item) {
          if (item.productId === productId) {
            return itemTotal + Number(item.quantity || 0) * Number(item.price || 0);
          }

          return itemTotal;
        }, 0);
      }, 0);
    }

    function getClientStats(clientId, salesList) {
      const sales = getClientSales(clientId, salesList);
      const quantities = {};
      let revenue = 0;
      let items = 0;

      sales.forEach(function(sale) {
        revenue += getSaleTotal(sale);

        (sale.items || []).forEach(function(item) {
          quantities[item.productId] = (quantities[item.productId] || 0) + Number(item.quantity || 0);
          items += Number(item.quantity || 0);
        });
      });

      const dates = sales
        .map(function(sale) {
          return sale.date;
        })
        .filter(Boolean)
        .sort()
        .reverse();

      return {
        sales: sales,
        quantities: quantities,
        revenue: revenue,
        items: items,
        lastSale: dates[0] || ""
      };
    }

    function daysWithoutPurchase(client) {
      const stats = getClientStats(client.id);

      if (!stats.lastSale) {
        return Infinity;
      }

      const lastDate = new Date(stats.lastSale + "T12:00:00");
      return Math.floor((new Date() - lastDate) / 86400000);
    }

    function clientStatus(client) {
      const days = daysWithoutPurchase(client);

      if (days === Infinity) return "Nunca comprou";
      if (days > 45) return "Mais de 45 dias";
      if (days > 30) return "Mais de 30 dias";
      if (days > 15) return "Mais de 15 dias";

      return "Ativo";
    }

    function supplierChip(supplier, active) {
      if (!supplier) return "";

      const isActive = active !== false;

      return `
        <span class="supplier-chip ${isActive ? "" : "inactive"}">
          <span
            class="dot"
            style="background:${isActive ? supplier.color : "#555"}">
          </span>
          ${escapeHTML(supplier.name)}
        </span>
      `;
    }

    function abcBadge(letter) {
      return `
        <span class="badge badge-${String(letter).toLowerCase()}">
          Classe ${letter}
        </span>
      `;
    }

    function showPage(page) {
      document.querySelectorAll(".page").forEach(function(element) {
        element.classList.remove("active");
      });

      document.querySelectorAll(".nav-btn").forEach(function(element) {
        element.classList.remove("active");
      });

      const target = document.getElementById("page-" + page);

      if (target) {
        target.classList.add("active");
      }

      const nav = document.querySelector('[data-page="' + page + '"]');

      if (nav) {
        nav.classList.add("active");
      }

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

    document.querySelectorAll(".nav-btn").forEach(function(button) {
      button.addEventListener("click", function() {
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
      const totalRevenue = db.sales.reduce(function(total, sale) {
        return total + getSaleTotal(sale);
      }, 0);

      document.getElementById("metricClients").textContent = db.clients.length;
      document.getElementById("metricProducts").textContent = db.products.length;
      document.getElementById("metricSales").textContent = db.sales.length;
      document.getElementById("metricRevenue").textContent = money(totalRevenue);

      const inactive = db.clients
        .map(function(client) {
          return {
            client: client,
            days: daysWithoutPurchase(client)
          };
        })
        .filter(function(item) {
          return item.days === Infinity || item.days > 15;
        })
        .sort(function(a, b) {
          if (a.days === Infinity) return -1;
          if (b.days === Infinity) return 1;
          return b.days - a.days;
        });

      document.getElementById("inactiveClients").innerHTML = inactive.length
        ? inactive.map(function(item) {
            return `
              <div
                class="list-item"
                style="cursor:pointer"
                onclick="openClientProfile('${item.client.id}')">

                <strong>${escapeHTML(item.client.name)}</strong>

                <span class="muted">
                  ${
                    item.days === Infinity
                      ? "Nunca comprou"
                      : item.days + " dias sem comprar"
                  }
                </span>
              </div>
            `;
          }).join("")
        : `<div class="empty">Nenhum cliente inativo há mais de 15 dias.</div>`;

      const unused = db.products.filter(function(product) {
        return getProductQuantity(product.id) === 0;
      });

      document.getElementById("unusedProducts").innerHTML = unused.length
        ? unused.map(function(product) {
            const supplier = getSupplier(product.supplierId);

            return `
              <div class="list-item">
                <strong>${escapeHTML(product.name)}</strong>
                <span class="muted">
                  ${supplier ? escapeHTML(supplier.name) : "Sem fornecedor"}
                </span>
              </div>
            `;
          }).join("")
        : `<div class="empty">Todos os produtos já possuem pedidos.</div>`;

      const birthdays = db.clients.filter(function(client) {
        return client.birth && client.birth.slice(5) === today().slice(5);
      });

      let alerts = "";

      if (birthdays.length) {
        alerts += `
          <div class="alert">
            Aniversariantes de hoje:
            ${birthdays.map(function(client) {
              return escapeHTML(client.name);
            }).join(", ")}
          </div>
        `;
      }

      if (inactive.length) {
        alerts += `
          <div class="alert danger-alert">
            ${inactive.length} cliente(s) precisam de acompanhamento por inatividade.
          </div>
        `;
      }

      document.getElementById("dashboardAlerts").innerHTML = alerts;
    }

    document.getElementById("clientForm").addEventListener("submit", function(event) {
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

      const clients = db.clients.filter(function(client) {
        return client.name.toLowerCase().includes(search) ||
          (client.phone || "").toLowerCase().includes(search);
      });

      document.getElementById("clientsTable").innerHTML = clients.length
        ? clients.map(function(client) {
            const stats = getClientStats(client.id);
            const status = clientStatus(client);

            return `
              <tr
                class="clickable"
                onclick="openClientProfile('${client.id}')">

                <td>
                  <strong>${escapeHTML(client.name)}</strong>
                  <br>
                  <span class="muted">${escapeHTML(client.city || "")}</span>
                </td>

                <td>
                  ${escapeHTML(client.phone || "—")}
                  <br>
                  <span class="muted">${escapeHTML(client.email || "")}</span>
                </td>

                <td>${dateBR(stats.lastSale)}</td>

                <td>
                  <span class="badge ${status === "Ativo" ? "badge-c" : "badge-a"}">
                    ${status}
                  </span>
                </td>

                <td>${stats.sales.length}</td>

                <td>
                  <button
                    class="btn btn-small"
                    onclick="event.stopPropagation();openClientProfile('${client.id}')">
                    Abrir perfil
                  </button>

                  <button
                    class="btn btn-small btn-danger"
                    onclick="event.stopPropagation();deleteClient('${client.id}')">
                    Excluir
                  </button>
                </td>
              </tr>
            `;
          }).join("")
        : `
          <tr>
            <td colspan="6" class="empty">Nenhum cliente cadastrado.</td>
          </tr>
        `;
    }

    function deleteClient(id) {
      const client = getClient(id);

      if (!client) return;

      if (!confirm("Excluir o cliente " + client.name + "? As vendas também serão removidas.")) {
        return;
      }

      db.clients = db.clients.filter(function(item) {
        return item.id !== id;
      });

      db.sales = db.sales.filter(function(sale) {
        return sale.clientId !== id;
      });

      db.attachments = db.attachments.filter(function(file) {
        return file.clientId !== id;
      });

      db.lowerReasons = db.lowerReasons.filter(function(reason) {
        return reason.clientId !== id;
      });

      saveDB();
      renderAll();
    }

    document.getElementById("supplierForm").addEventListener("submit", function(event) {
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
        ? db.suppliers.map(function(supplier) {
            const products = db.products.filter(function(product) {
              return product.supplierId === supplier.id;
            });

            return `
              <tr>
                <td>
                  <span class="dot" style="background:${supplier.color}"></span>
                  <strong>${escapeHTML(supplier.name)}</strong>
                </td>

                <td>${escapeHTML(supplier.contact || "—")}</td>

                <td>
                  <span class="supplier-chip">
                    <span class="dot" style="background:${supplier.color}"></span>
                    ${supplier.color}
                  </span>
                </td>

                <td>${products.length}</td>

                <td>
                  <button
                    class="btn btn-small btn-danger"
                    onclick="deleteSupplier('${supplier.id}')">
                    Excluir
                  </button>
                </td>
              </tr>
            `;
          }).join("")
        : `
          <tr>
            <td colspan="5" class="empty">Nenhum fornecedor cadastrado.</td>
          </tr>
        `;
    }

    function deleteSupplier(id) {
      const hasProducts = db.products.some(function(product) {
        return product.supplierId === id;
      });

      if (hasProducts) {
        alert("Não é possível excluir um fornecedor que possui produtos vinculados.");
        return;
      }

      db.suppliers = db.suppliers.filter(function(supplier) {
        return supplier.id !== id;
      });

      saveDB();
      renderAll();
    }

    document.getElementById("productForm").addEventListener("submit", function(event) {
      event.preventDefault();

      const code = "P" + String(db.products.length + 1).padStart(4, "0");

      db.products.push({
        id: uid("prod"),
        code: code,
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

      const products = db.products.filter(function(product) {
        return product.name.toLowerCase().includes(search) ||
          product.code.toLowerCase().includes(search);
      });

      document.getElementById("productsTable").innerHTML = products.length
        ? products.map(function(product) {
            const supplier = getSupplier(product.supplierId);
            const quantity = getProductQuantity(product.id);

            return `
              <tr>
                <td>${escapeHTML(product.code)}</td>

                <td>
                  <strong>${escapeHTML(product.name)}</strong>
                </td>

                <td>
                  ${supplier ? supplierChip(supplier, true) : "—"}
                </td>

                <td>${escapeHTML(product.category || "—")}</td>

                <td>${money(product.price)}</td>

                <td>${quantity}</td>

                <td>
                  <button
                    class="btn btn-small btn-danger"
                    onclick="deleteProduct('${product.id}')">
                    Excluir
                  </button>
                </td>
              </tr>
            `;
          }).join("")
        : `
          <tr>
            <td colspan="7" class="empty">Nenhum produto cadastrado.</td>
          </tr>
        `;
    }

    function deleteProduct(id) {
      const hasSales = db.sales.some(function(sale) {
        return (sale.items || []).some(function(item) {
          return item.productId === id;
        });
      });

      if (hasSales) {
        alert("Este produto possui histórico de vendas e não pode ser excluído.");
        return;
      }

      db.products = db.products.filter(function(product) {
        return product.id !== id;
      });

      saveDB();
      renderAll();
    }

    function updateSelects() {
      const productSupplier = document.getElementById("productSupplier");
      const oldSupplier = productSupplier.value;

      productSupplier.innerHTML =
        `<option value="">Selecione...</option>` +
        db.suppliers.map(function(supplier) {
          return `
            <option value="${supplier.id}">
              ${escapeHTML(supplier.name)}
            </option>
          `;
        }).join("");

      if (oldSupplier) {
        productSupplier.value = oldSupplier;
      }

      const saleClient = document.getElementById("saleClient");
      const oldClient = saleClient.value;

      saleClient.innerHTML =
        `<option value="">Selecione...</option>` +
        db.clients.map(function(client) {
          return `
            <option value="${client.id}">
              ${escapeHTML(client.name)}
            </option>
          `;
        }).join("");

      if (oldClient) {
        saleClient.value = oldClient;
      }
    }

    function openSaleModal(clientId) {
      updateSelects();

      document.getElementById("saleDate").value = today();
      document.getElementById("saleClient").value = clientId || "";
      document.getElementById("saleSeller").value = "";
      document.getElementById("saleNotes").value = "";
      document.getElementById("saleLines").innerHTML = "";

      addSaleLine();

      document.getElementById("saleModal").classList.add("show");
    }

    function addSaleLine(productId, quantity) {
      const line = document.createElement("div");

      line.className = "product-line";

      line.innerHTML = `
        <div class="field">
          <label>Produto</label>

          <select class="sale-product" onchange="updateSaleTotal()">
            <option value="">Selecione...</option>

            ${db.products.map(function(product) {
              return `
                <option
                  value="${product.id}"
                  ${product.id === productId ? "selected" : ""}>
                  ${escapeHTML(product.code)} -
                  ${escapeHTML(product.name)}
                  (${money(product.price)})
                </option>
              `;
            }).join("")}
          </select>
        </div>

        <div class="field">
          <label>Quantidade</label>

          <input
            class="sale-quantity"
            type="number"
            min="1"
            value="${quantity || 1}"
            oninput="updateSaleTotal()">
        </div>

        <div class="mini-total">R$ 0,00</div>

        <button
          type="button"
          class="btn btn-small btn-danger"
          onclick="this.parentElement.remove();updateSaleTotal()">
          ×
        </button>
      `;

      document.getElementById("saleLines").appendChild(line);
      updateSaleTotal();
    }

    function updateSaleTotal() {
      let total = 0;

      document.querySelectorAll(".product-line").forEach(function(line) {
        const productId = line.querySelector(".sale-product")?.value;
        const product = getProduct(productId);
        const quantity = Number(line.querySelector(".sale-quantity")?.value || 0);
        const lineTotal = product ? product.price * quantity : 0;

        total += lineTotal;

        const display = line.querySelector(".mini-total");

        if (display) {
          display.textContent = money(lineTotal);
        }
      });

      document.getElementById("saleTotal").textContent = money(total);
    }

    document.getElementById("saleForm").addEventListener("submit", function(event) {
      event.preventDefault();

      const clientId = document.getElementById("saleClient").value;
      const items = [];

      document.querySelectorAll(".product-line").forEach(function(line) {
        const productId = line.querySelector(".sale-product").value;
        const quantity = Number(line.querySelector(".sale-quantity").value || 0);
        const product = getProduct(productId);

        if (product && quantity > 0) {
          items.push({
            productId: productId,
            quantity: quantity,
            price: product.price,
            guarantee: false
          });
        }
      });

      if (!clientId) {
        alert("Selecione um cliente.");
        return;
      }

      if (!items.length) {
        alert("Adicione pelo menos um produto.");
        return;
      }

      db.sales.push({
        id: uid("sale"),
        clientId: clientId,
        date: document.getElementById("saleDate").value,
        seller: document.getElementById("saleSeller").value.trim(),
        channel: document.getElementById("saleChannel").value,
        notes: document.getElementById("saleNotes").value.trim(),
        items: items
      });

      saveDB();
      closeModal("saleModal");
      renderAll();

      alert("Venda registrada com sucesso.");
    });

    function getFilteredSales() {
      const period = document.getElementById("abcPeriod")?.value || "all";

      if (period === "all") {
        return db.sales;
      }

      const limit = new Date();
      limit.setDate(limit.getDate() - Number(period));

      return db.sales.filter(function(sale) {
        return new Date(sale.date + "T12:00:00") >= limit;
      });
    }

    function getABCClassByAccumulated(rows, index) {
      if (!rows.length) {
        return "C";
      }

      const total = rows.reduce(function(sum, row) {
        return sum + Number(row.revenue || 0);
      }, 0);

      if (total <= 0) {
        if (index === 0) return "A";
        if (index === 1) return "B";
        return "C";
      }

      const accumulated = rows
        .slice(0, index + 1)
        .reduce(function(sum, row) {
          return sum + Number(row.revenue || 0);
        }, 0);

      const percentage = accumulated / total * 100;

      if (percentage <= 80) return "A";
      if (percentage <= 95) return "B";

      return "C";
    }

    function getProductABCClass(productId, salesList) {
      const rows = db.products.map(function(product) {
        return {
          id: product.id,
          revenue: getProductRevenue(product.id, salesList)
        };
      }).sort(function(a, b) {
        return b.revenue - a.revenue;
      });

      const index = rows.findIndex(function(row) {
        return row.id === productId;
      });

      if (index < 0) {
        return "C";
      }

      return getABCClassByAccumulated(rows, index);
    }

    function getProductSuggestions(clientId, salesList) {
      const stats = getClientStats(clientId, salesList || db.sales);
      const purchasedIds = Object.keys(stats.quantities);
      const sourceSales = salesList || db.sales;

      const rows = db.products
        .filter(function(product) {
          return !purchasedIds.includes(product.id);
        })
        .map(function(product) {
          const supplier = getSupplier(product.supplierId);

          return {
            product: product,
            supplier: supplier,
            abc: getProductABCClass(product.id, sourceSales),
            revenue: getProductRevenue(product.id, sourceSales),
            quantity: getProductQuantity(product.id, sourceSales)
          };
        })
        .sort(function(a, b) {
          const order = {
            A: 1,
            B: 2,
            C: 3
          };

          if (order[a.abc] !== order[b.abc]) {
            return order[a.abc] - order[b.abc];
          }

          return b.revenue - a.revenue;
        });

      return rows;
    }

    function getLowerPurchases(clientId) {
      const clientStats = getClientStats(clientId);
      const result = [];

      db.products.forEach(function(product) {
        const clientQuantity = Number(clientStats.quantities[product.id] || 0);

        if (clientQuantity <= 0) {
          return;
        }

        let total = 0;
        let buyers = 0;

        db.clients.forEach(function(otherClient) {
          const stats = getClientStats(otherClient.id);
          const quantity = Number(stats.quantities[product.id] || 0);

          if (quantity > 0) {
            total += quantity;
            buyers++;
          }
        });

        if (!buyers) {
          return;
        }

        const average = total / buyers;

        if (clientQuantity < average) {
          const savedReason = db.lowerReasons.find(function(reason) {
            return reason.clientId === clientId &&
              reason.productId === product.id;
          });

          result.push({
            product: product,
            clientQuantity: clientQuantity,
            average: average,
            reason: savedReason ? savedReason.reason : ""
          });
        }
      });

      return result.sort(function(a, b) {
        return (b.average - b.clientQuantity) - (a.average - a.clientQuantity);
      });
    }

    function renderABC() {
      const sales = getFilteredSales();

      const rows = db.clients.map(function(client) {
        const stats = getClientStats(client.id, sales);
        const supplierIds = [];
        const productIds = [];

        stats.sales.forEach(function(sale) {
          (sale.items || []).forEach(function(item) {
            const product = getProduct(item.productId);

            if (!product) return;

            if (!supplierIds.includes(product.supplierId)) {
              supplierIds.push(product.supplierId);
            }

            if (!productIds.includes(product.id)) {
              productIds.push(product.id);
            }
          });
        });

        return {
          client: client,
          revenue: stats.revenue,
          stats: stats,
          supplierIds: supplierIds,
          productIds: productIds
        };
      }).sort(function(a, b) {
        return b.revenue - a.revenue;
      });

      const totalRevenue = rows.reduce(function(sum, row) {
        return sum + row.revenue;
      }, 0);

      document.getElementById("abcTable").innerHTML = rows.length
        ? rows.map(function(row, index) {
            const abc = getABCClassByAccumulated(rows, index);
            const participation = totalRevenue > 0
              ? row.revenue / totalRevenue * 100
              : 0;

            const suggestions = getProductSuggestions(row.client.id, sales)
              .slice(0, 3);

            const suppliersHtml = db.suppliers.length
              ? db.suppliers.map(function(supplier) {
                  return supplierChip(
                    supplier,
                    row.supplierIds.includes(supplier.id)
                  );
                }).join("")
              : "Nenhum fornecedor cadastrado";

            const productsHtml = row.productIds.length
              ? row.productIds.map(function(productId) {
                  const product = getProduct(productId);

                  return product
                    ? `
                      <span class="badge badge-c">
                        ${escapeHTML(product.name)}
                      </span>
                    `
                    : "";
                }).join(" ")
              : `<span class="muted">Nenhum produto</span>`;

            const suggestionsHtml = suggestions.length
              ? `
                <div class="list suggestion-box">
                  ${suggestions.map(function(item) {
                    return `
                      <div class="list-item">
                        <strong>${escapeHTML(item.product.name)}</strong>
                        <span class="muted">
                          ${abcBadge(item.abc)}
                          ${item.supplier ? " · " + escapeHTML(item.supplier.name) : ""}
                        </span>
                      </div>
                    `;
                  }).join("")}
                </div>
              `
              : `<span class="muted">Sem sugestões</span>`;

            return `
              <tr
                class="clickable"
                onclick="openClientProfile('${row.client.id}')">

                <td>
                  <strong>${escapeHTML(row.client.name)}</strong>
                  <br>
                  <span class="muted">Clique para abrir o cliente</span>
                </td>

                <td>${abcBadge(abc)}</td>

                <td>
                  <div class="supplier-list">
                    ${suppliersHtml}
                  </div>
                </td>

                <td>
                  <div class="supplier-list">
                    ${productsHtml}
                  </div>
                </td>

                <td>${row.stats.sales.length}</td>
                <td>${row.stats.items}</td>

                <td class="green">${money(row.revenue)}</td>

                <td>
                  ${participation.toFixed(2)}%
                  <br>
                  <span class="muted">da base</span>
                </td>

                <td>${dateBR(row.stats.lastSale)}</td>

                <td>
                  <button
                    class="btn btn-small btn-primary"
                    onclick="event.stopPropagation();openClientProfile('${row.client.id}')">
                    Ver cliente
                  </button>

                  <div style="margin-top:8px">
                    <strong style="font-size:11px">Sugestões:</strong>
                    ${suggestionsHtml}
                  </div>
                </td>
              </tr>
            `;
          }).join("")
        : `
          <tr>
            <td colspan="10" class="empty">
              Cadastre clientes e vendas para visualizar a Curva ABC.
            </td>
          </tr>
        `;

      renderABCProducts(sales);
    }

    function renderABCProducts(sales) {
      const rows = db.products.map(function(product) {
        const quantity = getProductQuantity(product.id, sales);
        const revenue = getProductRevenue(product.id, sales);
        const clients = [];

        sales.forEach(function(sale) {
          const hasProduct = (sale.items || []).some(function(item) {
            return item.productId === product.id;
          });

          if (hasProduct && !clients.includes(sale.clientId)) {
            clients.push(sale.clientId);
          }
        });

        return {
          product: product,
          quantity: quantity,
          revenue: revenue,
          clients: clients
        };
      }).sort(function(a, b) {
        return b.revenue - a.revenue;
      });

      document.getElementById("abcProductsTable").innerHTML = rows.length
        ? rows.map(function(row) {
            const supplier = getSupplier(row.product.supplierId);
            const abc = getProductABCClass(row.product.id, sales);

            return `
              <tr>
                <td>
                  <strong>${escapeHTML(row.product.name)}</strong>
                  <br>
                  <span class="muted">${escapeHTML(row.product.code)}</span>
                </td>

                <td>${supplier ? supplierChip(supplier, true) : "—"}</td>
                <td>${abcBadge(abc)}</td>
                <td>${row.quantity}</td>
                <td class="green">${money(row.revenue)}</td>
                <td>${row.clients.length}</td>
              </tr>
            `;
          }).join("")
        : `
          <tr>
            <td colspan="6" class="empty">Nenhum produto cadastrado.</td>
          </tr>
        `;
    }

    function openClientProfile(clientId) {
      const client = getClient(clientId);

      if (!client) return;

      const stats = getClientStats(clientId);
      const boughtProductIds = Object.keys(stats.quantities);
      const boughtSupplierIds = [];

      boughtProductIds.forEach(function(productId) {
        const product = getProduct(productId);

        if (product && !boughtSupplierIds.includes(product.supplierId)) {
          boughtSupplierIds.push(product.supplierId);
        }
      });

      const suggestions = getProductSuggestions(clientId);
      const lowerPurchases = getLowerPurchases(clientId);

      const ordersHtml = stats.sales.length
        ? stats.sales
            .slice()
            .sort(function(a, b) {
              return b.date.localeCompare(a.date);
            })
            .map(function(sale) {
              return `
                <div class="list-item">
                  <strong>
                    Pedido de ${dateBR(sale.date)} —
                    ${money(getSaleTotal(sale))}
                  </strong>

                  <div class="muted">
                    ${(sale.items || []).length} produto(s) ·
                    ${escapeHTML(sale.channel || "Canal não informado")} ·
                    ${escapeHTML(sale.seller || "Vendedor não informado")}
                  </div>

                  <div class="form-actions">
                    <button
                      class="btn btn-small"
                      onclick="openOrder('${sale.id}')">
                      Ver pedido
                    </button>

                    <button
                      class="btn btn-small btn-primary"
                      onclick="downloadOrderPDF('${sale.id}')">
                      Baixar PDF
                    </button>
                  </div>
                </div>
              `;
            }).join("")
        : `<div class="empty">Este cliente ainda não possui pedidos.</div>`;

      const suggestionsHtml = suggestions.length
        ? suggestions.slice(0, 15).map(function(item) {
            return `
              <div class="list-item">
                <strong>${escapeHTML(item.product.name)}</strong>

                <div class="muted">
                  ${abcBadge(item.abc)}
                  · ${item.quantity} unidade(s) vendida(s) na base
                  · ${money(item.revenue)} em faturamento
                  ${item.supplier ? " · " + escapeHTML(item.supplier.name) : ""}
                </div>
              </div>
            `;
          }).join("")
        : `<div class="empty">Não há sugestões disponíveis.</div>`;

      const lowerHtml = lowerPurchases.length
        ? lowerPurchases.map(function(item) {
            return `
              <div class="list-item">
                <strong>${escapeHTML(item.product.name)}</strong>

                <div class="muted">
                  Cliente comprou: <strong>${item.clientQuantity}</strong>
                  · Média dos compradores:
                  <strong>${item.average.toFixed(1)}</strong>
                </div>

                <div class="field" style="margin-top:10px">
                  <label>Motivo da compra menor</label>

                  <input
                    value="${escapeHTML(item.reason)}"
                    placeholder="Ex.: preço, baixa procura, preferência..."
                    onchange="saveLowerReason('${client.id}','${item.product.id}',this.value)">
                </div>
              </div>
            `;
          }).join("")
        : `<div class="empty">Nenhum produto abaixo da média identificado.</div>`;

      document.getElementById("clientProfile").innerHTML = `
        <div class="profile-header">
          <div>
            <button
              class="btn btn-small"
              onclick="showPage('clientes');renderAll()">
              ← Voltar
            </button>

            <h2 style="margin-top:15px">${escapeHTML(client.name)}</h2>

            <div class="muted">
              ${escapeHTML(client.phone || "Sem telefone")} ·
              ${escapeHTML(client.email || "Sem e-mail")} ·
              ${escapeHTML(client.city || "Sem cidade")}
            </div>
          </div>

          <div class="form-actions" style="margin-top:0">
            <button
              class="btn btn-primary"
              onclick="openSaleModal('${client.id}')">
              + Nova venda
            </button>

            <button
              class="btn"
              onclick="document.getElementById('attachmentInput').click()">
              Anexar arquivo
            </button>

            <input
              id="attachmentInput"
              type="file"
              hidden
              onchange="saveAttachment('${client.id}', this.files[0])">
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
            <div class="metric-value" style="font-size:18px">
              ${clientStatus(client)}
            </div>
          </div>
        </div>

        <div class="profile-layout">
          <div>
            <div class="panel">
              <h2>Fornecedores comprados pelo cliente</h2>

              <div class="supplier-list">
                ${
                  db.suppliers.length
                    ? db.suppliers.map(function(supplier) {
                        return supplierChip(
                          supplier,
                          boughtSupplierIds.includes(supplier.id)
                        );
                      }).join("")
                    : `<span class="muted">Nenhum fornecedor cadastrado.</span>`
                }
              </div>

              <div class="muted" style="margin-top:12px">
                <span class="dot" style="background:#555"></span>
                Cinza: ainda não comprou
                &nbsp;&nbsp;
                <span class="dot" style="background:var(--red)"></span>
                Cor cadastrada: já comprou
              </div>
            </div>

            <div class="panel" style="margin-top:15px">
              <h2>Pedidos do cliente</h2>
              <div class="list">${ordersHtml}</div>
            </div>

            <div class="panel" style="margin-top:15px">
              <h2>Anexos do cliente</h2>
              ${renderAttachments(client.id)}
            </div>
          </div>

          <div>
            <div class="panel">
              <h2>Sugestões de produtos</h2>

              <div class="muted" style="margin-bottom:12px">
                Produtos que o cliente ainda não comprou, priorizados pela Curva ABC geral.
              </div>

              <div class="list">
                ${suggestionsHtml}
              </div>
            </div>

            <div class="panel" style="margin-top:15px">
              <h2>Produtos comprados em menor quantidade</h2>

              <div class="muted" style="margin-bottom:12px">
                Compare a quantidade comprada pelo cliente com a média dos clientes que compraram o mesmo produto.
              </div>

              <div class="list">
                ${lowerHtml}
              </div>
            </div>
          </div>
        </div>
      `;

      showPage("profile");
    }

    function saveLowerReason(clientId, productId, reason) {
      const existing = db.lowerReasons.find(function(item) {
        return item.clientId === clientId &&
          item.productId === productId;
      });

      if (existing) {
        existing.reason = reason;
      } else {
        db.lowerReasons.push({
          id: uid("reason"),
          clientId: clientId,
          productId: productId,
          reason: reason
        });
      }

      saveDB();
    }

    function saveAttachment(clientId, file) {
      if (!file) return;

      const reader = new FileReader();

      reader.onload = function() {
        db.attachments.push({
          id: uid("file"),
          clientId: clientId,
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
      const attachments = db.attachments.filter(function(file) {
        return file.clientId === clientId;
      });

      if (!attachments.length) {
        return `<div class="empty">Nenhum arquivo anexado.</div>`;
      }

      return `
        <div class="list">
          ${attachments.map(function(file) {
            return `
              <div class="list-item">
                <strong>${escapeHTML(file.name)}</strong>

                <div class="muted">
                  ${dateBR(file.date)} · ${formatBytes(file.size)}
                </div>

                <div class="form-actions">
                  <a
                    class="btn btn-small"
                    href="${file.data}"
                    download="${escapeHTML(file.name)}">
                    Baixar
                  </a>

                  ${
                    file.type && file.type.startsWith("image/")
                      ? `
                        <img
                          class="image-preview"
                          src="${file.data}"
                          alt="Pré-visualização">
                      `
                      : ""
                  }

                  <button
                    class="btn btn-small btn-danger"
                    onclick="deleteAttachment('${file.id}','${clientId}')">
                    Excluir
                  </button>
                </div>
              </div>
            `;
          }).join("")}
        </div>
      `;
    }

    function formatBytes(bytes) {
      if (!bytes) return "0 B";

      const units = ["B", "KB", "MB", "GB"];
      const index = Math.floor(Math.log(bytes) / Math.log(1024));

      return (bytes / Math.pow(1024, index)).toFixed(1) + " " + units[index];
    }

    function deleteAttachment(fileId, clientId) {
      if (!confirm("Excluir este anexo?")) {
        return;
      }

      db.attachments = db.attachments.filter(function(file) {
        return file.id !== fileId;
      });

      saveDB();
      openClientProfile(clientId);
    }

    function openOrder(saleId) {
      const sale = db.sales.find(function(item) {
        return item.id === saleId;
      });

      if (!sale) return;

      const client = getClient(sale.clientId);

      const itemsHtml = (sale.items || []).map(function(item) {
        const product = getProduct(item.productId);
        const supplier = product ? getSupplier(product.supplierId) : null;

        return `
          <tr>
            <td>${escapeHTML(product?.name || "Produto removido")}</td>
            <td>${supplier ? supplierChip(supplier, true) : "—"}</td>
            <td>${item.quantity}</td>
            <td>${money(item.price)}</td>
            <td class="green">${money(item.quantity * item.price)}</td>
          </tr>
        `;
      }).join("");

      document.getElementById("orderDetails").innerHTML = `
        <div class="card" style="margin-bottom:14px">
          <strong>${escapeHTML(client?.name || "Cliente removido")}</strong>

          <div class="muted">
            ${escapeHTML(client?.phone || "")} ·
            ${escapeHTML(client?.email || "")}
          </div>

          <div class="muted" style="margin-top:7px">
            Data: ${dateBR(sale.date)} ·
            Vendedor: ${escapeHTML(sale.seller || "—")} ·
            Canal: ${escapeHTML(sale.channel || "—")}
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

            <tbody>${itemsHtml}</tbody>
          </table>
        </div>

        <div style="margin-top:18px;text-align:right;font-size:20px">
          Total:
          <strong class="green">${money(getSaleTotal(sale))}</strong>
        </div>

        ${
          sale.notes
            ? `
              <div class="card" style="margin-top:15px">
                <strong>Observações</strong>
                <div class="muted" style="margin-top:7px">
                  ${escapeHTML(sale.notes)}
                </div>
              </div>
            `
            : ""
        }

        <div class="form-actions">
          <button
            class="btn btn-primary"
            onclick="downloadOrderPDF('${sale.id}')">
            Baixar pedido em PDF
          </button>

          <button
            class="btn"
            onclick="closeModal('orderModal')">
            Fechar
          </button>
        </div>
      `;

      document.getElementById("orderModal").classList.add("show");
    }

    function downloadOrderPDF(saleId) {
      const sale = db.sales.find(function(item) {
        return item.id === saleId;
      });

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

      doc.text("Cliente: " + (client?.name || "—"), 15, y);
      y += 6;

      doc.text("Telefone: " + (client?.phone || "—"), 15, y);
      y += 6;

      doc.text("E-mail: " + (client?.email || "—"), 15, y);
      y += 6;

      doc.text("Data: " + dateBR(sale.date), 15, y);
      y += 6;

      doc.text(
        "Vendedor: " + (sale.seller || "—") +
        " | Canal: " + (sale.channel || "—"),
        15,
        y
      );

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

      sale.items.forEach(function(item) {
        const product = getProduct(item.productId);
        const productName = product?.name || "Produto removido";
        const lineTotal = item.quantity * item.price;

        doc.text(productName.substring(0, 48), 18, y);
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
      doc.text("TOTAL: " + money(getSaleTotal(sale)), 145, y);

      if (sale.notes) {
        y += 12;
        doc.setFontSize(10);
        doc.text("Observações:", 15, y);
        y += 6;

        const notes = doc.splitTextToSize(sale.notes, 175);
        doc.text(notes, 15, y);
      }

      const safeName = (client?.name || "cliente")
        .replace(/[^a-z0-9]/gi, "-")
        .toLowerCase();

      doc.save("pedido-" + safeName + "-" + sale.date + ".pdf");
    }

    function closeModal(id) {
      document.getElementById(id).classList.remove("show");
    }

    document.querySelectorAll(".modal").forEach(function(modal) {
      modal.addEventListener("click", function(event) {
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
