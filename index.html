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
      --black-2: #111111;
      --black-3: #1c1c1c;
      --border: #383838;
      --white: #ffffff;
      --gray: #a8a8a8;
      --red: #e50914;
      --green: #20c77a;
      --yellow: #f4c542;
      --blue: #4298ed;
      --purple: #ae7aff;
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
    }

    .sidebar {
      position: fixed;
      top: 0;
      left: 0;
      bottom: 0;
      z-index: 20;
      width: 240px;
      padding: 20px 12px;
      overflow-y: auto;
      background: #050505;
      border-right: 1px solid var(--border);
    }

    .brand {
      margin: 0 10px 24px;
      color: var(--red);
      font-size: 22px;
      font-weight: bold;
      letter-spacing: .5px;
    }

    .brand small {
      display: block;
      margin-top: 4px;
      color: var(--gray);
      font-size: 10px;
      font-weight: normal;
      letter-spacing: 1px;
    }

    .menu-button {
      display: flex;
      align-items: center;
      gap: 9px;
      width: 100%;
      margin: 4px 0;
      padding: 12px;
      border: 0;
      border-radius: 6px;
      background: transparent;
      color: #bdbdbd;
      text-align: left;
    }

    .menu-button:hover,
    .menu-button.active {
      background: var(--red);
      color: white;
    }

    .content {
      width: calc(100% - 240px);
      min-height: 100vh;
      margin-left: 240px;
      padding: 24px;
    }

    .topbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 15px;
      margin-bottom: 22px;
    }

    h1,
    h2,
    h3 {
      margin-top: 0;
    }

    h1 {
      margin-bottom: 5px;
      font-size: 27px;
    }

    h2 {
      margin-bottom: 16px;
      font-size: 20px;
    }

    h3 {
      margin-bottom: 10px;
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
      background: var(--black-2);
      border: 1px solid var(--border);
      border-radius: 8px;
    }

    .panel {
      margin-bottom: 15px;
      padding: 17px;
    }

    .card {
      padding: 16px;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 14px;
      margin-bottom: 15px;
    }

    .grid-2,
    .grid-3,
    .grid-4 {
      display: grid;
      gap: 12px;
    }

    .grid-2 {
      grid-template-columns: repeat(2, 1fr);
    }

    .grid-3 {
      grid-template-columns: repeat(3, 1fr);
    }

    .grid-4 {
      grid-template-columns: repeat(4, 1fr);
    }

    .field {
      display: flex;
      flex-direction: column;
      gap: 6px;
    }

    .full {
      grid-column: 1 / -1;
    }

    label {
      color: #d7d7d7;
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
      background: #090909;
      color: white;
    }

    input:focus,
    select:focus,
    textarea:focus {
      border-color: var(--red);
    }

    textarea {
      min-height: 85px;
      resize: vertical;
    }

    input[type="color"] {
      height: 40px;
      padding: 3px;
    }

    .actions,
    .toolbar {
      display: flex;
      align-items: center;
      flex-wrap: wrap;
      gap: 9px;
    }

    .actions {
      margin-top: 14px;
    }

    .toolbar {
      justify-content: space-between;
      margin-bottom: 14px;
    }

    .button {
      padding: 9px 13px;
      border: 1px solid var(--border);
      border-radius: 5px;
      background: var(--black-3);
      color: white;
    }

    .button:hover {
      filter: brightness(1.25);
    }

    .button.primary {
      border-color: var(--red);
      background: var(--red);
    }

    .button.success {
      border-color: #14764f;
      background: #075b3c;
    }

    .button.danger {
      border-color: #87151c;
      background: #4a0b0f;
    }

    .button.small {
      padding: 6px 9px;
      font-size: 12px;
    }

    .metric-label {
      color: var(--gray);
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: .5px;
    }

    .metric-value {
      margin-top: 9px;
      font-size: 24px;
      font-weight: bold;
    }

    .green {
      color: var(--green);
    }

    .red {
      color: var(--red);
    }

    .yellow {
      color: var(--yellow);
    }

    .blue {
      color: var(--blue);
    }

    .purple {
      color: var(--purple);
    }

    .table-wrap {
      overflow-x: auto;
    }

    table {
      width: 100%;
      min-width: 800px;
      border-collapse: collapse;
    }

    th,
    td {
      padding: 10px 8px;
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
      background: #252525;
    }

    .list {
      display: flex;
      flex-direction: column;
      gap: 8px;
    }

    .list-item {
      padding: 10px;
      border: 1px solid var(--border);
      border-radius: 6px;
      background: #101010;
    }

    .list-item strong {
      display: block;
      margin-bottom: 5px;
    }

    .empty {
      padding: 20px 10px;
      color: var(--gray);
      text-align: center;
      font-size: 13px;
    }

    .alert {
      margin-bottom: 14px;
      padding: 12px;
      border-left: 4px solid var(--yellow);
      border-radius: 5px;
      background: #2a2208;
      color: #f4d97b;
      font-size: 13px;
    }

    .alert.red-alert {
      border-left-color: var(--red);
      background: #2b0a0d;
      color: #ffadb3;
    }

    .progress {
      height: 12px;
      overflow: hidden;
      border-radius: 20px;
      background: #292929;
    }

    .progress-bar {
      height: 100%;
      border-radius: 20px;
      background: linear-gradient(90deg, var(--red), #ff5560);
    }

    .badge {
      display: inline-flex;
      padding: 4px 8px;
      border-radius: 20px;
      font-size: 11px;
      white-space: nowrap;
    }

    .badge-a {
      background: #681019;
      color: #ff9ca3;
    }

    .badge-b {
      background: #65520a;
      color: #ffe36b;
    }

    .badge-c {
      background: #10496f;
      color: #85c9ff;
    }

    .badge-active {
      background: #075a3b;
      color: #7df1bd;
    }

    .badge-inactive {
      background: #571017;
      color: #ff979e;
    }

    .chip {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      padding: 5px 8px;
      border-radius: 18px;
      background: #292929;
      font-size: 11px;
    }

    .dot {
      width: 9px;
      height: 9px;
      border-radius: 50%;
    }

    .filter-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 10px;
      margin-bottom: 10px;
    }

    .comparison-card {
      border-left: 4px solid var(--blue);
    }

    .comparison-card.main-period {
      border-left-color: var(--green);
    }

    .comparison-box {
      margin-top: 10px;
      padding: 12px;
      border: 1px solid var(--border);
      border-radius: 7px;
      background: #151515;
    }

    .sale-row {
      display: grid;
      grid-template-columns: 180px 1fr 90px 115px 38px;
      align-items: end;
      gap: 8px;
      margin-bottom: 9px;
    }

    .line-total {
      padding-bottom: 10px;
      color: var(--green);
      font-size: 13px;
      font-weight: bold;
    }

    .modal {
      position: fixed;
      inset: 0;
      z-index: 100;
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      background: rgba(0, 0, 0, .8);
    }

    .modal.open {
      display: flex;
    }

    .modal-box {
      width: min(1050px, 100%);
      max-height: 92vh;
      overflow-y: auto;
      padding: 20px;
      border: 1px solid #444;
      border-top: 3px solid var(--red);
      border-radius: 8px;
      background: var(--black-2);
    }

    .modal-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 16px;
    }

    .close {
      border: 0;
      background: transparent;
      color: #aaa;
      font-size: 25px;
    }

    .profile-header {
      display: flex;
      align-items: flex-start;
      justify-content: space-between;
      gap: 15px;
      margin-bottom: 17px;
    }

    .profile-grid {
      display: grid;
      grid-template-columns: 1.1fr .9fr;
      gap: 15px;
    }

    .abc-a {
      border-left: 5px solid var(--red);
      background: rgba(229, 9, 20, .12);
    }

    .abc-b {
      border-left: 5px solid var(--yellow);
      background: rgba(244, 197, 66, .11);
    }

    .abc-c {
      border-left: 5px solid var(--blue);
      background: rgba(66, 152, 237, .11);
    }

    @media (max-width: 1100px) {
      .cards {
        grid-template-columns: repeat(2, 1fr);
      }

      .grid-4 {
        grid-template-columns: repeat(2, 1fr);
      }

      .profile-grid {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 760px) {
      .sidebar {
        position: sticky;
        top: 0;
        left: auto;
        right: auto;
        bottom: auto;
        display: flex;
        width: 100%;
        padding: 8px;
        overflow-x: auto;
        border-right: 0;
        border-bottom: 1px solid var(--border);
      }

      .brand {
        display: none;
      }

      .menu-button {
        flex: 0 0 auto;
        width: auto;
        white-space: nowrap;
      }

      .content {
        width: 100%;
        margin-left: 0;
        padding: 15px;
      }

      .topbar {
        align-items: flex-start;
        flex-direction: column;
      }

      .grid-2,
      .grid-3,
      .grid-4,
      .filter-grid {
        grid-template-columns: 1fr;
      }

      .cards {
        grid-template-columns: 1fr 1fr;
        gap: 8px;
      }

      .sale-row {
        grid-template-columns: 1fr 1fr 45px;
      }

      .sale-row .supplier-field,
      .sale-row .product-field {
        grid-column: 1 / -1;
      }

      .profile-header {
        flex-direction: column;
      }
    }
  </style>
</head>

<body>
  <div class="app">
    <aside class="sidebar">
      <div class="brand">
        GESTÃO
        <small>REPRESENTAÇÃO COMERCIAL</small>
      </div>

      <button class="menu-button active" data-page="dashboard">
        Dashboard
      </button>

      <button class="menu-button" data-page="clientes">
        Clientes
      </button>

      <button class="menu-button" data-page="produtos">
        Produtos
      </button>

      <button class="menu-button" data-page="fornecedores">
        Fornecedores
      </button>

      <button class="menu-button" data-page="vendedores">
        Vendedores
      </button>

      <button class="menu-button" data-page="financeiro">
        Financeiro
      </button>

      <button class="menu-button" data-page="abc">
        Curva ABC
      </button>

      <button class="menu-button" data-page="configuracoes">
        Configurações
      </button>
    </aside>

    <main class="content">
      <header class="topbar">
        <div>
          <h1 id="page-title">Dashboard</h1>
          <div class="muted">Gestão comercial, vendas e análises</div>
        </div>

        <button class="button primary" onclick="openSaleModal()">
          + Nova venda
        </button>
      </header>

      <!-- DASHBOARD -->
      <section class="page active" id="page-dashboard">
        <div class="panel">
          <div class="toolbar">
            <div>
              <h2>Filtros da dashboard</h2>
              <div class="muted">
                Filtre o período e compare vários cenários.
              </div>
            </div>

            <div class="actions" style="margin-top:0">
              <button class="button small" onclick="addComparison()">
                + Adicionar comparação
              </button>

              <button class="button small danger" onclick="clearComparisons()">
                Limpar comparações
              </button>
            </div>
          </div>

          <div class="filter-grid">
            <div class="field">
              <label>Data inicial</label>
              <input id="filter-start" type="date" onchange="renderDashboard()">
            </div>

            <div class="field">
              <label>Data final</label>
              <input id="filter-end" type="date" onchange="renderDashboard()">
            </div>

            <div class="field">
              <label>Cliente</label>
              <select id="filter-client" onchange="renderDashboard()"></select>
            </div>

            <div class="field">
              <label>Vendedor</label>
              <select id="filter-seller" onchange="renderDashboard()"></select>
            </div>

            <div class="field">
              <label>Fornecedor</label>
              <select id="filter-supplier" onchange="renderDashboard()"></select>
            </div>

            <div class="field">
              <label>Produto</label>
              <select id="filter-product" onchange="renderDashboard()"></select>
            </div>

            <div class="field">
              <label>Canal</label>
              <select id="filter-channel" onchange="renderDashboard()">
                <option value="">Todos os canais</option>
                <option>Presencial</option>
                <option>WhatsApp</option>
                <option>Telefone</option>
                <option>Site</option>
                <option>Outro</option>
              </select>
            </div>

            <div class="field">
              <label>Atalho de período</label>
              <select id="filter-shortcut" onchange="applyShortcut()">
                <option value="">Selecionar</option>
                <option value="today">Hoje</option>
                <option value="7">Últimos 7 dias</option>
                <option value="30">Últimos 30 dias</option>
                <option value="90">Últimos 90 dias</option>
                <option value="month">Mês atual</option>
                <option value="previous-month">Mês anterior</option>
                <option value="year">Ano atual</option>
              </select>
            </div>
          </div>

          <div id="comparisons"></div>

          <div class="actions">
            <button class="button small" onclick="clearDashboardFilters()">
              Limpar filtros
            </button>

            <button class="button small primary" onclick="renderDashboard()">
              Atualizar análise
            </button>
          </div>
        </div>

        <div id="dashboard-alerts"></div>

        <div class="cards">
          <div class="card">
            <div class="metric-label">Faturamento filtrado</div>
            <div class="metric-value green" id="dash-revenue">R$ 0,00</div>
          </div>

          <div class="card">
            <div class="metric-label">Pedidos</div>
            <div class="metric-value" id="dash-orders">0</div>
          </div>

          <div class="card">
            <div class="metric-label">Clientes alcançados</div>
            <div class="metric-value blue" id="dash-clients">0</div>
          </div>

          <div class="card">
            <div class="metric-label">Ticket médio</div>
            <div class="metric-value yellow" id="dash-ticket">R$ 0,00</div>
          </div>
        </div>

        <div class="panel">
          <h2>Comparação dos períodos</h2>
          <div class="grid-3" id="comparison-results"></div>
        </div>

        <div class="panel">
          <div class="toolbar">
            <h2>Metas</h2>
            <button class="button small" onclick="openGoalModal()">
              Configurar meta
            </button>
          </div>

          <div class="cards">
            <div class="card">
              <div class="metric-label">Meta mensal</div>
              <div class="metric-value" id="goal-month">R$ 0,00</div>
            </div>

            <div class="card">
              <div class="metric-label">Meta diária</div>
              <div class="metric-value yellow" id="goal-day">R$ 0,00</div>
            </div>

            <div class="card">
              <div class="metric-label">Vendido no mês</div>
              <div class="metric-value green" id="goal-sold">R$ 0,00</div>
            </div>

            <div class="card">
              <div class="metric-label">Falta vender</div>
              <div class="metric-value red" id="goal-missing">R$ 0,00</div>
            </div>
          </div>

          <div class="progress">
            <div class="progress-bar" id="goal-progress"></div>
          </div>

          <div class="muted" id="goal-text" style="margin-top:8px"></div>
        </div>

        <div class="grid-2">
          <div class="panel">
            <h2>Aniversariantes</h2>
            <div id="birthdays"></div>
          </div>

          <div class="panel">
            <h2>Clientes inativos</h2>
            <div id="inactive-clients"></div>
          </div>
        </div>

        <div class="grid-2">
          <div class="panel">
            <h2>Oportunidades de expansão</h2>
            <div id="opportunities"></div>
          </div>

          <div class="panel">
            <h2>Produtos sem pedidos</h2>
            <div id="unused-products"></div>
          </div>
        </div>
      </section>

      <!-- CLIENTES -->
      <section class="page" id="page-clientes">
        <div class="panel">
          <h2>Cadastrar cliente</h2>

          <form id="client-form">
            <div class="grid-3">
              <div class="field">
                <label>Nome completo *</label>
                <input id="client-name" required>
              </div>

              <div class="field">
                <label>Telefone / WhatsApp</label>
                <input id="client-phone">
              </div>

              <div class="field">
                <label>E-mail</label>
                <input id="client-email" type="email">
              </div>

              <div class="field">
                <label>Data de nascimento</label>
                <input id="client-birth" type="date">
              </div>

              <div class="field">
                <label>CPF / CNPJ</label>
                <input id="client-document">
              </div>

              <div class="field">
                <label>Logo do cliente</label>
                <input id="client-logo" placeholder="URL da imagem">
              </div>

              <div class="field full">
                <label>Endereço</label>
                <input id="client-address">
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar cliente</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <div class="toolbar">
            <h2>Clientes cadastrados</h2>
            <input
              id="client-search"
              style="max-width:280px"
              placeholder="Buscar cliente..."
              oninput="renderClients()">
          </div>

          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Nome</th>
                  <th>Telefone</th>
                  <th>Última compra</th>
                  <th>Status</th>
                  <th>Pedidos</th>
                  <th>Faturamento</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="clients-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- PRODUTOS -->
      <section class="page" id="page-produtos">
        <div class="panel">
          <h2>Cadastrar produto</h2>

          <form id="product-form">
            <div class="grid-3">
              <div class="field">
                <label>SKU *</label>
                <input id="product-sku" required>
              </div>

              <div class="field">
                <label>Nome do produto *</label>
                <input id="product-name" required>
              </div>

              <div class="field">
                <label>Fornecedor *</label>
                <select id="product-supplier" required></select>
              </div>

              <div class="field">
                <label>Preço *</label>
                <input id="product-price" type="number" min="0" step="0.01" required>
              </div>

              <div class="field">
                <label>Categoria</label>
                <input id="product-category">
              </div>

              <div class="field">
                <label>Garantia em dias</label>
                <input id="product-warranty" type="number" min="0" value="0">
              </div>

              <div class="field">
                <label>Venda por caixa fechada?</label>
                <select id="product-box">
                  <option value="nao">Não — venda por unidade</option>
                  <option value="sim">Sim — venda somente em múltiplos</option>
                </select>
              </div>

              <div class="field">
                <label>Unidades por caixa</label>
                <input id="product-box-quantity" type="number" min="1" value="1">
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar produto</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <div class="toolbar">
            <h2>Produtos cadastrados</h2>
            <input
              id="product-search"
              style="max-width:280px"
              placeholder="Buscar produto ou SKU..."
              oninput="renderProducts()">
          </div>

          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>SKU</th>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Venda</th>
                  <th>Preço</th>
                  <th>Vendidos</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="products-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- FORNECEDORES -->
      <section class="page" id="page-fornecedores">
        <div class="panel">
          <h2>Cadastrar fornecedor</h2>

          <form id="supplier-form">
            <div class="grid-3">
              <div class="field">
                <label>Nome *</label>
                <input id="supplier-name" required>
              </div>

              <div class="field">
                <label>Contato</label>
                <input id="supplier-contact">
              </div>

              <div class="field">
                <label>Cor de identificação</label>
                <input id="supplier-color" type="color" value="#e50914">
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar fornecedor</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <h2>Fornecedores cadastrados</h2>

          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Fornecedor</th>
                  <th>Contato</th>
                  <th>Produtos</th>
                  <th>Ação</th>
                </tr>
              </thead>
              <tbody id="suppliers-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- VENDEDORES -->
      <section class="page" id="page-vendedores">
        <div class="panel">
          <h2>Cadastrar vendedor</h2>

          <form id="seller-form">
            <div class="grid-4">
              <div class="field">
                <label>Nome *</label>
                <input id="seller-name" required>
              </div>

              <div class="field">
                <label>Telefone</label>
                <input id="seller-phone">
              </div>

              <div class="field">
                <label>E-mail</label>
                <input id="seller-email" type="email">
              </div>

              <div class="field">
                <label>Meta mensal</label>
                <input id="seller-goal" type="number" min="0" step="0.01" value="0">
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar vendedor</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <h2>Vendedores cadastrados</h2>

          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Nome</th>
                  <th>Telefone</th>
                  <th>Meta</th>
                  <th>Faturamento</th>
                  <th>Ação</th>
                </tr>
              </thead>
              <tbody id="sellers-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- FINANCEIRO -->
      <section class="page" id="page-financeiro">
        <div class="cards">
          <div class="card">
            <div class="metric-label">A receber</div>
            <div class="metric-value green" id="finance-receivable">R$ 0,00</div>
          </div>

          <div class="card">
            <div class="metric-label">A pagar</div>
            <div class="metric-value red" id="finance-payable">R$ 0,00</div>
          </div>

          <div class="card">
            <div class="metric-label">Recebido</div>
            <div class="metric-value blue" id="finance-received">R$ 0,00</div>
          </div>

          <div class="card">
            <div class="metric-label">Resultado</div>
            <div class="metric-value purple" id="finance-result">R$ 0,00</div>
          </div>
        </div>

        <div class="panel">
          <h2>Nova movimentação</h2>

          <form id="finance-form">
            <div class="grid-4">
              <div class="field">
                <label>Tipo</label>
                <select id="finance-type">
                  <option value="receber">A receber</option>
                  <option value="pagar">A pagar</option>
                </select>
              </div>

              <div class="field">
                <label>Descrição *</label>
                <input id="finance-description" required>
              </div>

              <div class="field">
                <label>Valor *</label>
                <input id="finance-value" type="number" min="0" step="0.01" required>
              </div>

              <div class="field">
                <label>Vencimento *</label>
                <input id="finance-due" type="date" required>
              </div>

              <div class="field">
                <label>Status</label>
                <select id="finance-status">
                  <option value="pendente">Pendente</option>
                  <option value="pago">Pago</option>
                </select>
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar movimentação</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <h2>Movimentações</h2>

          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Tipo</th>
                  <th>Descrição</th>
                  <th>Valor</th>
                  <th>Vencimento</th>
                  <th>Status</th>
                  <th>Ação</th>
                </tr>
              </thead>
              <tbody id="finance-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- CURVA ABC -->
      <section class="page" id="page-abc">
        <div class="panel">
          <div class="toolbar">
            <div>
              <h2>Curva ABC de produtos</h2>
              <div class="muted">
                A representa os produtos responsáveis pelos primeiros 60%,
                B de 60% até 90% e C acima de 90%.
              </div>
            </div>

            <select id="abc-period" onchange="renderABC()">
              <option value="all">Todo o período</option>
              <option value="30">Últimos 30 dias</option>
              <option value="90">Últimos 90 dias</option>
              <option value="365">Últimos 365 dias</option>
            </select>
          </div>

          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Posição</th>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Curva</th>
                  <th>Quantidade</th>
                  <th>Faturamento</th>
                  <th>% acumulado</th>
                  <th>Clientes</th>
                </tr>
              </thead>
              <tbody id="abc-products"></tbody>
            </table>
          </div>
        </div>

        <div class="panel">
          <h2>Curva ABC de clientes</h2>

          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>Cliente</th>
                  <th>Curva</th>
                  <th>Pedidos</th>
                  <th>Faturamento</th>
                  <th>Produtos sugeridos</th>
                  <th>Ação</th>
                </tr>
              </thead>
              <tbody id="abc-clients"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- CONFIGURAÇÕES -->
      <section class="page" id="page-configuracoes">
        <div class="panel">
          <h2>Dados da empresa</h2>

          <form id="company-form">
            <div class="grid-3">
              <div class="field">
                <label>Nome da empresa *</label>
                <input id="company-name" required>
              </div>

              <div class="field">
                <label>CNPJ</label>
                <input id="company-document">
              </div>

              <div class="field">
                <label>Telefone</label>
                <input id="company-phone">
              </div>

              <div class="field">
                <label>E-mail</label>
                <input id="company-email" type="email">
              </div>

              <div class="field">
                <label>Logo da empresa</label>
                <input id="company-logo" placeholder="URL da imagem">
              </div>

              <div class="field full">
                <label>Endereço</label>
                <input id="company-address">
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar dados da empresa</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <h2>Observação</h2>

          <div class="muted">
            Os dados informados aqui serão utilizados no cabeçalho do PDF
            dos pedidos. A logo deve estar em uma URL pública de imagem.
          </div>
        </div>
      </section>

      <!-- PERFIL DO CLIENTE -->
      <section class="page" id="page-perfil">
        <div id="client-profile"></div>
      </section>
    </main>
  </div>

  <!-- MODAL DE VENDA -->
  <div class="modal" id="sale-modal">
    <div class="modal-box">
      <div class="modal-header">
        <h2>Nova venda</h2>
        <button class="close" onclick="closeModal('sale-modal')">×</button>
      </div>

      <form id="sale-form">
        <div class="grid-4">
          <div class="field">
            <label>Cliente *</label>
            <select id="sale-client" required></select>
          </div>

          <div class="field">
            <label>Vendedor *</label>
            <select id="sale-seller" required></select>
          </div>

          <div class="field">
            <label>Data *</label>
            <input id="sale-date" type="date" required>
          </div>

          <div class="field">
            <label>Canal</label>
            <select id="sale-channel">
              <option>Presencial</option>
              <option>WhatsApp</option>
              <option>Telefone</option>
              <option>Site</option>
              <option>Outro</option>
            </select>
          </div>
        </div>

        <div class="alert" style="margin-top:16px">
          Cada venda pode conter produtos de apenas um fornecedor.
          Para vender produtos de outro fornecedor, registre uma nova venda.
        </div>

        <h3>Itens da venda</h3>

        <div id="sale-lines"></div>

        <button type="button" class="button small" onclick="addSaleLine()">
          + Adicionar item
        </button>

        <div class="field" style="margin-top:15px">
          <label>Observações</label>
          <textarea id="sale-notes"></textarea>
        </div>

        <div style="margin-top:15px;text-align:right;font-size:20px">
          Total:
          <strong class="green" id="sale-total">R$ 0,00</strong>
        </div>

        <div class="actions">
          <button class="button primary">Salvar venda</button>
        </div>
      </form>
    </div>
  </div>

  <!-- MODAL DE META -->
  <div class="modal" id="goal-modal">
    <div class="modal-box">
      <div class="modal-header">
        <h2>Configurar meta</h2>
        <button class="close" onclick="closeModal('goal-modal')">×</button>
      </div>

      <form id="goal-form">
        <div class="grid-3">
          <div class="field">
            <label>Meta mensal</label>
            <input id="monthly-goal" type="number" min="0" step="0.01" required>
          </div>

          <div class="field">
            <label>Dias considerados</label>
            <input id="goal-days" type="number" min="1" max="31" value="30" required>
          </div>

          <div class="field">
            <label>Meta diária</label>
            <input id="daily-goal" type="number" readonly>
          </div>
        </div>

        <div class="actions">
          <button class="button primary">Salvar meta</button>
        </div>
      </form>
    </div>
  </div>

  <!-- MODAL DE PEDIDO -->
  <div class="modal" id="order-modal">
    <div class="modal-box">
      <div class="modal-header">
        <h2>Detalhes do pedido</h2>
        <button class="close" onclick="closeModal('order-modal')">×</button>
      </div>

      <div id="order-details"></div>
    </div>
  </div>

  <script>
    const STORAGE_KEY = "gestao_comercial_v3";

    let db = loadDB();
    let comparisonFilters = [];

    function loadDB() {
      let saved = null;

      try {
        saved = JSON.parse(localStorage.getItem(STORAGE_KEY));
      } catch (error) {
        saved = null;
      }

      if (!saved || typeof saved !== "object") {
        saved = {};
      }

      return {
        settings: saved.settings || {
          monthlyGoal: 0,
          goalDays: 30,
          dailyGoal: 0
        },

        company: saved.company || {
          name: "",
          document: "",
          phone: "",
          email: "",
          address: "",
          logo: ""
        },

        clients: Array.isArray(saved.clients) ? saved.clients : [],
        suppliers: Array.isArray(saved.suppliers) ? saved.suppliers : [],
        sellers: Array.isArray(saved.sellers) ? saved.sellers : [],
        products: Array.isArray(saved.products) ? saved.products : [],
        sales: Array.isArray(saved.sales) ? saved.sales : [],
        finances: Array.isArray(saved.finances) ? saved.finances : []
      };
    }

    function saveDB() {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(db));
    }

    function id(prefix) {
      return prefix + "_" +
        Date.now().toString(36) +
        Math.random().toString(36).slice(2, 8);
    }

    function today() {
      const date = new Date();

      return date.getFullYear() + "-" +
        String(date.getMonth() + 1).padStart(2, "0") + "-" +
        String(date.getDate()).padStart(2, "0");
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

      return parts.length === 3
        ? parts[2] + "/" + parts[1] + "/" + parts[0]
        : value;
    }

    function safe(value) {
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

    function findClient(clientId) {
      return db.clients.find(item => item.id === clientId);
    }

    function findSupplier(supplierId) {
      return db.suppliers.find(item => item.id === supplierId);
    }

    function findSeller(sellerId) {
      return db.sellers.find(item => item.id === sellerId);
    }

    function findProduct(productId) {
      return db.products.find(item => item.id === productId);
    }

    function totalSale(sale) {
      return (sale.items || []).reduce(function(total, item) {
        return total + Number(item.quantity || 0) * Number(item.price || 0);
      }, 0);
    }

    function productQuantity(productId, sales = db.sales) {
      return sales.reduce(function(total, sale) {
        return total + (sale.items || []).reduce(function(sum, item) {
          return sum + (
            item.productId === productId
              ? Number(item.quantity || 0)
              : 0
          );
        }, 0);
      }, 0);
    }

    function productRevenue(productId, sales = db.sales) {
      return sales.reduce(function(total, sale) {
        return total + (sale.items || []).reduce(function(sum, item) {
          return sum + (
            item.productId === productId
              ? Number(item.quantity || 0) * Number(item.price || 0)
              : 0
          );
        }, 0);
      }, 0);
    }

    function salesByClient(clientId, sales = db.sales) {
      return sales.filter(sale => sale.clientId === clientId);
    }

    function clientStats(clientId, sales = db.sales) {
      const list = salesByClient(clientId, sales);
      const dates = list
        .map(item => item.date)
        .filter(Boolean)
        .sort()
        .reverse();

      return {
        sales: list,
        revenue: list.reduce((sum, sale) => sum + totalSale(sale), 0),
        lastSale: dates[0] || "",
        quantities: list.reduce(function(result, sale) {
          (sale.items || []).forEach(function(item) {
            result[item.productId] =
              (result[item.productId] || 0) +
              Number(item.quantity || 0);
          });

          return result;
        }, {})
      };
    }

    function daysWithoutPurchase(clientId) {
      const last = clientStats(clientId).lastSale;

      if (!last) return Infinity;

      const date = new Date(last + "T12:00:00");

      return Math.floor((Date.now() - date.getTime()) / 86400000);
    }

    function chipSupplier(supplier) {
      if (!supplier) return "—";

      return `
        <span class="chip">
          <span class="dot" style="background:${supplier.color}"></span>
          ${safe(supplier.name)}
        </span>
      `;
    }

    function badgeABC(curve) {
      return `
        <span class="badge badge-${curve.toLowerCase()}">
          Curva ${curve}
        </span>
      `;
    }

    function calculateABC(rows) {
      const sorted = rows.slice().sort(function(a, b) {
        return Number(b.revenue || 0) - Number(a.revenue || 0);
      });

      const total = sorted.reduce(
        (sum, row) => sum + Number(row.revenue || 0),
        0
      );

      let accumulated = 0;

      return sorted.map(function(row, index) {
        const revenue = Number(row.revenue || 0);
        const individual = total ? revenue / total * 100 : 0;
        const previous = accumulated;

        accumulated += individual;

        let curve = "C";

        if (revenue > 0) {
          if (previous < 60) {
            curve = "A";
          } else if (previous < 90) {
            curve = "B";
          }
        }

        return {
          row,
          position: index + 1,
          individual,
          accumulated,
          curve
        };
      });
    }

    function getSalesByFilters(filters) {
      return db.sales.filter(function(sale) {
        if (filters.start && sale.date < filters.start) return false;
        if (filters.end && sale.date > filters.end) return false;

        if (filters.client && sale.clientId !== filters.client) {
          return false;
        }

        if (filters.seller && sale.sellerId !== filters.seller) {
          return false;
        }

        if (filters.channel && sale.channel !== filters.channel) {
          return false;
        }

        if (filters.supplier || filters.product) {
          const valid = (sale.items || []).some(function(item) {
            const supplierOK =
              !filters.supplier || item.supplierId === filters.supplier;

            const productOK =
              !filters.product || item.productId === filters.product;

            return supplierOK && productOK;
          });

          if (!valid) return false;
        }

        return true;
      });
    }

    function filterValues(prefix) {
      return {
        start: document.getElementById(prefix + "start")?.value || "",
        end: document.getElementById(prefix + "end")?.value || "",
        client: document.getElementById(prefix + "client")?.value || "",
        seller: document.getElementById(prefix + "seller")?.value || "",
        supplier: document.getElementById(prefix + "supplier")?.value || "",
        product: document.getElementById(prefix + "product")?.value || "",
        channel: document.getElementById(prefix + "channel")?.value || ""
      };
    }

    function populateFilter(prefix) {
      const fields = {
        client: document.getElementById(prefix + "client"),
        seller: document.getElementById(prefix + "seller"),
        supplier: document.getElementById(prefix + "supplier"),
        product: document.getElementById(prefix + "product"),
        channel: document.getElementById(prefix + "channel")
      };

      if (!fields.client) return;

      const current = {
        client: fields.client.value,
        seller: fields.seller.value,
        supplier: fields.supplier.value,
        product: fields.product.value,
        channel: fields.channel.value
      };

      fields.client.innerHTML =
        `<option value="">Todos os clientes</option>` +
        db.clients.map(item => `
          <option value="${item.id}">${safe(item.name)}</option>
        `).join("");

      fields.seller.innerHTML =
        `<option value="">Todos os vendedores</option>` +
        db.sellers.map(item => `
          <option value="${item.id}">${safe(item.name)}</option>
        `).join("");

      fields.supplier.innerHTML =
        `<option value="">Todos os fornecedores</option>` +
        db.suppliers.map(item => `
          <option value="${item.id}">${safe(item.name)}</option>
        `).join("");

      fields.product.innerHTML =
        `<option value="">Todos os produtos</option>` +
        db.products.map(item => `
          <option value="${item.id}">
            ${safe(item.sku)} — ${safe(item.name)}
          </option>
        `).join("");

      fields.channel.innerHTML = `
        <option value="">Todos os canais</option>
        <option>Presencial</option>
        <option>WhatsApp</option>
        <option>Telefone</option>
        <option>Site</option>
        <option>Outro</option>
      `;

      fields.client.value = current.client;
      fields.seller.value = current.seller;
      fields.supplier.value = current.supplier;
      fields.product.value = current.product;
      fields.channel.value = current.channel;
    }

    function renderComparisonBoxes() {
      const container = document.getElementById("comparisons");

      container.innerHTML = comparisonFilters.map(function(item, index) {
        return `
          <div class="comparison-box">
            <div class="toolbar">
              <strong>Comparação ${index + 1}</strong>

              <button
                class="button small danger"
                type="button"
                onclick="removeComparison(${index})">
                Remover
              </button>
            </div>

            <div class="filter-grid">
              <div class="field">
                <label>Data inicial</label>
                <input
                  type="date"
                  id="compare-${index}-start"
                  value="${item.start}"
                  onchange="saveComparison(${index})">
              </div>

              <div class="field">
                <label>Data final</label>
                <input
                  type="date"
                  id="compare-${index}-end"
                  value="${item.end}"
                  onchange="saveComparison(${index})">
              </div>

              <div class="field">
                <label>Cliente</label>
                <select
                  id="compare-${index}-client"
                  onchange="saveComparison(${index})">
                </select>
              </div>

              <div class="field">
                <label>Vendedor</label>
                <select
                  id="compare-${index}-seller"
                  onchange="saveComparison(${index})">
                </select>
              </div>

              <div class="field">
                <label>Fornecedor</label>
                <select
                  id="compare-${index}-supplier"
                  onchange="saveComparison(${index})">
                </select>
              </div>

              <div class="field">
                <label>Produto</label>
                <select
                  id="compare-${index}-product"
                  onchange="saveComparison(${index})">
                </select>
              </div>

              <div class="field">
                <label>Canal</label>
                <select
                  id="compare-${index}-channel"
                  onchange="saveComparison(${index})">
                  <option value="">Todos os canais</option>
                  <option>Presencial</option>
                  <option>WhatsApp</option>
                  <option>Telefone</option>
                  <option>Site</option>
                  <option>Outro</option>
                </select>
              </div>
            </div>
          </div>
        `;
      }).join("");

      comparisonFilters.forEach(function(item, index) {
        populateComparisonSelects(index);
      });
    }

    function populateComparisonSelects(index) {
      const prefix = "compare-" + index + "-";

      const client = document.getElementById(prefix + "client");
      const seller = document.getElementById(prefix + "seller");
      const supplier = document.getElementById(prefix + "supplier");
      const product = document.getElementById(prefix + "product");
      const channel = document.getElementById(prefix + "channel");

      if (!client) return;

      const values = comparisonFilters[index];

      client.innerHTML =
        `<option value="">Todos os clientes</option>` +
        db.clients.map(item => `
          <option value="${item.id}">${safe(item.name)}</option>
        `).join("");

      seller.innerHTML =
        `<option value="">Todos os vendedores</option>` +
        db.sellers.map(item => `
          <option value="${item.id}">${safe(item.name)}</option>
        `).join("");

      supplier.innerHTML =
        `<option value="">Todos os fornecedores</option>` +
        db.suppliers.map(item => `
          <option value="${item.id}">${safe(item.name)}</option>
        `).join("");

      product.innerHTML =
        `<option value="">Todos os produtos</option>` +
        db.products.map(item => `
          <option value="${item.id}">
            ${safe(item.sku)} — ${safe(item.name)}
          </option>
        `).join("");

      client.value = values.client || "";
      seller.value = values.seller || "";
      supplier.value = values.supplier || "";
      product.value = values.product || "";
      channel.value = values.channel || "";
    }

    function saveComparison(index) {
      const prefix = "compare-" + index + "-";

      comparisonFilters[index] = {
        start: document.getElementById(prefix + "start").value,
        end: document.getElementById(prefix + "end").value,
        client: document.getElementById(prefix + "client").value,
        seller: document.getElementById(prefix + "seller").value,
        supplier: document.getElementById(prefix + "supplier").value,
        product: document.getElementById(prefix + "product").value,
        channel: document.getElementById(prefix + "channel").value
      };

      renderDashboard();
    }

    function addComparison() {
      comparisonFilters.push({
        start: "",
        end: "",
        client: "",
        seller: "",
        supplier: "",
        product: "",
        channel: ""
      });

      renderComparisonBoxes();
      renderDashboard();
    }

    function removeComparison(index) {
      comparisonFilters.splice(index, 1);
      renderComparisonBoxes();
      renderDashboard();
    }

    function clearComparisons() {
      comparisonFilters = [];
      renderComparisonBoxes();
      renderDashboard();
    }

    function applyShortcut() {
      const value = document.getElementById("filter-shortcut").value;
      const start = document.getElementById("filter-start");
      const end = document.getElementById("filter-end");
      const now = new Date();

      if (!value) return;

      if (value === "today") {
        start.value = today();
        end.value = today();
      }

      if (["7", "30", "90"].includes(value)) {
        const initial = new Date();
        initial.setDate(initial.getDate() - Number(value));

        start.value = initial.toISOString().slice(0, 10);
        end.value = today();
      }

      if (value === "month") {
        start.value = now.getFullYear() + "-" +
          String(now.getMonth() + 1).padStart(2, "0") +
          "-01";

        end.value = today();
      }

      if (value === "previous-month") {
        const first = new Date(now.getFullYear(), now.getMonth() - 1, 1);
        const last = new Date(now.getFullYear(), now.getMonth(), 0);

        start.value = first.toISOString().slice(0, 10);
        end.value = last.toISOString().slice(0, 10);
      }

      if (value === "year") {
        start.value = now.getFullYear() + "-01-01";
        end.value = today();
      }

      renderDashboard();
    }

    function clearDashboardFilters() {
      [
        "filter-start",
        "filter-end",
        "filter-client",
        "filter-seller",
        "filter-supplier",
        "filter-product",
        "filter-channel"
      ].forEach(function(id) {
        const element = document.getElementById(id);

        if (element) element.value = "";
      });

      document.getElementById("filter-shortcut").value = "";
      comparisonFilters = [];
      renderComparisonBoxes();
      renderDashboard();
    }

    function renderDashboard() {
      populateFilter("filter-");

      const filters = filterValues("filter-");
      const sales = getSalesByFilters(filters);
      const revenue = sales.reduce((sum, sale) => sum + totalSale(sale), 0);
      const customers = new Set(sales.map(sale => sale.clientId)).size;
      const average = sales.length ? revenue / sales.length : 0;

      document.getElementById("dash-revenue").textContent = money(revenue);
      document.getElementById("dash-orders").textContent = sales.length;
      document.getElementById("dash-clients").textContent = customers;
      document.getElementById("dash-ticket").textContent = money(average);

      const result = [];

      result.push(`
        <div class="card comparison-card main-period">
          <div class="metric-label">Período principal</div>
          <div class="metric-value">${money(revenue)}</div>
          <div class="muted">${sales.length} pedido(s)</div>
        </div>
      `);

      comparisonFilters.forEach(function(item, index) {
        const comparisonSales = getSalesByFilters(item);
        const comparisonRevenue = comparisonSales.reduce(
          (sum, sale) => sum + totalSale(sale),
          0
        );

        result.push(`
          <div class="card comparison-card">
            <div class="metric-label">Comparação ${index + 1}</div>
            <div class="metric-value">${money(comparisonRevenue)}</div>
            <div class="muted">${comparisonSales.length} pedido(s)</div>
          </div>
        `);
      });

      document.getElementById("comparison-results").innerHTML =
        result.join("");

      const alerts = [];

      if (!db.settings.monthlyGoal) {
        alerts.push(`
          <div class="alert">
            Configure a meta mensal para acompanhar o progresso.
          </div>
        `);
      }

      if (!sales.length && (
        filters.start ||
        filters.end ||
        filters.client ||
        filters.seller ||
        filters.supplier ||
        filters.product ||
        filters.channel
      )) {
        alerts.push(`
          <div class="alert red-alert">
            Nenhuma venda foi encontrada para os filtros selecionados.
          </div>
        `);
      }

      document.getElementById("dashboard-alerts").innerHTML =
        alerts.join("");

      renderGoal();
      renderBirthdays();
      renderInactive();
      renderOpportunities();
      renderUnusedProducts();
    }

    function renderGoal() {
      const month = today().slice(0, 7);
      const sales = db.sales.filter(sale => sale.date.slice(0, 7) === month);
      const sold = sales.reduce((sum, sale) => sum + totalSale(sale), 0);
      const goal = Number(db.settings.monthlyGoal || 0);
      const days = Number(db.settings.goalDays || 30);
      const daily = goal / Math.max(days, 1);
      const missing = Math.max(goal - sold, 0);
      const progress = goal ? Math.min(sold / goal * 100, 100) : 0;

      document.getElementById("goal-month").textContent = money(goal);
      document.getElementById("goal-day").textContent = money(daily);
      document.getElementById("goal-sold").textContent = money(sold);
      document.getElementById("goal-missing").textContent = money(missing);
      document.getElementById("goal-progress").style.width = progress + "%";

      document.getElementById("goal-text").textContent =
        progress.toFixed(1) + "% da meta atingida. " +
        days + " dias considerados.";
    }

    function renderBirthdays() {
      const month = today().slice(5, 7);

      const list = db.clients.filter(function(client) {
        return client.birth && client.birth.slice(5, 7) === month;
      });

      document.getElementById("birthdays").innerHTML =
        list.length
          ? list.map(function(client) {
              return `
                <div class="list-item">
                  <strong>${safe(client.name)}</strong>
                  <div class="muted">
                    Aniversário: ${dateBR(client.birth)}
                  </div>
                  <div class="actions">
                    <button
                      class="button small"
                      onclick="openClientProfile('${client.id}')">
                      Ver perfil
                    </button>
                  </div>
                </div>
              `;
            }).join("")
          : `<div class="empty">Nenhum aniversariante neste mês.</div>`;
    }

    function renderInactive() {
      const list = db.clients.filter(function(client) {
        const days = daysWithoutPurchase(client.id);
        return days === Infinity || days > 15;
      });

      document.getElementById("inactive-clients").innerHTML =
        list.length
          ? list.map(function(client) {
              const days = daysWithoutPurchase(client.id);

              return `
                <div class="list-item">
                  <strong>${safe(client.name)}</strong>
                  <div class="muted">
                    ${
                      days === Infinity
                        ? "Nunca comprou"
                        : days + " dias sem comprar"
                    }
                  </div>
                </div>
              `;
            }).join("")
          : `<div class="empty">Nenhum cliente inativo.</div>`;
    }

    function getSuggestions(clientId) {
      const stats = clientStats(clientId);

      return calculateABC(db.products.map(function(product) {
        return {
          product,
          revenue: productRevenue(product.id)
        };
      })).filter(function(item) {
        return !Object.keys(stats.quantities).includes(item.row.product.id);
      });
    }

    function renderOpportunities() {
      const list = db.clients.filter(function(client) {
        return clientStats(client.id).sales.length &&
          getSuggestions(client.id).length;
      });

      document.getElementById("opportunities").innerHTML =
        list.length
          ? list.slice(0, 10).map(function(client) {
              const suggestions = getSuggestions(client.id)
                .slice(0, 3)
                .map(item => item.row.product.name)
                .join(", ");

              return `
                <div class="list-item">
                  <strong>${safe(client.name)}</strong>
                  <div class="muted">
                    Sugestões: ${safe(suggestions)}
                  </div>
                  <div class="actions">
                    <button
                      class="button small"
                      onclick="openClientProfile('${client.id}')">
                      Ver análise
                    </button>
                  </div>
                </div>
              `;
            }).join("")
          : `<div class="empty">Nenhuma oportunidade encontrada.</div>`;
    }

    function renderUnusedProducts() {
      const list = db.products.filter(
        product => productQuantity(product.id) === 0
      );

      document.getElementById("unused-products").innerHTML =
        list.length
          ? list.map(product => `
              <div class="list-item">
                <strong>${safe(product.name)}</strong>
                <div class="muted">SKU: ${safe(product.sku)}</div>
              </div>
            `).join("")
          : `<div class="empty">Todos os produtos possuem pedidos.</div>`;
    }

    document.getElementById("client-form").addEventListener("submit", function(event) {
      event.preventDefault();

      db.clients.push({
        id: id("client"),
        name: document.getElementById("client-name").value.trim(),
        phone: document.getElementById("client-phone").value.trim(),
        email: document.getElementById("client-email").value.trim(),
        birth: document.getElementById("client-birth").value,
        document: document.getElementById("client-document").value.trim(),
        logo: document.getElementById("client-logo").value.trim(),
        address: document.getElementById("client-address").value.trim()
      });

      saveDB();
      event.target.reset();
      renderAll();

      alert("Cliente cadastrado com sucesso.");
    });

    function renderClients() {
      const search = (
        document.getElementById("client-search")?.value || ""
      ).toLowerCase();

      const list = db.clients.filter(function(client) {
        return client.name.toLowerCase().includes(search) ||
          (client.document || "").toLowerCase().includes(search);
      });

      document.getElementById("clients-table").innerHTML =
        list.length
          ? list.map(function(client) {
              const stats = clientStats(client.id);
              const inactive =
                daysWithoutPurchase(client.id) === Infinity ||
                daysWithoutPurchase(client.id) > 15;

              return `
                <tr
                  class="clickable"
                  onclick="openClientProfile('${client.id}')">
                  <td><strong>${safe(client.name)}</strong></td>
                  <td>${safe(client.phone || "—")}</td>
                  <td>${dateBR(stats.lastSale)}</td>
                  <td>
                    <span class="badge ${
                      inactive ? "badge-inactive" : "badge-active"
                    }">
                      ${inactive ? "Inativo" : "Ativo"}
                    </span>
                  </td>
                  <td>${stats.sales.length}</td>
                  <td class="green">${money(stats.revenue)}</td>
                  <td>
                    <button
                      class="button small danger"
                      onclick="event.stopPropagation();deleteClient('${client.id}')">
                      Excluir
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="7" class="empty">
                Nenhum cliente encontrado.
              </td>
            </tr>
          `;
    }

    function deleteClient(clientId) {
      if (!confirm("Excluir este cliente e suas vendas?")) return;

      db.clients = db.clients.filter(item => item.id !== clientId);
      db.sales = db.sales.filter(item => item.clientId !== clientId);

      saveDB();
      renderAll();
    }

    document.getElementById("supplier-form").addEventListener("submit", function(event) {
      event.preventDefault();

      db.suppliers.push({
        id: id("supplier"),
        name: document.getElementById("supplier-name").value.trim(),
        contact: document.getElementById("supplier-contact").value.trim(),
        color: document.getElementById("supplier-color").value
      });

      saveDB();
      event.target.reset();
      renderAll();

      alert("Fornecedor cadastrado com sucesso.");
    });

    function renderSuppliers() {
      document.getElementById("suppliers-table").innerHTML =
        db.suppliers.length
          ? db.suppliers.map(function(supplier) {
              const products = db.products.filter(
                product => product.supplierId === supplier.id
              );

              return `
                <tr>
                  <td>${chipSupplier(supplier)}</td>
                  <td>${safe(supplier.contact || "—")}</td>
                  <td>
                    ${
                      products.length
                        ? products.map(product => `
                            <div class="muted">
                              ${safe(product.sku)} — ${safe(product.name)}
                            </div>
                          `).join("")
                        : "Nenhum produto"
                    }
                  </td>
                  <td>
                    <button
                      class="button small danger"
                      onclick="deleteSupplier('${supplier.id}')">
                      Excluir
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="4" class="empty">
                Nenhum fornecedor cadastrado.
              </td>
            </tr>
          `;
    }

    function deleteSupplier(supplierId) {
      if (db.products.some(product => product.supplierId === supplierId)) {
        alert("Este fornecedor possui produtos vinculados.");
        return;
      }

      db.suppliers = db.suppliers.filter(item => item.id !== supplierId);
      saveDB();
      renderAll();
    }

    document.getElementById("product-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const sku = document.getElementById("product-sku")
        .value.trim()
        .toUpperCase();

      if (db.products.some(product => product.sku === sku)) {
        alert("Este SKU já está cadastrado.");
        return;
      }

      const box = document.getElementById("product-box").value;
      const boxQuantity = Number(
        document.getElementById("product-box-quantity").value || 1
      );

      if (box === "sim" && boxQuantity < 1) {
        alert("Informe a quantidade de unidades por caixa.");
        return;
      }

      db.products.push({
        id: id("product"),
        sku,
        name: document.getElementById("product-name").value.trim(),
        supplierId: document.getElementById("product-supplier").value,
        price: Number(document.getElementById("product-price").value || 0),
        category: document.getElementById("product-category").value.trim(),
        warrantyDays: Number(
          document.getElementById("product-warranty").value || 0
        ),
        soldByBox: box === "sim",
        unitsPerBox: box === "sim" ? boxQuantity : 1
      });

      saveDB();
      event.target.reset();
      renderAll();

      alert("Produto cadastrado com sucesso.");
    });

    function renderProducts() {
      const search = (
        document.getElementById("product-search")?.value || ""
      ).toLowerCase();

      const list = db.products.filter(function(product) {
        return product.name.toLowerCase().includes(search) ||
          product.sku.toLowerCase().includes(search);
      });

      document.getElementById("products-table").innerHTML =
        list.length
          ? list.map(function(product) {
              const supplier = findSupplier(product.supplierId);

              return `
                <tr>
                  <td>${safe(product.sku)}</td>
                  <td>
                    <strong>${safe(product.name)}</strong>
                    <br>
                    <span class="muted">
                      ${safe(product.category || "Sem categoria")}
                    </span>
                  </td>
                  <td>${chipSupplier(supplier)}</td>
                  <td>
                    ${
                      product.soldByBox
                        ? "Caixa com " + product.unitsPerBox + " un."
                        : "Unidade"
                    }
                  </td>
                  <td>${money(product.price)}</td>
                  <td>${productQuantity(product.id)}</td>
                  <td>
                    <button
                      class="button small danger"
                      onclick="deleteProduct('${product.id}')">
                      Excluir
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="7" class="empty">
                Nenhum produto encontrado.
              </td>
            </tr>
          `;
    }

    function deleteProduct(productId) {
      if (db.sales.some(sale =>
        (sale.items || []).some(item => item.productId === productId)
      )) {
        alert("Este produto possui histórico de vendas.");
        return;
      }

      db.products = db.products.filter(item => item.id !== productId);
      saveDB();
      renderAll();
    }

    document.getElementById("seller-form").addEventListener("submit", function(event) {
      event.preventDefault();

      db.sellers.push({
        id: id("seller"),
        name: document.getElementById("seller-name").value.trim(),
        phone: document.getElementById("seller-phone").value.trim(),
        email: document.getElementById("seller-email").value.trim(),
        goal: Number(document.getElementById("seller-goal").value || 0)
      });

      saveDB();
      event.target.reset();
      renderAll();

      alert("Vendedor cadastrado com sucesso.");
    });

    function renderSellers() {
      document.getElementById("sellers-table").innerHTML =
        db.sellers.length
          ? db.sellers.map(function(seller) {
              const sales = db.sales.filter(
                sale => sale.sellerId === seller.id
              );

              const revenue = sales.reduce(
                (sum, sale) => sum + totalSale(sale),
                0
              );

              return `
                <tr>
                  <td>${safe(seller.name)}</td>
                  <td>${safe(seller.phone || "—")}</td>
                  <td>${money(seller.goal)}</td>
                  <td class="green">${money(revenue)}</td>
                  <td>
                    <button
                      class="button small danger"
                      onclick="deleteSeller('${seller.id}')">
                      Excluir
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="5" class="empty">
                Nenhum vendedor cadastrado.
              </td>
            </tr>
          `;
    }

    function deleteSeller(sellerId) {
      if (db.sales.some(sale => sale.sellerId === sellerId)) {
        alert("Este vendedor possui vendas registradas.");
        return;
      }

      db.sellers = db.sellers.filter(item => item.id !== sellerId);
      saveDB();
      renderAll();
    }

    function populateGeneralSelects() {
      const productSupplier = document.getElementById("product-supplier");
      const saleClient = document.getElementById("sale-client");
      const saleSeller = document.getElementById("sale-seller");

      productSupplier.innerHTML =
        `<option value="">Selecione...</option>` +
        db.suppliers.map(item => `
          <option value="${item.id}">${safe(item.name)}</option>
        `).join("");

      saleClient.innerHTML =
        `<option value="">Selecione...</option>` +
        db.clients.map(item => `
          <option value="${item.id}">${safe(item.name)}</option>
        `).join("");

      saleSeller.innerHTML =
        `<option value="">Selecione...</option>` +
        db.sellers.map(item => `
          <option value="${item.id}">${safe(item.name)}</option>
        `).join("");

      populateFilter("filter-");
    }

    function openSaleModal(clientId = "") {
      populateGeneralSelects();

      document.getElementById("sale-client").value = clientId;
      document.getElementById("sale-seller").value = "";
      document.getElementById("sale-date").value = today();
      document.getElementById("sale-channel").value = "Presencial";
      document.getElementById("sale-notes").value = "";
      document.getElementById("sale-lines").innerHTML = "";

      addSaleLine();

      document.getElementById("sale-modal").classList.add("open");
    }

    function addSaleLine() {
      const line = document.createElement("div");

      line.className = "sale-row";

      line.innerHTML = `
        <div class="field supplier-field">
          <label>Fornecedor *</label>
          <select class="line-supplier" onchange="loadLineProducts(this)">
            <option value="">Selecione...</option>
            ${db.suppliers.map(item => `
              <option value="${item.id}">
                ${safe(item.name)}
              </option>
            `).join("")}
          </select>
        </div>

        <div class="field product-field">
          <label>Produto / SKU *</label>
          <select
            class="line-product"
            onchange="updateSaleTotal()"
            disabled>
            <option value="">Selecione o fornecedor...</option>
          </select>
        </div>

        <div class="field">
          <label>Quantidade</label>
          <input
            class="line-quantity"
            type="number"
            min="1"
            value="1"
            oninput="updateSaleTotal()">
        </div>

        <div class="line-total">R$ 0,00</div>

        <button
          type="button"
          class="button small danger"
          onclick="this.parentElement.remove();updateSaleTotal()">
          ×
        </button>
      `;

      document.getElementById("sale-lines").appendChild(line);
      updateSaleTotal();
    }

    function loadLineProducts(supplierSelect) {
      const row = supplierSelect.closest(".sale-row");
      const productSelect = row.querySelector(".line-product");
      const supplierId = supplierSelect.value;

      const products = db.products.filter(
        product => product.supplierId === supplierId
      );

      productSelect.disabled = !supplierId;

      productSelect.innerHTML = supplierId
        ? `<option value="">Selecione...</option>` +
          products.map(product => `
            <option value="${product.id}">
              ${safe(product.sku)} — ${safe(product.name)}
              (${money(product.price)})
            </option>
          `).join("")
        : `<option value="">Selecione o fornecedor...</option>`;

      updateSaleTotal();
    }

    function updateSaleTotal() {
      let total = 0;

      document.querySelectorAll(".sale-row").forEach(function(row) {
        const product = findProduct(
          row.querySelector(".line-product")?.value
        );

        const quantity = Number(
          row.querySelector(".line-quantity")?.value || 0
        );

        const lineTotal = product ? product.price * quantity : 0;
        total += lineTotal;

        row.querySelector(".line-total").textContent = money(lineTotal);
      });

      document.getElementById("sale-total").textContent = money(total);
    }

    document.getElementById("sale-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const rows = Array.from(document.querySelectorAll(".sale-row"));
      const items = [];
      let supplierOfSale = "";
      let invalid = false;

      rows.forEach(function(row) {
        const supplierId = row.querySelector(".line-supplier").value;
        const productId = row.querySelector(".line-product").value;
        const quantity = Number(
          row.querySelector(".line-quantity").value || 0
        );

        if (!supplierId || !productId || quantity <= 0) {
          invalid = true;
          return;
        }

        if (!supplierOfSale) {
          supplierOfSale = supplierId;
        }

        if (supplierOfSale !== supplierId) {
          invalid = true;
          alert(
            "Não é permitido misturar fornecedores na mesma venda. " +
            "Registre outra venda para o fornecedor diferente."
          );
          return;
        }

        const product = findProduct(productId);

        if (!product || product.supplierId !== supplierId) {
          invalid = true;
          return;
        }

        if (
          product.soldByBox &&
          quantity % Number(product.unitsPerBox || 1) !== 0
        ) {
          invalid = true;

          alert(
            "O produto " + product.name +
            " deve ser vendido em múltiplos de " +
            product.unitsPerBox + " unidades."
          );

          return;
        }

        items.push({
          productId: product.id,
          supplierId,
          sku: product.sku,
          quantity,
          price: product.price
        });
      });

      if (invalid || !items.length) {
        alert("Preencha corretamente os itens da venda.");
        return;
      }

      const clientId = document.getElementById("sale-client").value;
      const sellerId = document.getElementById("sale-seller").value;

      if (!clientId || !sellerId) {
        alert("Selecione o cliente e o vendedor.");
        return;
      }

      db.sales.push({
        id: id("sale"),
        clientId,
        sellerId,
        date: document.getElementById("sale-date").value,
        channel: document.getElementById("sale-channel").value,
        notes: document.getElementById("sale-notes").value.trim(),
        items
      });

      saveDB();
      closeModal("sale-modal");
      renderAll();

      alert("Venda registrada com sucesso.");
    });

    document.getElementById("finance-form").addEventListener("submit", function(event) {
      event.preventDefault();

      db.finances.push({
        id: id("finance"),
        type: document.getElementById("finance-type").value,
        description: document.getElementById("finance-description").value.trim(),
        value: Number(document.getElementById("finance-value").value || 0),
        due: document.getElementById("finance-due").value,
        status: document.getElementById("finance-status").value
      });

      saveDB();
      event.target.reset();
      renderFinance();

      alert("Movimentação salva.");
    });

    function renderFinance() {
      let receivable = 0;
      let payable = 0;
      let received = 0;
      let paid = 0;

      db.finances.forEach(function(item) {
        if (item.type === "receber") {
          item.status === "pago"
            ? received += item.value
            : receivable += item.value;
        } else {
          item.status === "pago"
            ? paid += item.value
            : payable += item.value;
        }
      });

      document.getElementById("finance-receivable").textContent =
        money(receivable);

      document.getElementById("finance-payable").textContent =
        money(payable);

      document.getElementById("finance-received").textContent =
        money(received);

      document.getElementById("finance-result").textContent =
        money(received - paid);

      document.getElementById("finance-table").innerHTML =
        db.finances.length
          ? db.finances.map(function(item) {
              return `
                <tr>
                  <td>${item.type === "receber" ? "A receber" : "A pagar"}</td>
                  <td>${safe(item.description)}</td>
                  <td>${money(item.value)}</td>
                  <td>${dateBR(item.due)}</td>
                  <td>${safe(item.status)}</td>
                  <td>
                    <button
                      class="button small danger"
                      onclick="deleteFinance('${item.id}')">
                      Excluir
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="6" class="empty">
                Nenhuma movimentação financeira.
              </td>
            </tr>
          `;
    }

    function deleteFinance(financeId) {
      db.finances = db.finances.filter(item => item.id !== financeId);
      saveDB();
      renderFinance();
    }

    function abcSales() {
      const period = document.getElementById("abc-period").value;

      if (period === "all") return db.sales;

      const start = new Date();
      start.setDate(start.getDate() - Number(period));

      return db.sales.filter(function(sale) {
        return new Date(sale.date + "T12:00:00") >= start;
      });
    }

    function renderABC() {
      const sales = abcSales();

      const products = db.products.map(function(product) {
        const relatedSales = sales.filter(sale =>
          (sale.items || []).some(item => item.productId === product.id)
        );

        return {
          product,
          revenue: productRevenue(product.id, sales),
          quantity: productQuantity(product.id, sales),
          clients: new Set(
            relatedSales.map(sale => sale.clientId)
          ).size
        };
      });

      const abcProducts = calculateABC(products);

      document.getElementById("abc-products").innerHTML =
        abcProducts.length
          ? abcProducts.map(function(item) {
              const product = item.row.product;
              const supplier = findSupplier(product.supplierId);

              return `
                <tr class="abc-${item.curve.toLowerCase()}">
                  <td>${item.position}</td>
                  <td>
                    <strong>${safe(product.name)}</strong>
                    <br>
                    <span class="muted">${safe(product.sku)}</span>
                  </td>
                  <td>${chipSupplier(supplier)}</td>
                  <td>${badgeABC(item.curve)}</td>
                  <td>${item.row.quantity}</td>
                  <td class="green">${money(item.row.revenue)}</td>
                  <td>${item.accumulated.toFixed(2)}%</td>
                  <td>${item.row.clients}</td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="8" class="empty">
                Cadastre produtos e vendas para calcular a curva ABC.
              </td>
            </tr>
          `;

      const clients = db.clients.map(function(client) {
        const stats = clientStats(client.id, sales);

        return {
          client,
          stats,
          revenue: stats.revenue
        };
      });

      const abcClients = calculateABC(clients);

      document.getElementById("abc-clients").innerHTML =
        abcClients.length
          ? abcClients.map(function(item) {
              const suggestions = getSuggestions(item.row.client.id)
                .slice(0, 3)
                .map(x => x.row.product.name)
                .join(", ");

              return `
                <tr class="abc-${item.curve.toLowerCase()}">
                  <td>${safe(item.row.client.name)}</td>
                  <td>${badgeABC(item.curve)}</td>
                  <td>${item.row.stats.sales.length}</td>
                  <td class="green">${money(item.row.revenue)}</td>
                  <td>${safe(suggestions || "Nenhuma")}</td>
                  <td>
                    <button
                      class="button small"
                      onclick="openClientProfile('${item.row.client.id}')">
                      Ver perfil
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="6" class="empty">
                Cadastre clientes e vendas para calcular a curva ABC.
              </td>
            </tr>
          `;
    }

    function openClientProfile(clientId) {
      const client = findClient(clientId);

      if (!client) return;

      const stats = clientStats(clientId);
      const suggestions = getSuggestions(clientId);

      document.getElementById("client-profile").innerHTML = `
        <div class="profile-header">
          <div>
            <button
              class="button small"
              onclick="showPage('clientes');renderAll()">
              ← Voltar para clientes
            </button>

            <h2 style="margin-top:15px">${safe(client.name)}</h2>

            <div class="muted">
              ${safe(client.phone || "Sem telefone")}
              · ${safe(client.email || "Sem e-mail")}
              · ${safe(client.document || "Sem documento")}
            </div>
          </div>

          <button
            class="button primary"
            onclick="openSaleModal('${client.id}')">
            + Nova venda
          </button>
        </div>

        <div class="cards">
          <div class="card">
            <div class="metric-label">Pedidos</div>
            <div class="metric-value">${stats.sales.length}</div>
          </div>

          <div class="card">
            <div class="metric-label">Faturamento</div>
            <div class="metric-value green">${money(stats.revenue)}</div>
          </div>

          <div class="card">
            <div class="metric-label">Última compra</div>
            <div class="metric-value" style="font-size:17px">
              ${dateBR(stats.lastSale)}
            </div>
          </div>

          <div class="card">
            <div class="metric-label">Dias sem comprar</div>
            <div class="metric-value yellow">
              ${
                daysWithoutPurchase(clientId) === Infinity
                  ? "Nunca"
                  : daysWithoutPurchase(clientId)
              }
            </div>
          </div>
        </div>

        <div class="profile-grid">
          <div class="panel">
            <h2>Histórico de pedidos</h2>

            <div class="list">
              ${
                stats.sales.length
                  ? stats.sales.map(function(sale) {
                      return `
                        <div class="list-item">
                          <strong>
                            ${dateBR(sale.date)} · ${money(totalSale(sale))}
                          </strong>

                          <div class="muted">
                            Vendedor:
                            ${safe(findSeller(sale.sellerId)?.name || "—")}
                          </div>

                          <div class="actions">
                            <button
                              class="button small"
                              onclick="openOrder('${sale.id}')">
                              Detalhes
                            </button>

                            <button
                              class="button small primary"
                              onclick="downloadPDF('${sale.id}')">
                              Baixar PDF
                            </button>
                          </div>
                        </div>
                      `;
                    }).join("")
                  : `<div class="empty">Nenhum pedido registrado.</div>`
              }
            </div>
          </div>

          <div class="panel">
            <h2>Sugestões de produtos</h2>

            <div class="list">
              ${
                suggestions.length
                  ? suggestions.slice(0, 15).map(function(item) {
                      return `
                        <div class="list-item abc-${item.curve.toLowerCase()}">
                          <strong>${safe(item.row.product.name)}</strong>
                          <div class="muted">
                            SKU: ${safe(item.row.product.sku)}
                            · ${badgeABC(item.curve)}
                          </div>
                        </div>
                      `;
                    }).join("")
                  : `<div class="empty">Nenhuma sugestão no momento.</div>`
              }
            </div>
          </div>
        </div>
      `;

      showPage("perfil");
    }

    function openOrder(saleId) {
      const sale = db.sales.find(item => item.id === saleId);

      if (!sale) return;

      const client = findClient(sale.clientId);
      const seller = findSeller(sale.sellerId);

      document.getElementById("order-details").innerHTML = `
        <div class="card">
          <strong>${safe(client?.name || "Cliente")}</strong>

          <div class="muted">
            ${safe(client?.phone || "Sem telefone")}
            · ${safe(client?.email || "Sem e-mail")}
          </div>

          <div class="muted" style="margin-top:6px">
            Data: ${dateBR(sale.date)}
            · Vendedor: ${safe(seller?.name || "—")}
          </div>
        </div>

        <div class="table-wrap" style="margin-top:15px">
          <table>
            <thead>
              <tr>
                <th>Fornecedor</th>
                <th>SKU</th>
                <th>Produto</th>
                <th>Qtd.</th>
                <th>Preço</th>
                <th>Total</th>
              </tr>
            </thead>

            <tbody>
              ${(sale.items || []).map(function(item) {
                const product = findProduct(item.productId);
                const supplier = findSupplier(item.supplierId);

                return `
                  <tr>
                    <td>${chipSupplier(supplier)}</td>
                    <td>${safe(item.sku)}</td>
                    <td>${safe(product?.name || "Produto removido")}</td>
                    <td>${item.quantity}</td>
                    <td>${money(item.price)}</td>
                    <td class="green">
                      ${money(item.price * item.quantity)}
                    </td>
                  </tr>
                `;
              }).join("")}
            </tbody>
          </table>
        </div>

        <div style="margin-top:16px;text-align:right;font-size:20px">
          Total:
          <strong class="green">${money(totalSale(sale))}</strong>
        </div>

        <div class="actions">
          <button
            class="button primary"
            onclick="downloadPDF('${sale.id}')">
            Baixar PDF
          </button>
        </div>
      `;

      document.getElementById("order-modal").classList.add("open");
    }

    function downloadPDF(saleId) {
      const sale = db.sales.find(item => item.id === saleId);
      const PDF = window.jspdf?.jsPDF;

      if (!sale || !PDF) {
        alert("Não foi possível gerar o PDF.");
        return;
      }

      const company = db.company;
      const client = findClient(sale.clientId);
      const seller = findSeller(sale.sellerId);
      const pdf = new PDF();

      let y = 22;

      pdf.setFillColor(229, 9, 20);
      pdf.rect(0, 0, 210, 8, "F");

      if (company.logo) {
        try {
          pdf.addImage(company.logo, "PNG", 15, 12, 27, 18);
        } catch (error) {
          console.warn("Logo da empresa não pôde ser carregada.");
        }
      }

      if (client?.logo) {
        try {
          pdf.addImage(client.logo, "PNG", 168, 12, 27, 18);
        } catch (error) {
          console.warn("Logo do cliente não pôde ser carregada.");
        }
      }

      pdf.setTextColor(0, 0, 0);
      pdf.setFontSize(16);
      pdf.text(company.name || "Empresa", 48, y);

      pdf.setFontSize(8);
      pdf.text(
        [
          company.document,
          company.phone,
          company.email,
          company.address
        ].filter(Boolean).join(" · ").slice(0, 110),
        48,
        y + 6
      );

      y += 28;

      pdf.setFontSize(15);
      pdf.text("PEDIDO COMERCIAL", 15, y);

      y += 11;
      pdf.setFontSize(10);

      const clientLines = [
        "Cliente: " + (client?.name || "—"),
        "CPF/CNPJ: " + (client?.document || "—"),
        "Telefone: " + (client?.phone || "—"),
        "E-mail: " + (client?.email || "—"),
        "Endereço: " + (client?.address || "—"),
        "Data: " + dateBR(sale.date),
        "Vendedor: " + (seller?.name || "—"),
        "Canal: " + (sale.channel || "—")
      ];

      clientLines.forEach(function(line) {
        pdf.text(line.slice(0, 120), 15, y);
        y += 6;
      });

      y += 6;

      pdf.setFillColor(40, 40, 40);
      pdf.setTextColor(255, 255, 255);
      pdf.rect(15, y - 5, 180, 8, "F");

      pdf.setFontSize(8);
      pdf.text("Fornecedor", 17, y);
      pdf.text("SKU", 55, y);
      pdf.text("Produto", 82, y);
      pdf.text("Qtd.", 140, y);
      pdf.text("Unitário", 153, y);
      pdf.text("Total", 177, y);

      y += 9;
      pdf.setTextColor(0, 0, 0);

      sale.items.forEach(function(item) {
        const product = findProduct(item.productId);
        const supplier = findSupplier(item.supplierId);

        pdf.text((supplier?.name || "—").slice(0, 18), 17, y);
        pdf.text((item.sku || "—").slice(0, 14), 55, y);
        pdf.text((product?.name || "Produto removido").slice(0, 30), 82, y);
        pdf.text(String(item.quantity), 142, y);
        pdf.text(money(item.price), 153, y);
        pdf.text(money(item.price * item.quantity), 177, y);

        y += 7;

        if (y > 270) {
          pdf.addPage();
          y = 20;
        }
      });

      y += 10;
      pdf.setFontSize(13);
      pdf.text("TOTAL: " + money(totalSale(sale)), 145, y);

      if (sale.notes) {
        y += 14;
        pdf.setFontSize(9);
        pdf.text("Observações:", 15, y);
        y += 6;
        pdf.text(pdf.splitTextToSize(sale.notes, 175), 15, y);
      }

      pdf.setFontSize(8);
      pdf.text(
        "Documento gerado pelo sistema de Gestão Comercial.",
        15,
        285
      );

      pdf.save(
        "pedido-" +
        (client?.name || "cliente").replace(/[^a-z0-9]/gi, "-") +
        "-" +
        sale.date +
        ".pdf"
      );
    }

    document.getElementById("company-form").addEventListener("submit", function(event) {
      event.preventDefault();

      db.company = {
        name: document.getElementById("company-name").value.trim(),
        document: document.getElementById("company-document").value.trim(),
        phone: document.getElementById("company-phone").value.trim(),
        email: document.getElementById("company-email").value.trim(),
        logo: document.getElementById("company-logo").value.trim(),
        address: document.getElementById("company-address").value.trim()
      };

      saveDB();
      alert("Dados da empresa salvos.");
    });

    function loadCompanyForm() {
      document.getElementById("company-name").value = db.company.name || "";
      document.getElementById("company-document").value =
        db.company.document || "";
      document.getElementById("company-phone").value =
        db.company.phone || "";
      document.getElementById("company-email").value =
        db.company.email || "";
      document.getElementById("company-logo").value =
        db.company.logo || "";
      document.getElementById("company-address").value =
        db.company.address || "";
    }

    document.getElementById("goal-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const monthly = Number(
        document.getElementById("monthly-goal").value || 0
      );

      const days = Number(
        document.getElementById("goal-days").value || 30
      );

      db.settings.monthlyGoal = monthly;
      db.settings.goalDays = days;
      db.settings.dailyGoal = monthly / Math.max(days, 1);

      saveDB();
      closeModal("goal-modal");
      renderDashboard();

      alert("Meta salva com sucesso.");
    });

    function calculateDailyGoal() {
      const monthly = Number(
        document.getElementById("monthly-goal").value || 0
      );

      const days = Number(
        document.getElementById("goal-days").value || 30
      );

      document.getElementById("daily-goal").value =
        (monthly / Math.max(days, 1)).toFixed(2);
    }

    document.getElementById("monthly-goal").addEventListener(
      "input",
      calculateDailyGoal
    );

    document.getElementById("goal-days").addEventListener(
      "input",
      calculateDailyGoal
    );

    function openGoalModal() {
      document.getElementById("monthly-goal").value =
        db.settings.monthlyGoal || "";

      document.getElementById("goal-days").value =
        db.settings.goalDays || 30;

      calculateDailyGoal();
      document.getElementById("goal-modal").classList.add("open");
    }

    function closeModal(modalId) {
      document.getElementById(modalId).classList.remove("open");
    }

    document.querySelectorAll(".modal").forEach(function(modal) {
      modal.addEventListener("click", function(event) {
        if (event.target === modal) {
          modal.classList.remove("open");
        }
      });
    });

    function showPage(page) {
      document.querySelectorAll(".page").forEach(function(section) {
        section.classList.remove("active");
      });

      document.querySelectorAll(".menu-button").forEach(function(button) {
        button.classList.remove("active");
      });

      const pageElement = document.getElementById("page-" + page);

      if (pageElement) {
        pageElement.classList.add("active");
      }

      const menuButton = document.querySelector(
        '.menu-button[data-page="' + page + '"]'
      );

      if (menuButton) {
        menuButton.classList.add("active");
      }

      const titles = {
        dashboard: "Dashboard",
        clientes: "Clientes",
        produtos: "Produtos",
        fornecedores: "Fornecedores",
        vendedores: "Vendedores",
        financeiro: "Financeiro",
        abc: "Curva ABC",
        configuracoes: "Configurações",
        perfil: "Perfil do cliente"
      };

      document.getElementById("page-title").textContent =
        titles[page] || "Gestão Comercial";

      window.scrollTo(0, 0);
    }

    document.querySelectorAll(".menu-button").forEach(function(button) {
      button.addEventListener("click", function() {
        showPage(button.dataset.page);
        renderAll();
      });
    });

    function renderAll() {
      populateGeneralSelects();
      renderDashboard();
      renderClients();
      renderProducts();
      renderSuppliers();
      renderSellers();
      renderFinance();
      renderABC();
      loadCompanyForm();
    }

    renderComparisonBoxes();
    loadCompanyForm();
    renderAll();
  </script>
</body>
</html>
