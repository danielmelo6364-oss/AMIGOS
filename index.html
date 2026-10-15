<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gestão Comercial</title>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>

  <style>
    :root {
      --bg: #080808;
      --panel: #121212;
      --panel2: #1d1d1d;
      --border: #383838;
      --white: #fff;
      --muted: #aaa;
      --red: #e50914;
      --green: #2dcc83;
      --yellow: #f4c542;
      --blue: #4098f0;
      --purple: #a978ff;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      color: var(--white);
      background: var(--bg);
      font-family: Arial, Helvetica, sans-serif;
    }

    button,
    input,
    select,
    textarea {
      font: inherit;
    }

    button,
    a {
      cursor: pointer;
    }

    button {
      color: white;
    }

    a {
      color: white;
      text-decoration: none;
    }

    .layout {
      min-height: 100vh;
    }

    .sidebar {
      position: fixed;
      inset: 0 auto 0 0;
      z-index: 10;
      width: 240px;
      padding: 20px 12px;
      overflow-y: auto;
      background: #050505;
      border-right: 1px solid var(--border);
    }

    .logo {
      margin: 0 10px 25px;
      color: var(--red);
      font-size: 23px;
      font-weight: bold;
    }

    .logo small {
      display: block;
      margin-top: 4px;
      color: var(--muted);
      font-size: 10px;
      font-weight: normal;
      letter-spacing: 1px;
    }

    .nav {
      display: block;
      width: 100%;
      margin: 3px 0;
      padding: 12px;
      border: 0;
      border-radius: 6px;
      background: transparent;
      color: #bbb;
      text-align: left;
    }

    .nav:hover,
    .nav.active {
      background: var(--red);
      color: white;
    }

    .main {
      width: calc(100% - 240px);
      min-height: 100vh;
      margin-left: 240px;
      padding: 25px;
    }

    .topbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 15px;
      margin-bottom: 24px;
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
      color: var(--muted);
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
      padding: 17px;
      border: 1px solid var(--border);
      border-radius: 8px;
      background: var(--panel);
    }

    .panel {
      margin-bottom: 15px;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 14px;
      margin-bottom: 15px;
    }

    .metric-label {
      color: var(--muted);
      font-size: 11px;
      letter-spacing: .5px;
      text-transform: uppercase;
    }

    .metric-value {
      margin-top: 9px;
      font-size: 25px;
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
      background: var(--panel2);
    }

    .button:hover {
      filter: brightness(1.25);
    }

    .button.primary {
      border-color: var(--red);
      background: var(--red);
    }

    .button.success {
      border-color: #19724e;
      background: #095e3c;
    }

    .button.danger {
      border-color: #8f151c;
      background: #4d0c11;
    }

    .button.small {
      padding: 6px 9px;
      font-size: 12px;
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
      padding: 10px 8px;
      border-bottom: 1px solid var(--border);
      text-align: left;
      vertical-align: middle;
      font-size: 13px;
    }

    th {
      color: var(--muted);
      font-size: 11px;
      text-transform: uppercase;
    }

    tr.clickable {
      cursor: pointer;
    }

    tr.clickable:hover {
      background: #242424;
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
      padding: 22px 10px;
      color: var(--muted);
      text-align: center;
      font-size: 13px;
    }

    .alert {
      margin-bottom: 14px;
      padding: 12px;
      border-left: 4px solid var(--yellow);
      border-radius: 5px;
      background: #261f08;
      color: #f4d97b;
      font-size: 13px;
    }

    .alert.red-alert {
      border-left-color: var(--red);
      background: #2a0a0d;
      color: #ffafb4;
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
      background: linear-gradient(90deg, var(--red), #ff4851);
    }

    .badge {
      display: inline-flex;
      align-items: center;
      padding: 4px 8px;
      border-radius: 20px;
      font-size: 11px;
      white-space: nowrap;
    }

    .badge-a {
      background: #691019;
      color: #ff9aa0;
    }

    .badge-b {
      background: #62500c;
      color: #ffdf65;
    }

    .badge-c {
      background: #104b76;
      color: #83c4ff;
    }

    .badge-active {
      background: #075b3b;
      color: #7df0bd;
    }

    .badge-inactive {
      background: #571018;
      color: #ff969c;
    }

    .chips {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
    }

    .chip {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      padding: 5px 8px;
      border: 1px solid #444;
      border-radius: 20px;
      background: #282828;
      font-size: 11px;
    }

    .chip.inactive {
      background: #171717;
      color: #777;
    }

    .dot {
      display: inline-block;
      width: 9px;
      height: 9px;
      border-radius: 50%;
    }

    .sale-line {
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

    .filter-row {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 10px;
      margin-bottom: 10px;
    }

    .comparison-card {
      border-left: 4px solid var(--blue);
    }

    .comparison-card.current {
      border-left-color: var(--green);
    }

    .comparison-card.previous {
      border-left-color: var(--yellow);
    }

    .abc-row-a {
      border-left: 5px solid var(--red);
      background: rgba(229, 9, 20, .13);
    }

    .abc-row-b {
      border-left: 5px solid var(--yellow);
      background: rgba(244, 197, 66, .12);
    }

    .abc-row-c {
      border-left: 5px solid var(--blue);
      background: rgba(64, 152, 240, .12);
    }

    .modal {
      position: fixed;
      z-index: 30;
      inset: 0;
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      background: rgba(0, 0, 0, .8);
    }

    .modal.open {
      display: flex;
    }

    .modal-content {
      width: min(1050px, 100%);
      max-height: 92vh;
      overflow-y: auto;
      padding: 20px;
      border: 1px solid #444;
      border-top: 3px solid var(--red);
      border-radius: 8px;
      background: var(--panel);
    }

    .modal-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 17px;
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
      margin-bottom: 18px;
    }

    .profile-columns {
      display: grid;
      grid-template-columns: 1.1fr .9fr;
      gap: 15px;
    }

    @media (max-width: 1100px) {
      .cards {
        grid-template-columns: repeat(2, 1fr);
      }

      .grid-4 {
        grid-template-columns: repeat(2, 1fr);
      }

      .profile-columns {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 760px) {
      .sidebar {
        position: sticky;
        top: 0;
        inset: auto;
        display: flex;
        align-items: center;
        gap: 6px;
        width: 100%;
        padding: 8px;
        overflow-x: auto;
        overflow-y: hidden;
        border-right: 0;
        border-bottom: 1px solid var(--border);
      }

      .logo {
        display: none;
      }

      .nav {
        flex: 0 0 auto;
        width: auto;
        margin: 0;
        padding: 10px 14px;
        white-space: nowrap;
        font-size: 13px;
      }

      .main {
        width: 100%;
        margin-left: 0;
        padding: 15px;
      }

      .topbar {
        flex-direction: column;
        align-items: flex-start;
      }

      .grid-2,
      .grid-3,
      .grid-4,
      .filter-row {
        grid-template-columns: 1fr;
      }

      .cards {
        grid-template-columns: 1fr 1fr;
        gap: 8px;
      }

      .metric-value {
        font-size: 20px;
      }

      .sale-line {
        grid-template-columns: 1fr 1fr 40px;
      }

      .sale-line .supplier-field,
      .sale-line .product-field {
        grid-column: 1 / -1;
      }

      .profile-header {
        flex-direction: column;
      }
    }
  </style>
</head>

<body>
  <div class="layout">
    <aside class="sidebar">
      <div class="logo">
        GESTÃO
        <small>representação comercial</small>
      </div>

      <button class="nav active" data-page="dashboard">Dashboard</button>
      <button class="nav" data-page="clientes">Clientes</button>
      <button class="nav" data-page="produtos">Produtos</button>
      <button class="nav" data-page="fornecedores">Fornecedores</button>
      <button class="nav" data-page="vendedores">Vendedores</button>
      <button class="nav" data-page="financeiro">Financeiro</button>
      <button class="nav" data-page="abc">Curva ABC</button>
      <button class="nav" data-page="configuracoes">Configurações</button>
    </aside>

    <main class="main">
      <div class="topbar">
        <div>
          <h1 id="page-title">Dashboard</h1>
          <div class="muted">Gestão comercial, metas e análises</div>
        </div>

        <button class="button primary" onclick="openSaleModal()">
          + Nova venda
        </button>
      </div>

      <!-- DASHBOARD -->
      <section class="page active" id="page-dashboard">
        <div class="panel">
          <div class="toolbar">
            <div>
              <h2>Filtros e comparação de períodos</h2>
              <div class="muted">
                Escolha um período principal e adicione períodos para comparar.
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

          <div class="filter-row">
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
              <label>Atalho</label>
              <select id="filter-shortcut" onchange="applyShortcut()">
                <option value="">Selecionar período</option>
                <option value="today">Hoje</option>
                <option value="7">Últimos 7 dias</option>
                <option value="30">Últimos 30 dias</option>
                <option value="90">Últimos 90 dias</option>
                <option value="current-month">Mês atual</option>
                <option value="previous-month">Mês anterior</option>
                <option value="current-year">Ano atual</option>
              </select>
            </div>
          </div>

          <div id="comparison-filters"></div>

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
            <div class="metric-value green" id="dashboard-revenue">R$ 0,00</div>
          </div>

          <div class="card">
            <div class="metric-label">Pedidos filtrados</div>
            <div class="metric-value" id="dashboard-orders">0</div>
          </div>

          <div class="card">
            <div class="metric-label">Clientes alcançados</div>
            <div class="metric-value blue" id="dashboard-clients">0</div>
          </div>

          <div class="card">
            <div class="metric-label">Ticket médio</div>
            <div class="metric-value yellow" id="dashboard-ticket">R$ 0,00</div>
          </div>
        </div>

        <div class="panel">
          <h2>Comparação de períodos</h2>
          <div id="comparison-results" class="grid-3"></div>
        </div>

        <div class="panel">
          <h2>Meta de vendas</h2>

          <div class="cards">
            <div class="card">
              <div class="metric-label">Meta mensal</div>
              <div class="metric-value" id="goal-month">R$ 0,00</div>
            </div>

            <div class="card">
              <div class="metric-label">Meta diária</div>
              <div class="metric-value yellow" id="goal-daily">R$ 0,00</div>
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

          <div class="muted" id="goal-summary" style="margin-top:9px"></div>
        </div>

        <div class="grid-2">
          <div class="panel">
            <h2>Aniversariantes</h2>
            <div id="birthdays-list"></div>
          </div>

          <div class="panel">
            <h2>Oportunidades de expansão</h2>
            <div id="expansion-list"></div>
          </div>
        </div>

        <div class="grid-2">
          <div class="panel">
            <h2>Clientes inativos</h2>
            <div id="inactive-list"></div>
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
                <label>Empresa / CNPJ</label>
                <input id="client-document">
              </div>

              <div class="field">
                <label>Logo do cliente — URL</label>
                <input id="client-logo" placeholder="https://...">
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
            <input id="client-search" placeholder="Buscar cliente..." oninput="renderClients()">
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
            </div>

            <div class="actions">
              <button class="button primary">Salvar produto</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <div class="toolbar">
            <h2>Produtos cadastrados</h2>
            <input id="product-search" placeholder="Buscar produto ou SKU..." oninput="renderProducts()">
          </div>

          <div class="table-wrap">
            <table>
              <thead>
                <tr>
                  <th>SKU</th>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Preço</th>
                  <th>Curva</th>
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
                <label>Cor</label>
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
            <div class="grid-3">
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
                <label>Meta mensal individual</label>
                <input id="seller-goal" type="number" min="0" step="0.01" value="0">
              </div>

              <div class="field">
                <label>Status</label>
                <select id="seller-status">
                  <option value="ativo">Ativo</option>
                  <option value="inativo">Inativo</option>
                </select>
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
                  <th>Status</th>
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
              <h2>Curva ABC</h2>
              <div class="muted">
                A = até 60% · B = 60% a 90% · C = acima de 90%.
              </div>
            </div>

            <select id="abc-period" onchange="renderABC()">
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
                  <th>Posição</th>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Curva</th>
                  <th>Quantidade</th>
                  <th>Faturamento</th>
                  <th>% individual</th>
                  <th>% acumulado</th>
                  <th>Clientes</th>
                </tr>
              </thead>
              <tbody id="abc-products-table"></tbody>
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
                  <th>% acumulado</th>
                  <th>Ação</th>
                </tr>
              </thead>
              <tbody id="abc-clients-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- CONFIGURAÇÕES -->
      <section class="page" id="page-configuracoes">
        <div class="panel">
          <h2>Dados da empresa para o PDF</h2>

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
                <label>Logo da empresa — URL</label>
                <input id="company-logo" placeholder="https://...">
              </div>

              <div class="field full">
                <label>Endereço da empresa</label>
                <input id="company-address">
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar dados da empresa</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <h2>Como usar as logos no PDF</h2>

          <div class="muted">
            Informe uma URL pública de imagem, por exemplo:
            https://seusite.com/logo.png
          </div>

          <div class="alert" style="margin-top:14px">
            Para o PDF carregar corretamente a logo, a imagem precisa permitir
            acesso externo e estar em formato JPG, PNG ou base64.
          </div>
        </div>
      </section>

      <!-- PERFIL -->
      <section class="page" id="page-profile">
        <div id="client-profile"></div>
      </section>
    </main>
  </div>

  <!-- MODAL DE META -->
  <div class="modal" id="settings-modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2>Configurar meta</h2>
        <button class="close" onclick="closeModal('settings-modal')">×</button>
      </div>

      <form id="settings-form">
        <div class="grid-3">
          <div class="field">
            <label>Meta mensal *</label>
            <input id="monthly-goal" type="number" min="0" step="0.01" required>
          </div>

          <div class="field">
            <label>Dias considerados *</label>
            <input id="considered-days" type="number" min="1" max="31" value="30" required>
          </div>

          <div class="field">
            <label>Meta diária calculada</label>
            <input id="daily-goal" type="number" readonly>
          </div>
        </div>

        <div class="actions">
          <button class="button primary">Salvar meta</button>
        </div>
      </form>
    </div>
  </div>

  <!-- MODAL VENDA -->
  <div class="modal" id="sale-modal">
    <div class="modal-content">
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

        <h3 style="margin-top:20px">Itens</h3>

        <div class="alert">
          Selecione o fornecedor antes do produto.
          O sistema exibirá os produtos vinculados ao fornecedor.
        </div>

        <div id="sale-lines"></div>

        <button type="button" class="button small" onclick="addSaleLine()">
          + Adicionar item
        </button>

        <div class="field" style="margin-top:15px">
          <label>Observações</label>
          <textarea id="sale-notes"></textarea>
        </div>

        <div style="margin-top:15px;text-align:right;font-size:19px">
          Total:
          <strong class="green" id="sale-total">R$ 0,00</strong>
        </div>

        <div class="actions">
          <button class="button primary">Salvar venda</button>
        </div>
      </form>
    </div>
  </div>

  <!-- MODAL PEDIDO -->
  <div class="modal" id="order-modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2>Detalhes do pedido</h2>
        <button class="close" onclick="closeModal('order-modal')">×</button>
      </div>

      <div id="order-details"></div>
    </div>
  </div>

  <script>
    const STORAGE_KEY = "gestao_comercial_completo_comparacoes_pdf_v1";

    let database = loadDatabase();
    let comparisons = [];

    function loadDatabase() {
      let data = null;

      try {
        data = JSON.parse(localStorage.getItem(STORAGE_KEY));
      } catch (error) {
        data = null;
      }

      if (!data || typeof data !== "object") {
        data = {
          settings: {
            monthlyGoal: 0,
            dailyGoal: 0,
            consideredDays: 30
          },
          company: {
            name: "",
            document: "",
            phone: "",
            email: "",
            address: "",
            logo: ""
          },
          clients: [],
          suppliers: [],
          sellers: [],
          products: [],
          sales: [],
          finances: [],
          lowerReasons: []
        };
      }

      data.settings = data.settings || {};
      data.company = data.company || {};

      data.settings.monthlyGoal = Number(data.settings.monthlyGoal || 0);
      data.settings.dailyGoal = Number(data.settings.dailyGoal || 0);
      data.settings.consideredDays = Number(data.settings.consideredDays || 30);

      const arrays = [
        "clients",
        "suppliers",
        "sellers",
        "products",
        "sales",
        "finances",
        "lowerReasons"
      ];

      arrays.forEach(function(key) {
        if (!Array.isArray(data[key])) {
          data[key] = [];
        }
      });

      return data;
    }

    function saveDatabase() {
      try {
        localStorage.setItem(STORAGE_KEY, JSON.stringify(database));
      } catch (error) {
        alert("Não foi possível salvar os dados no navegador.");
      }
    }

    function createId(prefix) {
      return prefix + "_" + Date.now().toString(36) +
        Math.random().toString(36).substring(2, 8);
    }

    function today() {
      const date = new Date();
      const month = String(date.getMonth() + 1).padStart(2, "0");
      const day = String(date.getDate()).padStart(2, "0");

      return date.getFullYear() + "-" + month + "-" + day;
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

    function escapeHTML(value) {
      return String(value ?? "").replace(/[&<>"']/g, function(character) {
        return {
          "&": "&",
          "<": "<",
          ">": ">",
          '"': "&quot;",
          "'": "&#039;"
        }[character];
      });
    }

    function getClient(id) {
      return database.clients.find(item => item.id === id);
    }

    function getSupplier(id) {
      return database.suppliers.find(item => item.id === id);
    }

    function getSeller(id) {
      return database.sellers.find(item => item.id === id);
    }

    function getProduct(id) {
      return database.products.find(item => item.id === id);
    }

    function saleTotal(sale) {
      return (sale.items || []).reduce(function(total, item) {
        return total + Number(item.quantity || 0) * Number(item.price || 0);
      }, 0);
    }

    function getMonthSales() {
      const month = today().substring(0, 7);

      return database.sales.filter(function(sale) {
        return String(sale.date).substring(0, 7) === month;
      });
    }

    function getProductQuantity(productId, sales) {
      return (sales || database.sales).reduce(function(total, sale) {
        return total + (sale.items || []).reduce(function(sum, item) {
          return sum + (
            item.productId === productId
              ? Number(item.quantity || 0)
              : 0
          );
        }, 0);
      }, 0);
    }

    function getProductRevenue(productId, sales) {
      return (sales || database.sales).reduce(function(total, sale) {
        return total + (sale.items || []).reduce(function(sum, item) {
          return sum + (
            item.productId === productId
              ? Number(item.quantity || 0) * Number(item.price || 0)
              : 0
          );
        }, 0);
      }, 0);
    }

    function getClientStats(clientId, sales) {
      const source = sales || database.sales;
      const selected = source.filter(sale => sale.clientId === clientId);
      const quantities = {};
      let revenue = 0;
      let items = 0;

      selected.forEach(function(sale) {
        revenue += saleTotal(sale);

        (sale.items || []).forEach(function(item) {
          quantities[item.productId] =
            (quantities[item.productId] || 0) +
            Number(item.quantity || 0);

          items += Number(item.quantity || 0);
        });
      });

      const dates = selected
        .map(sale => sale.date)
        .filter(Boolean)
        .sort()
        .reverse();

      return {
        sales: selected,
        quantities: quantities,
        revenue: revenue,
        items: items,
        lastSale: dates[0] || ""
      };
    }

    function getDaysWithoutPurchase(client) {
      const stats = getClientStats(client.id);

      if (!stats.lastSale) return Infinity;

      const date = new Date(stats.lastSale + "T12:00:00");

      return Math.floor((new Date() - date) / 86400000);
    }

    function supplierChip(supplier, active) {
      if (!supplier) return "";

      return `
        <span class="chip ${active === false ? "inactive" : ""}">
          <span
            class="dot"
            style="background:${active === false ? "#555" : supplier.color}">
          </span>
          ${escapeHTML(supplier.name)}
        </span>
      `;
    }

    function abcBadge(curve) {
      return `
        <span class="badge badge-${String(curve).toLowerCase()}">
          Curva ${curve}
        </span>
      `;
    }

    function calculateABC(rows) {
      const sorted = rows.slice().sort(function(a, b) {
        return Number(b.revenue || 0) - Number(a.revenue || 0);
      });

      const total = sorted.reduce(function(sum, row) {
        return sum + Number(row.revenue || 0);
      }, 0);

      let accumulated = 0;

      return sorted.map(function(row, index) {
        const revenue = Number(row.revenue || 0);

        if (total <= 0 || revenue <= 0) {
          return {
            row: row,
            index: index + 1,
            individual: 0,
            accumulated: accumulated,
            curve: "C"
          };
        }

        const previous = accumulated;
        const individual = revenue / total * 100;

        accumulated += individual;

        let curve = "C";

        if (previous < 60) {
          curve = "A";
        } else if (previous < 90) {
          curve = "B";
        }

        return {
          row: row,
          index: index + 1,
          individual: individual,
          accumulated: accumulated,
          curve: curve
        };
      });
    }

    function getFilteredSales(filters) {
      return database.sales.filter(function(sale) {
        const date = String(sale.date || "");

        if (filters.start && date < filters.start) return false;
        if (filters.end && date > filters.end) return false;

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
          const validItem = (sale.items || []).some(function(item) {
            const supplierOk = !filters.supplier ||
              item.supplierId === filters.supplier;

            const productOk = !filters.product ||
              item.productId === filters.product;

            return supplierOk && productOk;
          });

          if (!validItem) return false;
        }

        return true;
      });
    }

    function readFilters(prefix) {
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

    function fillFilterSelects(prefix) {
      const client = document.getElementById(prefix + "client");
      const seller = document.getElementById(prefix + "seller");
      const supplier = document.getElementById(prefix + "supplier");
      const product = document.getElementById(prefix + "product");
      const channel = document.getElementById(prefix + "channel");

      if (!client) return;

      const values = {
        client: client.value,
        seller: seller.value,
        supplier: supplier.value,
        product: product.value,
        channel: channel.value
      };

      client.innerHTML =
        `<option value="">Todos os clientes</option>` +
        database.clients.map(item => `
          <option value="${item.id}">
            ${escapeHTML(item.name)}
          </option>
        `).join("");

      seller.innerHTML =
        `<option value="">Todos os vendedores</option>` +
        database.sellers.map(item => `
          <option value="${item.id}">
            ${escapeHTML(item.name)}
          </option>
        `).join("");

      supplier.innerHTML =
        `<option value="">Todos os fornecedores</option>` +
        database.suppliers.map(item => `
          <option value="${item.id}">
            ${escapeHTML(item.name)}
          </option>
        `).join("");

      product.innerHTML =
        `<option value="">Todos os produtos</option>` +
        database.products.map(item => `
          <option value="${item.id}">
            ${escapeHTML(item.sku)} — ${escapeHTML(item.name)}
          </option>
        `).join("");

      channel.innerHTML = `
        <option value="">Todos os canais</option>
        <option>Presencial</option>
        <option>WhatsApp</option>
        <option>Telefone</option>
        <option>Site</option>
        <option>Outro</option>
      `;

      client.value = values.client;
      seller.value = values.seller;
      supplier.value = values.supplier;
      product.value = values.product;
      channel.value = values.channel;
    }

    function renderComparisonFilters() {
      const container = document.getElementById("comparison-filters");

      container.innerHTML = comparisons.map(function(item, index) {
        return `
          <div class="panel" style="margin:8px 0;padding:12px">
            <div class="toolbar">
              <strong>Comparação ${index + 1}</strong>

              <button
                class="button small danger"
                onclick="removeComparison(${index})">
                Remover
              </button>
            </div>

            <div class="filter-row">
              <div class="field">
                <label>Data inicial</label>
                <input
                  id="compare-${index}-start"
                  type="date"
                  value="${item.start}"
                  onchange="updateComparison(${index})">
              </div>

              <div class="field">
                <label>Data final</label>
                <input
                  id="compare-${index}-end"
                  type="date"
                  value="${item.end}"
                  onchange="updateComparison(${index})">
              </div>

              <div class="field">
                <label>Cliente</label>
                <select id="compare-${index}-client" onchange="updateComparison(${index})"></select>
              </div>

              <div class="field">
                <label>Vendedor</label>
                <select id="compare-${index}-seller" onchange="updateComparison(${index})"></select>
              </div>

              <div class="field">
                <label>Fornecedor</label>
                <select id="compare-${index}-supplier" onchange="updateComparison(${index})"></select>
              </div>

              <div class="field">
                <label>Produto</label>
                <select id="compare-${index}-product" onchange="updateComparison(${index})"></select>
              </div>

              <div class="field">
                <label>Canal</label>
                <select id="compare-${index}-channel" onchange="updateComparison(${index})">
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

      comparisons.forEach(function(item, index) {
        fillComparisonSelects(index);
      });
    }

    function fillComparisonSelects(index) {
      const item = comparisons[index];

      const client = document.getElementById("compare-" + index + "-client");
      const seller = document.getElementById("compare-" + index + "-seller");
      const supplier = document.getElementById("compare-" + index + "-supplier");
      const product = document.getElementById("compare-" + index + "-product");
      const channel = document.getElementById("compare-" + index + "-channel");

      if (!client) return;

      client.innerHTML =
        `<option value="">Todos os clientes</option>` +
        database.clients.map(x => `
          <option value="${x.id}">${escapeHTML(x.name)}</option>
        `).join("");

      seller.innerHTML =
        `<option value="">Todos os vendedores</option>` +
        database.sellers.map(x => `
          <option value="${x.id}">${escapeHTML(x.name)}</option>
        `).join("");

      supplier.innerHTML =
        `<option value="">Todos os fornecedores</option>` +
        database.suppliers.map(x => `
          <option value="${x.id}">${escapeHTML(x.name)}</option>
        `).join("");

      product.innerHTML =
        `<option value="">Todos os produtos</option>` +
        database.products.map(x => `
          <option value="${x.id}">
            ${escapeHTML(x.sku)} — ${escapeHTML(x.name)}
          </option>
        `).join("");

      client.value = item.client || "";
      seller.value = item.seller || "";
      supplier.value = item.supplier || "";
      product.value = item.product || "";
      channel.value = item.channel || "";
    }

    function updateComparison(index) {
      const prefix = "compare-" + index + "-";

      comparisons[index] = {
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
      comparisons.push({
        start: "",
        end: "",
        client: "",
        seller: "",
        supplier: "",
        product: "",
        channel: ""
      });

      renderComparisonFilters();
      renderDashboard();
    }

    function removeComparison(index) {
      comparisons.splice(index, 1);
      renderComparisonFilters();
      renderDashboard();
    }

    function clearComparisons() {
      comparisons = [];
      renderComparisonFilters();
      renderDashboard();
    }

    function applyShortcut() {
      const value = document.getElementById("filter-shortcut").value;
      const start = document.getElementById("filter-start");
      const end = document.getElementById("filter-end");
      const current = new Date();

      if (!value) return;

      if (value === "today") {
        start.value = today();
        end.value = today();
      }

      if (["7", "30", "90"].includes(value)) {
        const initial = new Date();
        initial.setDate(initial.getDate() - Number(value));

        start.value = initial.toISOString().substring(0, 10);
        end.value = today();
      }

      if (value === "current-month") {
        start.value = current.getFullYear() + "-" +
          String(current.getMonth() + 1).padStart(2, "0") + "-01";

        end.value = today();
      }

      if (value === "previous-month") {
        const first = new Date(
          current.getFullYear(),
          current.getMonth() - 1,
          1
        );

        const last = new Date(
          current.getFullYear(),
          current.getMonth(),
          0
        );

        start.value = first.toISOString().substring(0, 10);
        end.value = last.toISOString().substring(0, 10);
      }

      if (value === "current-year") {
        start.value = current.getFullYear() + "-01-01";
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

        if (element) {
          element.value = "";
        }
      });

      document.getElementById("filter-shortcut").value = "";
      comparisons = [];
      renderComparisonFilters();
      renderDashboard();
    }

    function renderDashboard() {
      fillFilterSelects("filter-");

      const filters = readFilters("filter-");
      const sales = getFilteredSales(filters);
      const revenue = sales.reduce((sum, sale) => sum + saleTotal(sale), 0);
      const clients = new Set(sales.map(sale => sale.clientId)).size;
      const ticket = sales.length ? revenue / sales.length : 0;

      document.getElementById("dashboard-revenue").textContent = money(revenue);
      document.getElementById("dashboard-orders").textContent = sales.length;
      document.getElementById("dashboard-clients").textContent = clients;
      document.getElementById("dashboard-ticket").textContent = money(ticket);

      renderGoal();
      renderBirthdays();
      renderInactive();
      renderExpansion();
      renderUnusedProducts();

      const results = [];

      comparisons.forEach(function(item, index) {
        const comparisonSales = getFilteredSales(item);
        const comparisonRevenue = comparisonSales.reduce(
          (sum, sale) => sum + saleTotal(sale),
          0
        );

        results.push(`
          <div class="card comparison-card">
            <div class="metric-label">Comparação ${index + 1}</div>
            <div class="metric-value">${money(comparisonRevenue)}</div>
            <div class="muted">
              ${comparisonSales.length} pedido(s)
            </div>
          </div>
        `);
      });

      results.unshift(`
        <div class="card comparison-card current">
          <div class="metric-label">Período principal</div>
          <div class="metric-value">${money(revenue)}</div>
          <div class="muted">
            ${sales.length} pedido(s)
          </div>
        </div>
      `);

      document.getElementById("comparison-results").innerHTML =
        results.join("");

      const alerts = [];

      if (!database.settings.monthlyGoal) {
        alerts.push(`
          <div class="alert">
            Configure a meta mensal para acompanhar o desempenho.
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
            Nenhuma venda corresponde aos filtros selecionados.
          </div>
        `);
      }

      document.getElementById("dashboard-alerts").innerHTML =
        alerts.join("");
    }

    function renderGoal() {
      const monthSales = getMonthSales();
      const monthRevenue = monthSales.reduce(
        (sum, sale) => sum + saleTotal(sale),
        0
      );

      const monthlyGoal = Number(database.settings.monthlyGoal || 0);
      const days = Number(database.settings.consideredDays || 30);
      const dailyGoal = monthlyGoal / Math.max(days, 1);
      const missing = Math.max(monthlyGoal - monthRevenue, 0);
      const progress = monthlyGoal
        ? Math.min(monthRevenue / monthlyGoal * 100, 100)
        : 0;

      document.getElementById("goal-month").textContent = money(monthlyGoal);
      document.getElementById("goal-daily").textContent = money(dailyGoal);
      document.getElementById("goal-sold").textContent = money(monthRevenue);
      document.getElementById("goal-missing").textContent = money(missing);
      document.getElementById("goal-progress").style.width = progress + "%";

      document.getElementById("goal-summary").textContent =
        progress.toFixed(1) + "% da meta atingida · " +
        days + " dias considerados.";
    }

    function renderBirthdays() {
      const month = today().substring(5, 7);

      const list = database.clients.filter(function(client) {
        return client.birth &&
          client.birth.substring(5, 7) === month;
      });

      document.getElementById("birthdays-list").innerHTML =
        list.length
          ? list.map(function(client) {
              return `
                <div class="list-item">
                  <strong>${escapeHTML(client.name)}</strong>
                  <div class="muted">
                    Aniversário: dia ${client.birth.substring(8, 10)}
                  </div>
                  <div class="actions">
                    <button
                      class="button small"
                      onclick="openClientProfile('${client.id}')">
                      Ver cliente
                    </button>
                  </div>
                </div>
              `;
            }).join("")
          : `<div class="empty">Nenhum aniversariante neste mês.</div>`;
    }

    function renderInactive() {
      const list = database.clients.filter(function(client) {
        const days = getDaysWithoutPurchase(client);
        return days === Infinity || days > 15;
      });

      document.getElementById("inactive-list").innerHTML =
        list.length
          ? list.map(function(client) {
              const days = getDaysWithoutPurchase(client);

              return `
                <div class="list-item">
                  <strong>${escapeHTML(client.name)}</strong>
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

    function renderExpansion() {
      const opportunities = database.clients.filter(function(client) {
        const stats = getClientStats(client.id);
        return stats.sales.length > 0 && getSuggestions(client.id).length > 0;
      });

      document.getElementById("expansion-list").innerHTML =
        opportunities.length
          ? opportunities.slice(0, 10).map(function(client) {
              const suggestions = getSuggestions(client.id)
                .slice(0, 3)
                .map(item => item.product.name)
                .join(", ");

              return `
                <div class="list-item">
                  <strong>${escapeHTML(client.name)}</strong>
                  <div class="muted">
                    Sugestões: ${escapeHTML(suggestions)}
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
          : `<div class="empty">Nenhuma oportunidade identificada.</div>`;
    }

    function renderUnusedProducts() {
      const products = database.products.filter(function(product) {
        return getProductQuantity(product.id) === 0;
      });

      document.getElementById("unused-products").innerHTML =
        products.length
          ? products.map(function(product) {
              return `
                <div class="list-item">
                  <strong>${escapeHTML(product.name)}</strong>
                  <div class="muted">
                    SKU: ${escapeHTML(product.sku)}
                  </div>
                </div>
              `;
            }).join("")
          : `<div class="empty">Todos os produtos possuem vendas.</div>`;
    }

    document.getElementById("client-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.clients.push({
        id: createId("client"),
        name: document.getElementById("client-name").value.trim(),
        phone: document.getElementById("client-phone").value.trim(),
        email: document.getElementById("client-email").value.trim(),
        birth: document.getElementById("client-birth").value,
        document: document.getElementById("client-document").value.trim(),
        logo: document.getElementById("client-logo").value.trim(),
        address: document.getElementById("client-address").value.trim()
      });

      saveDatabase();
      event.target.reset();
      renderAll();

      alert("Cliente cadastrado com sucesso.");
    });

    function renderClients() {
      const search = (
        document.getElementById("client-search")?.value || ""
      ).toLowerCase();

      const list = database.clients.filter(function(client) {
        return client.name.toLowerCase().includes(search) ||
          (client.document || "").toLowerCase().includes(search);
      });

      document.getElementById("clients-table").innerHTML =
        list.length
          ? list.map(function(client) {
              const stats = getClientStats(client.id);
              const inactive = getDaysWithoutPurchase(client) > 15 ||
                getDaysWithoutPurchase(client) === Infinity;

              return `
                <tr
                  class="clickable"
                  onclick="openClientProfile('${client.id}')">
                  <td><strong>${escapeHTML(client.name)}</strong></td>
                  <td>${escapeHTML(client.phone || "—")}</td>
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
              <td colspan="7" class="empty">Nenhum cliente encontrado.</td>
            </tr>
          `;
    }

    function deleteClient(clientId) {
      if (!confirm("Excluir este cliente e seu histórico?")) return;

      database.clients = database.clients.filter(item => item.id !== clientId);
      database.sales = database.sales.filter(item => item.clientId !== clientId);

      saveDatabase();
      renderAll();
    }

    document.getElementById("supplier-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.suppliers.push({
        id: createId("supplier"),
        name: document.getElementById("supplier-name").value.trim(),
        contact: document.getElementById("supplier-contact").value.trim(),
        color: document.getElementById("supplier-color").value
      });

      saveDatabase();
      event.target.reset();
      renderAll();

      alert("Fornecedor cadastrado.");
    });

    function renderSuppliers() {
      document.getElementById("suppliers-table").innerHTML =
        database.suppliers.length
          ? database.suppliers.map(function(supplier) {
              const products = database.products.filter(
                product => product.supplierId === supplier.id
              );

              return `
                <tr>
                  <td>${supplierChip(supplier, true)}</td>
                  <td>${escapeHTML(supplier.contact || "—")}</td>
                  <td>
                    ${
                      products.length
                        ? products.map(product => `
                            <div class="muted">
                              ${escapeHTML(product.sku)} —
                              ${escapeHTML(product.name)}
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
              <td colspan="4" class="empty">Nenhum fornecedor cadastrado.</td>
            </tr>
          `;
    }

    function deleteSupplier(id) {
      if (database.products.some(product => product.supplierId === id)) {
        alert("Este fornecedor possui produtos vinculados.");
        return;
      }

      database.suppliers = database.suppliers.filter(item => item.id !== id);
      saveDatabase();
      renderAll();
    }

    document.getElementById("product-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const sku = document.getElementById("product-sku").value.trim().toUpperCase();

      if (database.products.some(product => product.sku === sku)) {
        alert("Este SKU já está cadastrado.");
        return;
      }

      database.products.push({
        id: createId("product"),
        sku: sku,
        name: document.getElementById("product-name").value.trim(),
        supplierId: document.getElementById("product-supplier").value,
        price: Number(document.getElementById("product-price").value || 0),
        category: document.getElementById("product-category").value.trim(),
        warrantyDays: Number(document.getElementById("product-warranty").value || 0)
      });

      saveDatabase();
      event.target.reset();
      renderAll();

      alert("Produto cadastrado.");
    });

    function renderProducts() {
      const search = (
        document.getElementById("product-search")?.value || ""
      ).toLowerCase();

      const abc = calculateABC(database.products.map(function(product) {
        return {
          product: product,
          revenue: getProductRevenue(product.id)
        };
      }));

      const list = database.products.filter(function(product) {
        return product.name.toLowerCase().includes(search) ||
          product.sku.toLowerCase().includes(search);
      });

      document.getElementById("products-table").innerHTML =
        list.length
          ? list.map(function(product) {
              const classification = abc.find(item =>
                item.row.product.id === product.id
              );

              const curve = classification ? classification.curve : "C";
              const supplier = getSupplier(product.supplierId);

              return `
                <tr class="abc-row-${curve.toLowerCase()}">
                  <td>${escapeHTML(product.sku)}</td>
                  <td>${escapeHTML(product.name)}</td>
                  <td>${supplier ? supplierChip(supplier, true) : "—"}</td>
                  <td>${money(product.price)}</td>
                  <td>${abcBadge(curve)}</td>
                  <td>${getProductQuantity(product.id)}</td>
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
              <td colspan="7" class="empty">Nenhum produto encontrado.</td>
            </tr>
          `;
    }

    function deleteProduct(id) {
      if (database.sales.some(sale =>
        sale.items.some(item => item.productId === id)
      )) {
        alert("Este produto possui histórico de vendas.");
        return;
      }

      database.products = database.products.filter(item => item.id !== id);
      saveDatabase();
      renderAll();
    }

    document.getElementById("seller-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.sellers.push({
        id: createId("seller"),
        name: document.getElementById("seller-name").value.trim(),
        phone: document.getElementById("seller-phone").value.trim(),
        email: document.getElementById("seller-email").value.trim(),
        goal: Number(document.getElementById("seller-goal").value || 0),
        status: document.getElementById("seller-status").value
      });

      saveDatabase();
      event.target.reset();
      renderAll();

      alert("Vendedor cadastrado.");
    });

    function renderSellers() {
      document.getElementById("sellers-table").innerHTML =
        database.sellers.length
          ? database.sellers.map(function(seller) {
              const revenue = database.sales
                .filter(sale => sale.sellerId === seller.id)
                .reduce((sum, sale) => sum + saleTotal(sale), 0);

              return `
                <tr>
                  <td>${escapeHTML(seller.name)}</td>
                  <td>${escapeHTML(seller.phone || "—")}</td>
                  <td>${money(seller.goal)}</td>
                  <td class="green">${money(revenue)}</td>
                  <td>
                    <span class="badge ${
                      seller.status === "ativo"
                        ? "badge-active"
                        : "badge-inactive"
                    }">
                      ${seller.status}
                    </span>
                  </td>
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
              <td colspan="6" class="empty">Nenhum vendedor cadastrado.</td>
            </tr>
          `;
    }

    function deleteSeller(id) {
      if (database.sales.some(sale => sale.sellerId === id)) {
        alert("Este vendedor possui vendas registradas.");
        return;
      }

      database.sellers = database.sellers.filter(item => item.id !== id);
      saveDatabase();
      renderAll();
    }

    function updateSelects() {
      const supplier = document.getElementById("product-supplier");
      const client = document.getElementById("sale-client");
      const seller = document.getElementById("sale-seller");

      if (supplier) {
        supplier.innerHTML =
          `<option value="">Selecione...</option>` +
          database.suppliers.map(item => `
            <option value="${item.id}">${escapeHTML(item.name)}</option>
          `).join("");
      }

      if (client) {
        client.innerHTML =
          `<option value="">Selecione...</option>` +
          database.clients.map(item => `
            <option value="${item.id}">${escapeHTML(item.name)}</option>
          `).join("");
      }

      if (seller) {
        seller.innerHTML =
          `<option value="">Selecione...</option>` +
          database.sellers
            .filter(item => item.status !== "inativo")
            .map(item => `
              <option value="${item.id}">
                ${escapeHTML(item.name)}
              </option>
            `).join("");
      }

      fillFilterSelects("filter-");
    }

    function calculateDailyGoal() {
      const monthly = Number(
        document.getElementById("monthly-goal").value || 0
      );

      const days = Number(
        document.getElementById("considered-days").value || 1
      );

      document.getElementById("daily-goal").value =
        (monthly / Math.max(days, 1)).toFixed(2);
    }

    document.getElementById("monthly-goal").addEventListener(
      "input",
      calculateDailyGoal
    );

    document.getElementById("considered-days").addEventListener(
      "input",
      calculateDailyGoal
    );

    document.getElementById("settings-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const monthly = Number(
        document.getElementById("monthly-goal").value || 0
      );

      const days = Number(
        document.getElementById("considered-days").value || 1
      );

      database.settings.monthlyGoal = monthly;
      database.settings.consideredDays = days;
      database.settings.dailyGoal = monthly / Math.max(days, 1);

      saveDatabase();
      closeModal("settings-modal");
      renderAll();

      alert("Meta salva e meta diária calculada.");
    });

    function openSettingsModal() {
      document.getElementById("monthly-goal").value =
        database.settings.monthlyGoal || "";

      document.getElementById("considered-days").value =
        database.settings.consideredDays || 30;

      calculateDailyGoal();

      document.getElementById("settings-modal").classList.add("open");
    }

    function openSaleModal(clientId) {
      updateSelects();

      document.getElementById("sale-client").value = clientId || "";
      document.getElementById("sale-date").value = today();
      document.getElementById("sale-seller").value = "";
      document.getElementById("sale-notes").value = "";
      document.getElementById("sale-lines").innerHTML = "";

      addSaleLine();

      document.getElementById("sale-modal").classList.add("open");
    }

    function addSaleLine() {
      const line = document.createElement("div");

      line.className = "sale-line";

      line.innerHTML = `
        <div class="field supplier-field">
          <label>Fornecedor *</label>
          <select class="sale-supplier" onchange="updateLineProducts(this)">
            <option value="">Selecione...</option>
            ${database.suppliers.map(item => `
              <option value="${item.id}">
                ${escapeHTML(item.name)}
              </option>
            `).join("")}
          </select>
        </div>

        <div class="field product-field">
          <label>Produto / SKU *</label>
          <select class="sale-product" onchange="updateSaleTotal()" disabled>
            <option value="">Selecione o fornecedor...</option>
          </select>
        </div>

        <div class="field">
          <label>Qtd.</label>
          <input class="sale-quantity" type="number" min="1" value="1" oninput="updateSaleTotal()">
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

    function updateLineProducts(select) {
      const line = select.closest(".sale-line");
      const productSelect = line.querySelector(".sale-product");
      const supplierId = select.value;

      const products = database.products.filter(function(product) {
        return product.supplierId === supplierId;
      });

      productSelect.disabled = !supplierId;

      productSelect.innerHTML = supplierId
        ? `<option value="">Selecione...</option>` +
          products.map(product => `
            <option value="${product.id}">
              ${escapeHTML(product.sku)} — ${escapeHTML(product.name)}
              (${money(product.price)})
            </option>
          `).join("")
        : `<option value="">Selecione o fornecedor...</option>`;

      updateSaleTotal();
    }

    function updateSaleTotal() {
      let total = 0;

      document.querySelectorAll(".sale-line").forEach(function(line) {
        const product = getProduct(
          line.querySelector(".sale-product")?.value
        );

        const quantity = Number(
          line.querySelector(".sale-quantity")?.value || 0
        );

        const lineTotal = product
          ? product.price * quantity
          : 0;

        total += lineTotal;

        line.querySelector(".line-total").textContent =
          money(lineTotal);
      });

      document.getElementById("sale-total").textContent = money(total);
    }

    document.getElementById("sale-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const items = [];
      let invalid = false;

      document.querySelectorAll(".sale-line").forEach(function(line) {
        const supplierId = line.querySelector(".sale-supplier").value;
        const productId = line.querySelector(".sale-product").value;
        const quantity = Number(
          line.querySelector(".sale-quantity").value || 0
        );

        const product = getProduct(productId);

        if (!supplierId || !product || quantity <= 0) {
          invalid = true;
          return;
        }

        if (product.supplierId !== supplierId) {
          invalid = true;
          return;
        }

        items.push({
          productId: product.id,
          supplierId: supplierId,
          sku: product.sku,
          quantity: quantity,
          price: product.price
        });
      });

      if (!document.getElementById("sale-client").value) {
        alert("Selecione o cliente.");
        return;
      }

      if (!document.getElementById("sale-seller").value) {
        alert("Selecione o vendedor.");
        return;
      }

      if (invalid || !items.length) {
        alert("Preencha corretamente os itens da venda.");
        return;
      }

      database.sales.push({
        id: createId("sale"),
        clientId: document.getElementById("sale-client").value,
        sellerId: document.getElementById("sale-seller").value,
        date: document.getElementById("sale-date").value,
        channel: document.getElementById("sale-channel").value,
        notes: document.getElementById("sale-notes").value.trim(),
        items: items
      });

      saveDatabase();
      closeModal("sale-modal");
      renderAll();

      alert("Venda registrada com sucesso.");
    });

    document.getElementById("finance-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.finances.push({
        id: createId("finance"),
        type: document.getElementById("finance-type").value,
        description: document.getElementById("finance-description").value.trim(),
        value: Number(document.getElementById("finance-value").value || 0),
        due: document.getElementById("finance-due").value,
        status: document.getElementById("finance-status").value
      });

      saveDatabase();
      event.target.reset();
      renderFinance();

      alert("Movimentação registrada.");
    });

    function renderFinance() {
      let receivable = 0;
      let payable = 0;
      let received = 0;
      let paid = 0;

      database.finances.forEach(function(item) {
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

      document.getElementById("finance-receivable").textContent = money(receivable);
      document.getElementById("finance-payable").textContent = money(payable);
      document.getElementById("finance-received").textContent = money(received);
      document.getElementById("finance-result").textContent = money(received - paid);

      document.getElementById("finance-table").innerHTML =
        database.finances.length
          ? database.finances.map(function(item) {
              return `
                <tr>
                  <td>${item.type === "receber" ? "A receber" : "A pagar"}</td>
                  <td>${escapeHTML(item.description)}</td>
                  <td>${money(item.value)}</td>
                  <td>${dateBR(item.due)}</td>
                  <td>${escapeHTML(item.status)}</td>
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

    function deleteFinance(id) {
      database.finances = database.finances.filter(item => item.id !== id);
      saveDatabase();
      renderFinance();
    }

    function renderABC() {
      const sales = getABCSales();

      const products = database.products.map(function(product) {
        return {
          product: product,
          revenue: getProductRevenue(product.id, sales),
          quantity: getProductQuantity(product.id, sales),
          clients: new Set(
            sales.filter(sale =>
              sale.items.some(item => item.productId === product.id)
            ).map(sale => sale.clientId)
          ).size
        };
      });

      const productABC = calculateABC(products);

      document.getElementById("abc-products-table").innerHTML =
        productABC.length
          ? productABC.map(function(item) {
              const product = item.row.product;
              const supplier = getSupplier(product.supplierId);

              return `
                <tr class="abc-row-${item.curve.toLowerCase()}">
                  <td>${item.index}</td>
                  <td>
                    <strong>${escapeHTML(product.name)}</strong>
                    <br>
                    <span class="muted">${escapeHTML(product.sku)}</span>
                  </td>
                  <td>${supplier ? supplierChip(supplier, true) : "—"}</td>
                  <td>${abcBadge(item.curve)}</td>
                  <td>${item.row.quantity}</td>
                  <td class="green">${money(item.row.revenue)}</td>
                  <td>${item.individual.toFixed(2)}%</td>
                  <td>${item.accumulated.toFixed(2)}%</td>
                  <td>${item.row.clients}</td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="9" class="empty">
                Cadastre produtos e vendas para calcular a Curva ABC.
              </td>
            </tr>
          `;

      const clients = database.clients.map(function(client) {
        const stats = getClientStats(client.id, sales);

        return {
          client: client,
          revenue: stats.revenue,
          stats: stats
        };
      });

      const clientABC = calculateABC(clients);

      document.getElementById("abc-clients-table").innerHTML =
        clientABC.length
          ? clientABC.map(function(item) {
              return `
                <tr class="abc-row-${item.curve.toLowerCase()}">
                  <td>${escapeHTML(item.row.client.name)}</td>
                  <td>${abcBadge(item.curve)}</td>
                  <td>${item.row.stats.sales.length}</td>
                  <td class="green">${money(item.row.revenue)}</td>
                  <td>${item.accumulated.toFixed(2)}%</td>
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
                Cadastre clientes e vendas para calcular a Curva ABC.
              </td>
            </tr>
          `;
    }

    function getABCSales() {
      const period = document.getElementById("abc-period")?.value || "all";

      if (period === "all") return database.sales;

      const start = new Date();
      start.setDate(start.getDate() - Number(period));

      return database.sales.filter(function(sale) {
        return new Date(sale.date + "T12:00:00") >= start;
      });
    }

    function getSuggestions(clientId) {
      const stats = getClientStats(clientId);
      const purchased = Object.keys(stats.quantities);

      const classification = calculateABC(
        database.products.map(function(product) {
          return {
            product: product,
            revenue: getProductRevenue(product.id)
          };
        })
      );

      return classification.filter(function(item) {
        return !purchased.includes(item.row.product.id);
      });
    }

    function openClientProfile(clientId) {
      const client = getClient(clientId);

      if (!client) return;

      const stats = getClientStats(clientId);
      const suggestions = getSuggestions(clientId);

      document.getElementById("client-profile").innerHTML = `
        <div class="profile-header">
          <div>
            <button class="button small" onclick="showPage('clientes');renderAll()">
              ← Voltar
            </button>

            <h2 style="margin-top:14px">${escapeHTML(client.name)}</h2>

            <div class="muted">
              ${escapeHTML(client.phone || "Sem telefone")}
              · ${escapeHTML(client.email || "Sem e-mail")}
              · ${escapeHTML(client.document || "Sem documento")}
            </div>
          </div>

          <button class="button primary" onclick="openSaleModal('${client.id}')">
            + Nova venda
          </button>
        </div>

        <div class="cards">
          <div class="card">
            <div class="metric-label">Pedidos</div>
            <div class="metric-value">${stats.sales.length}</div>
          </div>

          <div class="card">
            <div class="metric-label">Itens</div>
            <div class="metric-value">${stats.items}</div>
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
        </div>

        <div class="profile-columns">
          <div class="panel">
            <h2>Pedidos do cliente</h2>

            <div class="list">
              ${
                stats.sales.length
                  ? stats.sales.map(function(sale) {
                      return `
                        <div class="list-item">
                          <strong>
                            ${dateBR(sale.date)} · ${money(saleTotal(sale))}
                          </strong>

                          <div class="muted">
                            Vendedor:
                            ${escapeHTML(getSeller(sale.sellerId)?.name || "—")}
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
                              PDF
                            </button>
                          </div>
                        </div>
                      `;
                    }).join("")
                  : `<div class="empty">Nenhum pedido.</div>`
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
                        <div class="list-item abc-row-${item.curve.toLowerCase()}">
                          <strong>
                            ${escapeHTML(item.row.product.name)}
                          </strong>

                          <div class="muted">
                            SKU: ${escapeHTML(item.row.product.sku)}
                            · ${abcBadge(item.curve)}
                          </div>
                        </div>
                      `;
                    }).join("")
                  : `<div class="empty">Nenhuma sugestão.</div>`
              }
            </div>
          </div>
        </div>
      `;

      showPage("profile");
    }

    function openOrder(saleId) {
      const sale = database.sales.find(item => item.id === saleId);

      if (!sale) return;

      const client = getClient(sale.clientId);
      const seller = getSeller(sale.sellerId);

      document.getElementById("order-details").innerHTML = `
        <div class="card">
          <strong>${escapeHTML(client?.name || "Cliente")}</strong>

          <div class="muted">
            ${escapeHTML(client?.phone || "Sem telefone")}
            · ${escapeHTML(client?.email || "Sem e-mail")}
          </div>

          <div class="muted" style="margin-top:6px">
            Data: ${dateBR(sale.date)}
            · Vendedor: ${escapeHTML(seller?.name || "—")}
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
              ${sale.items.map(function(item) {
                const supplier = getSupplier(item.supplierId);
                const product = getProduct(item.productId);

                return `
                  <tr>
                    <td>${supplier ? supplierChip(supplier, true) : "—"}</td>
                    <td>${escapeHTML(item.sku)}</td>
                    <td>${escapeHTML(product?.name || "Produto removido")}</td>
                    <td>${item.quantity}</td>
                    <td>${money(item.price)}</td>
                    <td class="green">${money(item.price * item.quantity)}</td>
                  </tr>
                `;
              }).join("")}
            </tbody>
          </table>
        </div>

        <div style="margin-top:16px;text-align:right;font-size:20px">
          Total:
          <strong class="green">${money(saleTotal(sale))}</strong>
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

    function openClientLogo(client) {
      return client && client.logo ? client.logo : "";
    }

    function downloadPDF(saleId) {
      const sale = database.sales.find(item => item.id === saleId);

      if (!sale) return;

      const PDF = window.jspdf?.jsPDF;

      if (!PDF) {
        alert("A biblioteca PDF não foi carregada.");
        return;
      }

      const company = database.company;
      const client = getClient(sale.clientId);
      const seller = getSeller(sale.sellerId);
      const pdf = new PDF();

      let y = 20;

      pdf.setFillColor(229, 9, 20);
      pdf.rect(0, 0, 210, 8, "F");

      if (company.logo) {
        try {
          pdf.addImage(company.logo, "PNG", 15, y - 8, 28, 18);
        } catch (error) {
          console.warn("Logo da empresa não pôde ser inserida.");
        }
      }

      if (client?.logo) {
        try {
          pdf.addImage(client.logo, "PNG", 167, y - 8, 28, 18);
        } catch (error) {
          console.warn("Logo do cliente não pôde ser inserida.");
        }
      }

      pdf.setTextColor(0, 0, 0);
      pdf.setFontSize(16);
      pdf.text(company.name || "Empresa", 48, y);

      pdf.setFontSize(8);
      pdf.text(
        [
          company.document || "",
          company.phone || "",
          company.email || "",
          company.address || ""
        ].filter(Boolean).join(" · ").substring(0, 100),
        48,
        y + 6
      );

      y += 26;

      pdf.setFontSize(15);
      pdf.text("PEDIDO COMERCIAL", 15, y);

      y += 10;
      pdf.setFontSize(10);

      pdf.text("Cliente: " + (client?.name || "—"), 15, y);
      y += 6;

      pdf.text("Documento: " + (client?.document || "—"), 15, y);
      y += 6;

      pdf.text("Telefone: " + (client?.phone || "—"), 15, y);
      y += 6;

      pdf.text("E-mail: " + (client?.email || "—"), 15, y);
      y += 6;

      pdf.text("Endereço: " + (client?.address || "—"), 15, y);
      y += 6;

      pdf.text("Data do pedido: " + dateBR(sale.date), 15, y);
      y += 6;

      pdf.text("Vendedor: " + (seller?.name || "—"), 15, y);
      y += 6;

      pdf.text("Canal: " + (sale.channel || "—"), 15, y);
      y += 12;

      pdf.setFillColor(40, 40, 40);
      pdf.setTextColor(255, 255, 255);
      pdf.rect(15, y - 5, 180, 8, "F");

      pdf.text("Fornecedor", 17, y);
      pdf.text("SKU", 55, y);
      pdf.text("Produto", 82, y);
      pdf.text("Qtd.", 140, y);
      pdf.text("Unitário", 153, y);
      pdf.text("Total", 177, y);

      y += 9;
      pdf.setTextColor(0, 0, 0);
      pdf.setFontSize(8);

      sale.items.forEach(function(item) {
        const supplier = getSupplier(item.supplierId);
        const product = getProduct(item.productId);

        pdf.text(
          (supplier?.name || "—").substring(0, 18),
          17,
          y
        );

        pdf.text(
          (item.sku || "—").substring(0, 14),
          55,
          y
        );

        pdf.text(
          (product?.name || "Produto removido").substring(0, 30),
          82,
          y
        );

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
      pdf.text("TOTAL DO PEDIDO: " + money(saleTotal(sale)), 125, y);

      y += 14;
      pdf.setFontSize(9);

      if (sale.notes) {
        pdf.text("Observações:", 15, y);
        y += 6;
        pdf.text(pdf.splitTextToSize(sale.notes, 175), 15, y);
        y += 12;
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

      database.company = {
        name: document.getElementById("company-name").value.trim(),
        document: document.getElementById("company-document").value.trim(),
        phone: document.getElementById("company-phone").value.trim(),
        email: document.getElementById("company-email").value.trim(),
        logo: document.getElementById("company-logo").value.trim(),
        address: document.getElementById("company-address").value.trim()
      };

      saveDatabase();

      alert("Dados da empresa salvos.");
    });

    function loadCompanyForm() {
      document.getElementById("company-name").value = database.company.name || "";
      document.getElementById("company-document").value = database.company.document || "";
      document.getElementById("company-phone").value = database.company.phone || "";
      document.getElementById("company-email").value = database.company.email || "";
      document.getElementById("company-logo").value = database.company.logo || "";
      document.getElementById("company-address").value = database.company.address || "";
    }

    document.getElementById("settings-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const monthly = Number(
        document.getElementById("monthly-goal").value || 0
      );

      const days = Number(
        document.getElementById("considered-days").value || 1
      );

      database.settings.monthlyGoal = monthly;
      database.settings.consideredDays = days;
      database.settings.dailyGoal = monthly / Math.max(days, 1);

      saveDatabase();
      closeModal("settings-modal");
      renderAll();

      alert("Meta salva com sucesso.");
    });

    function openSettingsModal() {
      document.getElementById("monthly-goal").value =
        database.settings.monthlyGoal || "";

      document.getElementById("considered-days").value =
        database.settings.consideredDays || 30;

      document.getElementById("daily-goal").value =
        database.settings.dailyGoal || "";

      document.getElementById("settings-modal").classList.add("open");
    }

    document.getElementById("monthly-goal").addEventListener(
      "input",
      calculateDailyGoal
    );

    document.getElementById("considered-days").addEventListener(
      "input",
      calculateDailyGoal
    );

    function calculateDailyGoal() {
      const monthly = Number(
        document.getElementById("monthly-goal").value || 0
      );

      const days = Number(
        document.getElementById("considered-days").value || 1
      );

      document.getElementById("daily-goal").value =
        (monthly / Math.max(days, 1)).toFixed(2);
    }

    function closeModal(id) {
      document.getElementById(id).classList.remove("open");
    }

    document.querySelectorAll(".modal").forEach(function(modal) {
      modal.addEventListener("click", function(event) {
        if (event.target === modal) {
          modal.classList.remove("open");
        }
      });
    });

    function showPage(page) {
      document.querySelectorAll(".page").forEach(function(item) {
        item.classList.remove("active");
      });

      document.querySelectorAll(".nav").forEach(function(item) {
        item.classList.remove("active");
      });

      document.getElementById("page-" + page)?.classList.addactive");
      document.querySelector('[data-page="' + page + '"]')?.classList.add("active");

      const titles = {
        dashboard: "Dashboard",
        clientes: "Clientes",
        produtos: "Produtos",
        fornecedores: "Fornecedores",
        vendedores: "Vendedores",
        financeiro: "Financeiro",
        abc: "Curva ABC",
        configuracoes: "Configurações",
        profile: "Perfil do cliente"
      };

      document.getElementById("page-title").textContent =
        titles[page] || "Gestão";

      window.scrollTo(0, 0);
    }

    document.querySelectorAll(".nav").forEach(function(button) {
      button.addEventListener("click", function() {
        showPage(button.dataset.page);
        renderAll();
      });
    });

    loadCompanyForm();
    renderComparisonFilters();
    updateSelects();
    renderAll();
  </script>
</body>
</html>
