<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gestão Comercial</title>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>

  <style>
    :root {
      --preto: #080808;
      --preto-2: #121212;
      --preto-3: #1d1d1d;
      --preto-4: #292929;
      --vermelho: #e50914;
      --vermelho-escuro: #7f0b11;
      --branco: #ffffff;
      --cinza: #a8a8a8;
      --borda: #363636;
      --verde: #2dcc83;
      --amarelo: #f4c542;
      --azul: #4b9cff;
      --roxo: #a676ff;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      background: var(--preto);
      color: var(--branco);
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

    .layout {
      min-height: 100vh;
    }

    .sidebar {
      position: fixed;
      z-index: 10;
      top: 0;
      bottom: 0;
      left: 0;
      width: 245px;
      padding: 22px 14px;
      overflow-y: auto;
      background: #050505;
      border-right: 1px solid var(--borda);
    }

    .logo {
      margin: 0 10px 28px;
      color: var(--vermelho);
      font-size: 23px;
      font-weight: bold;
    }

    .logo small {
      display: block;
      margin-top: 5px;
      color: var(--cinza);
      font-size: 10px;
      font-weight: normal;
      letter-spacing: 1px;
    }

    .nav-button {
      width: 100%;
      margin: 3px 0;
      padding: 13px 12px;
      border: 0;
      border-radius: 7px;
      background: transparent;
      color: #bdbdbd;
      text-align: left;
      transition: .2s;
    }

    .nav-button:hover,
    .nav-button.active {
      background: var(--vermelho);
      color: white;
    }

    .main {
      width: calc(100% - 245px);
      min-height: 100vh;
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
    h3,
    p {
      margin-top: 0;
    }

    h1 {
      margin-bottom: 5px;
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
      color: var(--cinza);
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
      border: 1px solid var(--borda);
      border-radius: 9px;
      background: var(--preto-2);
    }

    .panel + .panel {
      margin-top: 15px;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 15px;
      margin-bottom: 20px;
    }

    .metric-label {
      color: var(--cinza);
      font-size: 11px;
      letter-spacing: .5px;
      text-transform: uppercase;
    }

    .metric-value {
      margin-top: 10px;
      font-size: 26px;
      font-weight: bold;
    }

    .green {
      color: var(--verde);
    }

    .red {
      color: var(--vermelho);
    }

    .yellow {
      color: var(--amarelo);
    }

    .blue {
      color: var(--azul);
    }

    .purple {
      color: var(--roxo);
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
      border: 1px solid var(--borda);
      border-radius: 5px;
      background: #0b0b0b;
      color: white;
    }

    input:focus,
    select:focus,
    textarea:focus {
      border-color: var(--vermelho);
    }

    textarea {
      min-height: 80px;
      resize: vertical;
    }

    input[type="color"] {
      height: 40px;
      padding: 3px;
    }

    .actions {
      display: flex;
      flex-wrap: wrap;
      gap: 9px;
      margin-top: 15px;
    }

    .button {
      padding: 10px 14px;
      border: 1px solid var(--borda);
      border-radius: 6px;
      background: var(--preto-3);
      color: white;
    }

    .button:hover {
      filter: brightness(1.25);
    }

    .button.primary {
      border-color: var(--vermelho);
      background: var(--vermelho);
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

    .toolbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 12px;
      margin-bottom: 15px;
    }

    .toolbar input {
      max-width: 320px;
    }

    .table-container {
      overflow-x: auto;
    }

    table {
      width: 100%;
      min-width: 900px;
      border-collapse: collapse;
    }

    th,
    td {
      padding: 11px 9px;
      border-bottom: 1px solid var(--borda);
      text-align: left;
      vertical-align: middle;
      font-size: 13px;
    }

    th {
      color: var(--cinza);
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
      background: #551017;
      color: #ff848b;
    }

    .badge-b {
      background: #55430b;
      color: #f6d469;
    }

    .badge-c {
      background: #123e5d;
      color: #79bbff;
    }

    .badge-active {
      background: #075b3b;
      color: #7df0bd;
    }

    .badge-inactive {
      background: #571018;
      color: #ff969c;
    }

    .badge-warning {
      background: #564207;
      color: #ffdd67;
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
      white-space: nowrap;
    }

    .chip.inactive {
      border-color: #2c2c2c;
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
      border: 1px solid var(--borda);
      border-radius: 6px;
      background: #101010;
    }

    .list-item strong {
      display: block;
      margin-bottom: 5px;
    }

    .empty {
      padding: 23px 10px;
      color: var(--cinza);
      text-align: center;
      font-size: 13px;
    }

    .alert {
      margin-bottom: 15px;
      padding: 13px;
      border-left: 4px solid var(--amarelo);
      border-radius: 5px;
      background: #261f08;
      color: #f4d97b;
      font-size: 13px;
    }

    .alert.red-alert {
      border-left-color: var(--vermelho);
      background: #2a0a0d;
      color: #ffafb4;
    }

    .alert.green-alert {
      border-left-color: var(--verde);
      background: #082b1d;
      color: #89e5b9;
    }

    .progress {
      height: 12px;
      overflow: hidden;
      border-radius: 20px;
      background: #292929;
    }

    .progress-bar {
      height: 100%;
      min-width: 0;
      border-radius: 20px;
      background: linear-gradient(90deg, var(--vermelho), #ff4851);
    }

    .supplier-products {
      padding-left: 17px;
      color: var(--cinza);
      font-size: 12px;
    }

    .sale-line {
      display: grid;
      grid-template-columns: 180px 1fr 95px 120px 42px;
      align-items: end;
      gap: 8px;
      margin-bottom: 9px;
    }

    .line-total {
      padding-bottom: 10px;
      color: var(--verde);
      font-size: 13px;
      font-weight: bold;
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
      padding: 21px;
      border: 1px solid #444;
      border-top: 3px solid var(--vermelho);
      border-radius: 9px;
      background: var(--preto-2);
    }

    .modal-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 18px;
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

    @media (max-width: 1150px) {
      .cards {
        grid-template-columns: repeat(2, 1fr);
      }

      .grid-4 {
        grid-template-columns: repeat(2, 1fr);
      }

      .profile-columns {
        grid-template-columns: 1fr;
      }

      .sale-line {
        grid-template-columns: 150px 1fr 80px 110px 38px;
      }
    }

    @media (max-width: 750px) {
      .sidebar {
        width: 65px;
        padding: 15px 7px;
      }

      .logo {
        margin: 0 0 27px;
        font-size: 0;
        text-align: center;
      }

      .logo::before {
        content: "G";
        font-size: 24px;
      }

      .logo small,
      .nav-button span {
        display: none;
      }

      .nav-button {
        padding: 12px 5px;
        text-align: center;
        font-size: 17px;
      }

      .main {
        width: calc(100% - 65px);
        margin-left: 65px;
        padding: 16px;
      }

      .grid-2,
      .grid-3,
      .grid-4 {
        grid-template-columns: 1fr;
      }

      .cards {
        grid-template-columns: 1fr 1fr;
        gap: 8px;
      }

      .card,
      .panel {
        padding: 13px;
      }

      .metric-value {
        font-size: 21px;
      }

      .sale-line {
        grid-template-columns: 1fr 75px 100px 35px;
      }

      .sale-line .supplier-field {
        grid-column: 1 / -1;
      }

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

      <button class="nav-button active" data-page="dashboard">▣ <span>Dashboard</span></button>
      <button class="nav-button" data-page="clientes">♙ <span>Clientes</span></button>
      <button class="nav-button" data-page="produtos">▤ <span>Produtos</span></button>
      <button class="nav-button" data-page="fornecedores">◉ <span>Fornecedores</span></button>
      <button class="nav-button" data-page="abc">▥ <span>Curva ABC</span></button>
    </aside>

    <main class="main">
      <div class="topbar">
        <div>
          <h1 id="page-title">Dashboard</h1>
          <div class="muted">Controle comercial, metas e oportunidades de vendas</div>
        </div>

        <button class="button primary" onclick="openSaleModal()">+ Nova venda</button>
      </div>

      <!-- DASHBOARD -->
      <section class="page active" id="page-dashboard">
        <div id="dashboard-alerts"></div>

        <div class="panel">
          <div class="toolbar">
            <div>
              <h2>Meta de vendas</h2>
              <div class="muted">
                Informe a meta mensal e a meta diária desejada.
              </div>
            </div>

            <button class="button small" onclick="openSettingsModal()">
              Configurar meta
            </button>
          </div>

          <div class="cards">
            <div class="card">
              <div class="metric-label">Meta mensal</div>
              <div class="metric-value" id="goal-month">R$ 0,00</div>
            </div>

            <div class="card">
              <div class="metric-label">Vendido no mês</div>
              <div class="metric-value green" id="goal-sold">R$ 0,00</div>
            </div>

            <div class="card">
              <div class="metric-label">Falta vender</div>
              <div class="metric-value red" id="goal-missing">R$ 0,00</div>
            </div>

            <div class="card">
              <div class="metric-label">Necessário por dia</div>
              <div class="metric-value yellow" id="goal-needed-day">R$ 0,00</div>
            </div>
          </div>

          <div class="progress">
            <div class="progress-bar" id="goal-progress"></div>
          </div>

          <div class="muted" id="goal-summary" style="margin-top:9px"></div>
        </div>

        <div class="cards" style="margin-top:15px">
          <div class="card">
            <div class="metric-label">Clientes cadastrados</div>
            <div class="metric-value" id="metric-clients">0</div>
          </div>

          <div class="card">
            <div class="metric-label">Produtos cadastrados</div>
            <div class="metric-value" id="metric-products">0</div>
          </div>

          <div class="card">
            <div class="metric-label">Vendas realizadas</div>
            <div class="metric-value" id="metric-sales">0</div>
          </div>

          <div class="card">
            <div class="metric-label">Faturamento geral</div>
            <div class="metric-value green" id="metric-revenue">R$ 0,00</div>
          </div>
        </div>

        <div class="grid-2">
          <div class="panel">
            <h2>Aniversariantes</h2>
            <div class="muted" style="margin-bottom:12px">
              Clientes que fazem aniversário neste mês.
            </div>
            <div id="birthdays-list"></div>
          </div>

          <div class="panel">
            <h2>Oportunidades de expansão</h2>
            <div class="muted" style="margin-bottom:12px">
              Clientes com possibilidade de comprar mais produtos.
            </div>
            <div id="expansion-list"></div>
          </div>
        </div>

        <div class="grid-2" style="margin-top:15px">
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
                <label>Cidade</label>
                <input id="client-city">
              </div>

              <div class="field">
                <label>Observações</label>
                <input id="client-notes">
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

          <div class="table-container">
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
                <input id="product-sku" required placeholder="Ex.: ABC-001">
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
                <label>Preço de venda *</label>
                <input id="product-price" type="number" min="0" step="0.01" required>
              </div>

              <div class="field">
                <label>Categoria</label>
                <input id="product-category">
              </div>

              <div class="field">
                <label>Prazo de garantia em dias</label>
                <input id="product-warranty" type="number" min="0" value="0">
              </div>

              <div class="field full">
                <label>Observações</label>
                <textarea id="product-notes"></textarea>
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
            <input id="product-search" placeholder="Buscar por SKU ou nome..." oninput="renderProducts()">
          </div>

          <div class="table-container">
            <table>
              <thead>
                <tr>
                  <th>SKU</th>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Categoria</th>
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
                <label>Nome do fornecedor *</label>
                <input id="supplier-name" required>
              </div>

              <div class="field">
                <label>Contato</label>
                <input id="supplier-contact">
              </div>

              <div class="field">
                <label>Cor do fornecedor</label>
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

          <div class="table-container">
            <table>
              <thead>
                <tr>
                  <th>Fornecedor</th>
                  <th>Contato</th>
                  <th>Produtos vinculados</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="suppliers-table"></tbody>
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
                Classificação por faturamento acumulado: A = 60%, B = 30%, C = 10%.
              </div>
            </div>

            <select id="abc-period" onchange="renderABC()">
              <option value="all">Todo o período</option>
              <option value="365">Últimos 365 dias</option>
              <option value="90">Últimos 90 dias</option>
              <option value="30">Últimos 30 dias</option>
            </select>
          </div>

          <div class="alert">
            Os produtos são ordenados do maior para o menor faturamento.
            A classificação é calculada pelo percentual acumulado do faturamento,
            e não pela quantidade de produtos.
          </div>

          <div class="table-container">
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
          <div class="muted" style="margin-bottom:14px">
            Clique no cliente para acessar o perfil, histórico, fornecedores,
            sugestões e oportunidades de expansão.
          </div>

          <div class="table-container">
            <table>
              <thead>
                <tr>
                  <th>Cliente</th>
                  <th>Curva</th>
                  <th>Pedidos</th>
                  <th>Itens</th>
                  <th>Faturamento</th>
                  <th>% individual</th>
                  <th>% acumulado</th>
                  <th>Última compra</th>
                  <th>Ação</th>
                </tr>
              </thead>
              <tbody id="abc-clients-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- PERFIL DO CLIENTE -->
      <section class="page" id="page-profile">
        <div id="client-profile"></div>
      </section>
    </main>
  </div>

  <!-- MODAL DE CONFIGURAÇÃO DE META -->
  <div class="modal" id="settings-modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2>Configurar meta de vendas</h2>
        <button class="close" onclick="closeModal('settings-modal')">×</button>
      </div>

      <form id="settings-form">
        <div class="grid-2">
          <div class="field">
            <label>Meta mensal de vendas *</label>
            <input id="monthly-goal" type="number" min="0" step="0.01" required>
          </div>

          <div class="field">
            <label>Meta diária desejada *</label>
            <input id="daily-goal" type="number" min="0" step="0.01" required>
          </div>
        </div>

        <div class="actions">
          <button class="button primary">Salvar meta</button>
          <button type="button" class="button" onclick="closeModal('settings-modal')">
            Cancelar
          </button>
        </div>
      </form>
    </div>
  </div>

  <!-- MODAL DE VENDA -->
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
            <label>Data *</label>
            <input id="sale-date" type="date" required>
          </div>

          <div class="field">
            <label>Vendedor</label>
            <input id="sale-seller">
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

        <h3 style="margin-top:20px">Itens da venda</h3>

        <div class="alert">
          Para cada item, selecione primeiro o fornecedor.
          Depois, aparecerão somente os produtos daquele fornecedor.
          O SKU é exibido automaticamente.
        </div>

        <div id="sale-lines"></div>

        <button type="button" class="button small" onclick="addSaleLine()">
          + Adicionar item
        </button>

        <div class="field" style="margin-top:15px">
          <label>Observações do pedido</label>
          <textarea id="sale-notes"></textarea>
        </div>

        <div style="margin-top:15px;text-align:right;font-size:19px">
          Total:
          <strong class="green" id="sale-total">R$ 0,00</strong>
        </div>

        <div class="actions">
          <button class="button primary">Salvar venda</button>
          <button type="button" class="button" onclick="closeModal('sale-modal')">
            Cancelar
          </button>
        </div>
      </form>
    </div>
  </div>

  <!-- MODAL DE PEDIDO -->
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
    const STORAGE_KEY = "gestao_comercial_completo_abc_60_30_10";

    let database = JSON.parse(localStorage.getItem(STORAGE_KEY)) || {
      settings: {
        monthlyGoal: 0,
        dailyGoal: 0
      },
      clients: [],
      suppliers: [],
      products: [],
      sales: [],
      attachments: [],
      lowerReasons: []
    };

    function saveDatabase() {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(database));
    }

    function id(prefix) {
      return prefix + "_" + Date.now().toString(36) + Math.random().toString(36).substring(2, 8);
    }

    function today() {
      return new Date().toISOString().substring(0, 10);
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
      return String(value ?? "").replace(/[&<>"']/g, function(character) {
        const replacements = {
          "&": "&",
          "<": "<",
          ">": ">",
          '"': "&quot;",
          "'": "&#039;"
        };

        return replacements[character];
      });
    }

    function getClient(clientId) {
      return database.clients.find(function(client) {
        return client.id === clientId;
      });
    }

    function getSupplier(supplierId) {
      return database.suppliers.find(function(supplier) {
        return supplier.id === supplierId;
      });
    }

    function getProduct(productId) {
      return database.products.find(function(product) {
        return product.id === productId;
      });
    }

    function getSaleTotal(sale) {
      return (sale.items || []).reduce(function(total, item) {
        return total + Number(item.quantity || 0) * Number(item.price || 0);
      }, 0);
    }

    function getClientSales(clientId, salesList) {
      const source = salesList || database.sales;

      return source.filter(function(sale) {
        return sale.clientId === clientId;
      });
    }

    function getProductQuantity(productId, salesList) {
      const source = salesList || database.sales;

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
      const source = salesList || database.sales;

      return source.reduce(function(total, sale) {
        return total + (sale.items || []).reduce(function(itemTotal, item) {
          if (item.productId === productId) {
            return itemTotal + Number(item.quantity || 0) * Number(item.price || 0);
          }

          return itemTotal;
        }, 0);
      }, 0);
    }

    function getProductClients(productId, salesList) {
      const source = salesList || database.sales;
      const clientIds = [];

      source.forEach(function(sale) {
        const hasProduct = (sale.items || []).some(function(item) {
          return item.productId === productId;
        });

        if (hasProduct && !clientIds.includes(sale.clientId)) {
          clientIds.push(sale.clientId);
        }
      });

      return clientIds.length;
    }

    function getClientStats(clientId, salesList) {
      const sales = getClientSales(clientId, salesList);
      const quantities = {};
      let totalRevenue = 0;
      let totalItems = 0;

      sales.forEach(function(sale) {
        totalRevenue += getSaleTotal(sale);

        (sale.items || []).forEach(function(item) {
          quantities[item.productId] = (quantities[item.productId] || 0) + Number(item.quantity || 0);
          totalItems += Number(item.quantity || 0);
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
        revenue: totalRevenue,
        items: totalItems,
        lastSale: dates[0] || ""
      };
    }

    function getDaysWithoutPurchase(client) {
      const stats = getClientStats(client.id);

      if (!stats.lastSale) {
        return Infinity;
      }

      const lastSale = new Date(stats.lastSale + "T12:00:00");
      return Math.floor((new Date() - lastSale) / 86400000);
    }

    function getClientStatus(client) {
      const days = getDaysWithoutPurchase(client);

      if (days === Infinity) return "Nunca comprou";
      if (days > 45) return "Mais de 45 dias";
      if (days > 30) return "Mais de 30 dias";
      if (days > 15) return "Mais de 15 dias";

      return "Ativo";
    }

    function getMonthSales() {
      const month = today().substring(0, 7);

      return database.sales.filter(function(sale) {
        return String(sale.date).substring(0, 7) === month;
      });
    }

    function getRemainingDaysInMonth() {
      const current = new Date();
      const year = current.getFullYear();
      const month = current.getMonth();

      return new Date(year, month + 1, 0).getDate() - current.getDate() + 1;
    }

    function getSupplierChip(supplier, active) {
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

    function getABCBadge(curve) {
      return `
        <span class="badge badge-${String(curve).toLowerCase()}">
          Curva ${curve}
        </span>
      `;
    }

    function showPage(page) {
      document.querySelectorAll(".page").forEach(function(section) {
        section.classList.remove("active");
      });

      document.querySelectorAll(".nav-button").forEach(function(button) {
        button.classList.remove("active");
      });

      const target = document.getElementById("page-" + page);

      if (target) {
        target.classList.add("active");
      }

      const navButton = document.querySelector('[data-page="' + page + '"]');

      if (navButton) {
        navButton.classList.add("active");
      }

      const titles = {
        dashboard: "Dashboard",
        clientes: "Clientes",
        produtos: "Produtos",
        fornecedores: "Fornecedores",
        abc: "Curva ABC",
        profile: "Perfil do cliente"
      };

      document.getElementById("page-title").textContent = titles[page] || "Gestão";
    }

    document.querySelectorAll(".nav-button").forEach(function(button) {
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
      const totalRevenue = database.sales.reduce(function(total, sale) {
        return total + getSaleTotal(sale);
      }, 0);

      const monthSales = getMonthSales();
      const monthRevenue = monthSales.reduce(function(total, sale) {
        return total + getSaleTotal(sale);
      }, 0);

      const monthlyGoal = Number(database.settings.monthlyGoal || 0);
      const dailyGoal = Number(database.settings.dailyGoal || 0);
      const missing = Math.max(monthlyGoal - monthRevenue, 0);
      const remainingDays = getRemainingDaysInMonth();
      const neededPerDay = missing / Math.max(remainingDays, 1);
      const progress = monthlyGoal > 0
        ? Math.min((monthRevenue / monthlyGoal) * 100, 100)
        : 0;

      document.getElementById("goal-month").textContent = money(monthlyGoal);
      document.getElementById("goal-sold").textContent = money(monthRevenue);
      document.getElementById("goal-missing").textContent = money(missing);
      document.getElementById("goal-needed-day").textContent = money(neededPerDay);
      document.getElementById("goal-progress").style.width = progress + "%";

      document.getElementById("goal-summary").textContent =
        "Meta diária configurada: " + money(dailyGoal) +
        " · " + remainingDays +
        " dia(s) restante(s) no mês · " +
        progress.toFixed(1) + "% da meta mensal atingida.";

      document.getElementById("metric-clients").textContent = database.clients.length;
      document.getElementById("metric-products").textContent = database.products.length;
      document.getElementById("metric-sales").textContent = database.sales.length;
      document.getElementById("metric-revenue").textContent = money(totalRevenue);

      renderBirthdays();
      renderInactiveClients();
      renderExpansionOpportunities();
      renderUnusedProducts();

      const alerts = [];

      if (database.settings.monthlyGoal <= 0) {
        alerts.push(`
          <div class="alert">
            A meta de vendas ainda não foi configurada.
            Clique em <strong>Configurar meta</strong> para informar os valores.
          </div>
        `);
      }

      const warranties = getWarrantyPendencies();

      if (warranties.length) {
        alerts.push(`
          <div class="alert red-alert">
            Existem <strong>${warranties.length}</strong> garantia(s) ativa(s)
            aguardando acompanhamento.
          </div>
        `);
      }

      document.getElementById("dashboard-alerts").innerHTML = alerts.join("");
    }

    function renderBirthdays() {
      const currentMonth = today().substring(5, 7);

      const birthdays = database.clients
        .filter(function(client) {
          return client.birth && client.birth.substring(5, 7) === currentMonth;
        })
        .sort(function(a, b) {
          return a.birth.substring(8, 10).localeCompare(b.birth.substring(8, 10));
        });

      document.getElementById("birthdays-list").innerHTML = birthdays.length
        ? birthdays.map(function(client) {
            const day = client.birth.substring(8, 10);

            return `
              <div
                class="list-item"
                style="cursor:pointer"
                onclick="openClientProfile('${client.id}')">

                <strong>${escapeHTML(client.name)}</strong>

                <div class="muted">
                  Aniversário: dia ${day}
                  ${client.phone ? " · " + escapeHTML(client.phone) : ""}
                </div>

                <div class="actions">
                  <button
                    class="button small success"
                    onclick="event.stopPropagation();sendBirthdayMessage('${client.id}')">
                    Preparar WhatsApp
                  </button>
                </div>
              </div>
            `;
          }).join("")
        : `<div class="empty">Nenhum aniversariante neste mês.</div>`;
    }

    function renderInactiveClients() {
      const inactive = database.clients
        .map(function(client) {
          return {
            client: client,
            days: getDaysWithoutPurchase(client),
            stats: getClientStats(client.id)
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

      document.getElementById("inactive-list").innerHTML = inactive.length
        ? inactive.map(function(item) {
            return `
              <div
                class="list-item"
                style="cursor:pointer"
                onclick="openClientProfile('${item.client.id}')">

                <strong>${escapeHTML(item.client.name)}</strong>

                <div class="muted">
                  ${
                    item.days === Infinity
                      ? "Nunca comprou"
                      : item.days + " dia(s) sem comprar"
                  }
                  · Último faturamento: ${money(item.stats.revenue)}
                </div>
              </div>
            `;
          }).join("")
        : `<div class="empty">Nenhum cliente inativo.</div>`;
    }

    function renderExpansionOpportunities() {
      const opportunities = database.clients
        .map(function(client) {
          const stats = getClientStats(client.id);
          const suggestions = getSuggestions(client.id).slice(0, 3);
          const lower = getLowerPurchases(client.id).slice(0, 2);
          const days = getDaysWithoutPurchase(client);

          return {
            client: client,
            stats: stats,
            suggestions: suggestions,
            lower: lower,
            days: days
          };
        })
        .filter(function(item) {
          return item.suggestions.length > 0 || item.lower.length > 0;
        })
        .sort(function(a, b) {
          const aScore = a.suggestions.length + a.lower.length;
          const bScore = b.suggestions.length + b.lower.length;

          return bScore - aScore;
        })
        .slice(0, 10);

      document.getElementById("expansion-list").innerHTML = opportunities.length
        ? opportunities.map(function(item) {
            const products = item.suggestions
              .map(function(suggestion) {
                return suggestion.product.name;
              })
              .join(", ");

            const lower = item.lower
              .map(function(itemLower) {
                return itemLower.product.name;
              })
              .join(", ");

            return `
              <div
                class="list-item"
                style="cursor:pointer"
                onclick="openClientProfile('${item.client.id}')">

                <strong>${escapeHTML(item.client.name)}</strong>

                <div class="muted">
                  ${item.stats.sales.length} pedido(s) ·
                  ${money(item.stats.revenue)} comprados
                </div>

                ${
                  products
                    ? `
                      <div class="muted" style="margin-top:6px">
                        Sugestões: ${escapeHTML(products)}
                      </div>
                    `
                    : ""
                }

                ${
                  lower
                    ? `
                      <div class="muted" style="margin-top:4px">
                        Abaixo da média: ${escapeHTML(lower)}
                      </div>
                    `
                    : ""
                }
              </div>
            `;
          }).join("")
        : `<div class="empty">Nenhuma oportunidade identificada.</div>`;
    }

    function renderUnusedProducts() {
      const unused = database.products.filter(function(product) {
        return getProductQuantity(product.id) === 0;
      });

      document.getElementById("unused-products").innerHTML = unused.length
        ? unused.map(function(product) {
            const supplier = getSupplier(product.supplierId);

            return `
              <div class="list-item">
                <strong>${escapeHTML(product.name)}</strong>
                <div class="muted">
                  SKU: ${escapeHTML(product.sku)} ·
                  Fornecedor: ${supplier ? escapeHTML(supplier.name) : "—"}
                </div>
              </div>
            `;
          }).join("")
        : `<div class="empty">Todos os produtos possuem pedidos.</div>`;
    }

    function renderClients() {
      const search = (document.getElementById("client-search")?.value || "").toLowerCase();

      const clients = database.clients.filter(function(client) {
        return client.name.toLowerCase().includes(search) ||
          (client.phone || "").toLowerCase().includes(search) ||
          (client.email || "").toLowerCase().includes(search);
      });

      document.getElementById("clients-table").innerHTML = clients.length
        ? clients.map(function(client) {
            const stats = getClientStats(client.id);
            const status = getClientStatus(client);
            const statusClass = status === "Ativo" ? "badge-active" : "badge-inactive";

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
                  <span class="badge ${statusClass}">
                    ${status}
                  </span>
                </td>

                <td>${stats.sales.length}</td>
                <td class="green">${money(stats.revenue)}</td>

                <td>
                  <button
                    class="button small"
                    onclick="event.stopPropagation();openClientProfile('${client.id}')">
                    Abrir
                  </button>

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

    document.getElementById("client-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.clients.push({
        id: id("client"),
        name: document.getElementById("client-name").value.trim(),
        phone: document.getElementById("client-phone").value.trim(),
        email: document.getElementById("client-email").value.trim(),
        birth: document.getElementById("client-birth").value,
        city: document.getElementById("client-city").value.trim(),
        notes: document.getElementById("client-notes").value.trim(),
        createdAt: today()
      });

      saveDatabase();
      event.target.reset();
      renderAll();

      alert("Cliente cadastrado com sucesso.");
    });

    function deleteClient(clientId) {
      const client = getClient(clientId);

      if (!client) return;

      if (!confirm("Excluir " + client.name + " e todo o histórico de vendas?")) {
        return;
      }

      database.clients = database.clients.filter(function(item) {
        return item.id !== clientId;
      });

      database.sales = database.sales.filter(function(sale) {
        return sale.clientId !== clientId;
      });

      database.attachments = database.attachments.filter(function(file) {
        return file.clientId !== clientId;
      });

      database.lowerReasons = database.lowerReasons.filter(function(item) {
        return item.clientId !== clientId;
      });

      saveDatabase();
      renderAll();
    }

    function renderSuppliers() {
      document.getElementById("suppliers-table").innerHTML = database.suppliers.length
        ? database.suppliers.map(function(supplier) {
            const products = database.products.filter(function(product) {
              return product.supplierId === supplier.id;
            });

            return `
              <tr>
                <td>
                  ${getSupplierChip(supplier, true)}
                  <div class="muted">${escapeHTML(supplier.contact || "Sem contato")}</div>
                </td>

                <td>${escapeHTML(supplier.contact || "—")}</td>

                <td>
                  <div class="supplier-products">
                    ${
                      products.length
                        ? products.map(function(product) {
                            return `
                              <div>
                                ${escapeHTML(product.sku)} —
                                ${escapeHTML(product.name)}
                              </div>
                            `;
                          }).join("")
                        : "Nenhum produto vinculado"
                    }
                  </div>
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

    document.getElementById("supplier-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.suppliers.push({
        id: id("supplier"),
        name: document.getElementById("supplier-name").value.trim(),
        contact: document.getElementById("supplier-contact").value.trim(),
        color: document.getElementById("supplier-color").value
      });

      saveDatabase();
      event.target.reset();
      document.getElementById("supplier-color").value = "#e50914";
      renderAll();

      alert("Fornecedor cadastrado com sucesso.");
    });

    function deleteSupplier(supplierId) {
      const hasProducts = database.products.some(function(product) {
        return product.supplierId === supplierId;
      });

      if (hasProducts) {
        alert("Não é possível excluir um fornecedor que possui produtos vinculados.");
        return;
      }

      database.suppliers = database.suppliers.filter(function(supplier) {
        return supplier.id !== supplierId;
      });

      saveDatabase();
      renderAll();
    }

    document.getElementById("product-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const sku = document.getElementById("product-sku").value.trim().toUpperCase();

      const skuExists = database.products.some(function(product) {
        return product.sku.toUpperCase() === sku;
      });

      if (skuExists) {
        alert("Esse SKU já está cadastrado. Informe outro SKU.");
        return;
      }

      const supplierId = document.getElementById("product-supplier").value;

      if (!supplierId) {
        alert("Selecione o fornecedor do produto.");
        return;
      }

      database.products.push({
        id: id("product"),
        sku: sku,
        name: document.getElementById("product-name").value.trim(),
        supplierId: supplierId,
        price: Number(document.getElementById("product-price").value || 0),
        category: document.getElementById("product-category").value.trim(),
        warrantyDays: Number(document.getElementById("product-warranty").value || 0),
        notes: document.getElementById("product-notes").value.trim()
      });

      saveDatabase();
      event.target.reset();
      renderAll();

      alert("Produto cadastrado com sucesso.");
    });

    function renderProducts() {
      const search = (document.getElementById("product-search")?.value || "").toLowerCase();

      const products = database.products.filter(function(product) {
        return product.sku.toLowerCase().includes(search) ||
          product.name.toLowerCase().includes(search) ||
          (product.category || "").toLowerCase().includes(search);
      });

      document.getElementById("products-table").innerHTML = products.length
        ? products.map(function(product) {
            const supplier = getSupplier(product.supplierId);

            return `
              <tr>
                <td><strong>${escapeHTML(product.sku)}</strong></td>

                <td>
                  <strong>${escapeHTML(product.name)}</strong>
                  <br>
                  <span class="muted">
                    Garantia: ${product.warrantyDays || 0} dia(s)
                  </span>
                </td>

                <td>${supplier ? getSupplierChip(supplier, true) : "—"}</td>
                <td>${escapeHTML(product.category || "—")}</td>
                <td>${money(product.price)}</td>
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

    function deleteProduct(productId) {
      const hasSales = database.sales.some(function(sale) {
        return (sale.items || []).some(function(item) {
          return item.productId === productId;
        });
      });

      if (hasSales) {
        alert("Esse produto possui histórico de vendas e não pode ser excluído.");
        return;
      }

      database.products = database.products.filter(function(product) {
        return product.id !== productId;
      });

      saveDatabase();
      renderAll();
    }

    function updateSelects() {
      const supplierSelect = document.getElementById("product-supplier");

      if (supplierSelect) {
        const currentSupplier = supplierSelect.value;

        supplierSelect.innerHTML =
          `<option value="">Selecione...</option>` +
          database.suppliers.map(function(supplier) {
            return `
              <option value="${supplier.id}">
                ${escapeHTML(supplier.name)}
              </option>
            `;
          }).join("");

        if (currentSupplier) {
          supplierSelect.value = currentSupplier;
        }
      }

      const clientSelect = document.getElementById("sale-client");

      if (clientSelect) {
        const currentClient = clientSelect.value;

        clientSelect.innerHTML =
          `<option value="">Selecione...</option>` +
          database.clients.map(function(client) {
            return `
              <option value="${client.id}">
                ${escapeHTML(client.name)}
              </option>
            `;
          }).join("");

        if (currentClient) {
          clientSelect.value = currentClient;
        }
      }
    }

    function getSalesByPeriod() {
      const period = document.getElementById("abc-period")?.value || "all";

      if (period === "all") {
        return database.sales;
      }

      const limit = new Date();
      limit.setDate(limit.getDate() - Number(period));

      return database.sales.filter(function(sale) {
        return new Date(sale.date + "T12:00:00") >= limit;
      });
    }

    /*
      CURVA ABC CORRETA:

      Curva A: até 60% do faturamento acumulado.
      Curva B: acima de 60% até 90% acumulado.
      Curva C: acima de 90% até 100% acumulado.

      O produto que ultrapassa o limite entra na curva correspondente
      ao percentual acumulado após a inclusão dele.
    */
    function getCurveByAccumulated(accumulatedPercentage) {
      if (accumulatedPercentage <= 60) {
        return "A";
      }

      if (accumulatedPercentage <= 90) {
        return "B";
      }

      return "C";
    }

    function calculateABC(rows) {
      const sortedRows = rows
        .slice()
        .sort(function(a, b) {
          return b.revenue - a.revenue;
        });

      const total = sortedRows.reduce(function(sum, row) {
        return sum + Number(row.revenue || 0);
      }, 0);

      let accumulated = 0;

      return sortedRows.map(function(row, index) {
        const individualPercentage = total > 0
          ? Number(row.revenue || 0) / total * 100
          : 0;

        accumulated += individualPercentage;

        return {
          row: row,
          index: index + 1,
          individualPercentage: individualPercentage,
          accumulatedPercentage: accumulated,
          curve: getCurveByAccumulated(accumulated)
        };
      });
    }

    function renderABC() {
      const sales = getSalesByPeriod();

      const productRows = database.products.map(function(product) {
        return {
          product: product,
          revenue: getProductRevenue(product.id, sales),
          quantity: getProductQuantity(product.id, sales),
          clients: getProductClients(product.id, sales)
        };
      });

      const productABC = calculateABC(productRows);

      document.getElementById("abc-products-table").innerHTML = productABC.length
        ? productABC.map(function(item) {
            const product = item.row.product;
            const supplier = getSupplier(product.supplierId);

            return `
              <tr>
                <td>${item.index}</td>

                <td>
                  <strong>${escapeHTML(product.name)}</strong>
                  <br>
                  <span class="muted">SKU: ${escapeHTML(product.sku)}</span>
                </td>

                <td>${supplier ? getSupplierChip(supplier, true) : "—"}</td>
                <td>${getABCBadge(item.curve)}</td>
                <td>${item.row.quantity}</td>
                <td class="green">${money(item.row.revenue)}</td>
                <td>${item.individualPercentage.toFixed(2)}%</td>
                <td>${item.accumulatedPercentage.toFixed(2)}%</td>
                <td>${item.row.clients}</td>
              </tr>
            `;
          }).join("")
        : `
          <tr>
            <td colspan="9" class="empty">
              Cadastre produtos e vendas para visualizar a Curva ABC.
            </td>
          </tr>
        `;

      const clientRows = database.clients.map(function(client) {
        const stats = getClientStats(client.id, sales);

        return {
          client: client,
          revenue: stats.revenue,
          stats: stats
        };
      });

      const clientABC = calculateABC(clientRows);

      document.getElementById("abc-clients-table").innerHTML = clientABC.length
        ? clientABC.map(function(item) {
            const client = item.row.client;

            return `
              <tr
                class="clickable"
                onclick="openClientProfile('${client.id}')">

                <td>
                  <strong>${escapeHTML(client.name)}</strong>
                  <br>
                  <span class="muted">Abrir análise individual</span>
                </td>

                <td>${getABCBadge(item.curve)}</td>
                <td>${item.row.stats.sales.length}</td>
                <td>${item.row.stats.items}</td>
                <td class="green">${money(item.row.revenue)}</td>
                <td>${item.individualPercentage.toFixed(2)}%</td>
                <td>${item.accumulatedPercentage.toFixed(2)}%</td>
                <td>${dateBR(item.row.stats.lastSale)}</td>

                <td>
                  <button
                    class="button small primary"
                    onclick="event.stopPropagation();openClientProfile('${client.id}')">
                    Ver perfil
                  </button>
                </td>
              </tr>
            `;
          }).join("")
        : `
          <tr>
            <td colspan="9" class="empty">
              Cadastre clientes e vendas para visualizar a Curva ABC.
            </td>
          </tr>
        `;
    }

    function getSuggestions(clientId) {
      const clientStats = getClientStats(clientId);
      const purchasedIds = Object.keys(clientStats.quantities);

      const products = database.products.map(function(product) {
        const productRows = database.products.map(function(item) {
          return {
            product: item,
            revenue: getProductRevenue(item.id)
          };
        });

        const abc = calculateABC(productRows).find(function(item) {
          return item.row.product.id === product.id;
        });

        return {
          product: product,
          curve: abc ? abc.curve : "C",
          revenue: getProductRevenue(product.id),
          quantity: getProductQuantity(product.id),
          supplier: getSupplier(product.supplierId)
        };
      });

      return products
        .filter(function(item) {
          return !purchasedIds.includes(item.product.id);
        })
        .sort(function(a, b) {
          const curveOrder = {
            A: 1,
            B: 2,
            C: 3
          };

          if (curveOrder[a.curve] !== curveOrder[b.curve]) {
            return curveOrder[a.curve] - curveOrder[b.curve];
          }

          return b.revenue - a.revenue;
        });
    }

    function getLowerPurchases(clientId) {
      const clientStats = getClientStats(clientId);
      const result = [];

      database.products.forEach(function(product) {
        const clientQuantity = Number(clientStats.quantities[product.id] || 0);

        if (clientQuantity <= 0) {
          return;
        }

        let totalQuantity = 0;
        let buyers = 0;

        database.clients.forEach(function(client) {
          const stats = getClientStats(client.id);
          const quantity = Number(stats.quantities[product.id] || 0);

          if (quantity > 0) {
            totalQuantity += quantity;
            buyers++;
          }
        });

        if (!buyers) {
          return;
        }

        const average = totalQuantity / buyers;

        if (clientQuantity < average) {
          const reason = database.lowerReasons.find(function(item) {
            return item.clientId === clientId &&
              item.productId === product.id;
          });

          result.push({
            product: product,
            clientQuantity: clientQuantity,
            average: average,
            reason: reason ? reason.reason : ""
          });
        }
      });

      return result.sort(function(a, b) {
        return (b.average - b.clientQuantity) - (a.average - a.clientQuantity);
      });
    }

    function openClientProfile(clientId) {
      const client = getClient(clientId);

      if (!client) return;

      const stats = getClientStats(clientId);
      const suggestions = getSuggestions(clientId);
      const lowerPurchases = getLowerPurchases(clientId);
      const purchasedProducts = Object.keys(stats.quantities);
      const purchasedSuppliers = [];

      purchasedProducts.forEach(function(productId) {
        const product = getProduct(productId);

        if (product && !purchasedSuppliers.includes(product.supplierId)) {
          purchasedSuppliers.push(product.supplierId);
        }
      });

      const suppliersHTML = database.suppliers.length
        ? database.suppliers.map(function(supplier) {
            return getSupplierChip(
              supplier,
              purchasedSuppliers.includes(supplier.id)
            );
          }).join("")
        : `<span class="muted">Nenhum fornecedor cadastrado.</span>`;

      const ordersHTML = stats.sales.length
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
                    ${sale.items.length} item(ns) ·
                    ${escapeHTML(sale.channel || "Canal não informado")} ·
                    Fornecedores:
                    ${getSaleSuppliers(sale)}
                  </div>

                  <div class="actions">
                    <button
                      class="button small"
                      onclick="openOrder('${sale.id}')">
                      Ver pedido
                    </button>

                    <button
                      class="button small primary"
                      onclick="downloadOrderPDF('${sale.id}')">
                      Baixar PDF
                    </button>
                  </div>
                </div>
              `;
            }).join("")
        : `<div class="empty">Este cliente ainda não possui pedidos.</div>`;

      const suggestionsHTML = suggestions.length
        ? suggestions.slice(0, 15).map(function(item) {
            return `
              <div class="list-item">
                <strong>${escapeHTML(item.product.name)}</strong>

                <div class="muted">
                  SKU: ${escapeHTML(item.product.sku)} ·
                  ${getABCBadge(item.curve)}
                  · ${item.supplier ? escapeHTML(item.supplier.name) : "Sem fornecedor"}
                </div>
              </div>
            `;
          }).join("")
        : `<div class="empty">Nenhuma sugestão disponível.</div>`;

      const lowerHTML = lowerPurchases.length
        ? lowerPurchases.map(function(item) {
            return `
              <div class="list-item">
                <strong>${escapeHTML(item.product.name)}</strong>

                <div class="muted">
                  Cliente comprou:
                  <strong>${item.clientQuantity}</strong> ·
                  Média dos clientes:
                  <strong>${item.average.toFixed(1)}</strong>
                </div>

                <div class="field" style="margin-top:9px">
                  <label>Motivo da compra menor</label>

                  <input
                    value="${escapeHTML(item.reason)}"
                    placeholder="Ex.: preço, baixa procura, preferência..."
                    onchange="saveLowerReason('${client.id}','${item.product.id}',this.value)">
                </div>
              </div>
            `;
          }).join("")
        : `<div class="empty">Nenhum produto abaixo da média.</div>`;

      document.getElementById("client-profile").innerHTML = `
        <div class="profile-header">
          <div>
            <button
              class="button small"
              onclick="showPage('clientes');renderAll()">
              ← Voltar
            </button>

            <h2 style="margin-top:14px">${escapeHTML(client.name)}</h2>

            <div class="muted">
              ${escapeHTML(client.phone || "Sem telefone")} ·
              ${escapeHTML(client.email || "Sem e-mail")} ·
              ${escapeHTML(client.city || "Sem cidade")}
            </div>
          </div>

          <div class="actions" style="margin-top:0">
            <button
              class="button primary"
              onclick="openSaleModal('${client.id}')">
              + Nova venda
            </button>

            <button
              class="button"
              onclick="document.getElementById('attachment-input').click()">
              Anexar arquivo
            </button>

            <input
              id="attachment-input"
              type="file"
              hidden
              onchange="saveAttachment('${client.id}', this.files[0])">
          </div>
        </div>

        <div class="cards">
          <div class="card">
            <div class="metric-label">Pedidos</div>
            <div class="metric-value">${stats.sales.length}</div>
          </div>

          <div class="card">
            <div class="metric-label">Itens comprados</div>
            <div class="metric-value">${stats.items}</div>
          </div>

          <div class="card">
            <div class="metric-label">Faturamento</div>
            <div class="metric-value green">${money(stats.revenue)}</div>
          </div>

          <div class="card">
            <div class="metric-label">Status</div>
            <div class="metric-value" style="font-size:17px">
              ${getClientStatus(client)}
            </div>
          </div>
        </div>

        <div class="profile-columns">
          <div>
            <div class="panel">
              <h2>Fornecedores do cliente</h2>

              <div class="chips">
                ${suppliersHTML}
              </div>

              <div class="muted" style="margin-top:12px">
                Colorido: fornecedor já comprado.
                Cinza: fornecedor ainda não comprado.
              </div>
            </div>

            <div class="panel">
              <h2>Histórico de pedidos</h2>
              <div class="list">${ordersHTML}</div>
            </div>

            <div class="panel">
              <h2>Anexos</h2>
              ${renderAttachments(client.id)}
            </div>
          </div>

          <div>
            <div class="panel">
              <h2>Oportunidades de expansão</h2>

              <div class="muted" style="margin-bottom:12px">
                Produtos que o cliente ainda não comprou, priorizados pela Curva ABC.
              </div>

              <div class="list">${suggestionsHTML}</div>
            </div>

            <div class="panel">
              <h2>Compras abaixo da média</h2>

              <div class="muted" style="margin-bottom:12px">
                Identifique por que o cliente comprou menos que os demais clientes.
              </div>

              <div class="list">${lowerHTML}</div>
            </div>
          </div>
        </div>
      `;

      showPage("profile");
    }

    function getSaleSuppliers(sale) {
      const suppliers = [];

      sale.items.forEach(function(item) {
        const product = getProduct(item.productId);

        if (!product) return;

        const supplier = getSupplier(product.supplierId);

        if (supplier && !suppliers.includes(supplier.name)) {
          suppliers.push(supplier.name);
        }
      });

      return suppliers.map(escapeHTML).join(", ") || "—";
    }

    function saveLowerReason(clientId, productId, reason) {
      const existing = database.lowerReasons.find(function(item) {
        return item.clientId === clientId &&
          item.productId === productId;
      });

      if (existing) {
        existing.reason = reason;
      } else {
        database.lowerReasons.push({
          id: id("reason"),
          clientId: clientId,
          productId: productId,
          reason: reason
        });
      }

      saveDatabase();
    }

    function renderAttachments(clientId) {
      const files = database.attachments.filter(function(file) {
        return file.clientId === clientId;
      });

      if (!files.length) {
        return `<div class="empty">Nenhum anexo cadastrado.</div>`;
      }

      return `
        <div class="list">
          ${files.map(function(file) {
            return `
              <div class="list-item">
                <strong>${escapeHTML(file.name)}</strong>

                <div class="muted">
                  Adicionado em ${dateBR(file.date)}
                </div>

                <div class="actions">
                  <a
                    class="button small"
                    href="${file.data}"
                    download="${escapeHTML(file.name)}">
                    Baixar
                  </a>

                  <button
                    class="button small danger"
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

    function saveAttachment(clientId, file) {
      if (!file) return;

      const reader = new FileReader();

      reader.onload = function() {
        database.attachments.push({
          id: id("file"),
          clientId: clientId,
          name: file.name,
          type: file.type,
          size: file.size,
          data: reader.result,
          date: today()
        });

        saveDatabase();
        openClientProfile(clientId);
      };

      reader.readAsDataURL(file);
    }

    function deleteAttachment(fileId, clientId) {
      if (!confirm("Excluir este anexo?")) {
        return;
      }

      database.attachments = database.attachments.filter(function(file) {
        return file.id !== fileId;
      });

      saveDatabase();
      openClientProfile(clientId);
    }

    function getWarrantyPendencies() {
      const pendencies = [];

      database.sales.forEach(function(sale) {
        sale.items.forEach(function(item) {
          if (!item.warrantyActive) return;

          const product = getProduct(item.productId);
          const client = getClient(sale.clientId);

          if (product && client) {
            pendencies.push({
              client: client,
              product: product,
              sale: sale
            });
          }
        });
      });

      return pendencies;
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

            ${database.suppliers.map(function(supplier) {
              return `
                <option value="${supplier.id}">
                  ${escapeHTML(supplier.name)}
                </option>
              `;
            }).join("")}
          </select>
        </div>

        <div class="field product-field">
          <label>Produto / SKU *</label>

          <select class="sale-product" onchange="updateSaleTotal()" disabled>
            <option value="">Selecione o fornecedor primeiro...</option>
          </select>
        </div>

        <div class="field">
          <label>Quantidade</label>

          <input
            class="sale-quantity"
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

    function updateLineProducts(supplierSelect) {
      const line = supplierSelect.closest(".sale-line");
      const productSelect = line.querySelector(".sale-product");
      const supplierId = supplierSelect.value;

      const products = database.products.filter(function(product) {
        return product.supplierId === supplierId;
      });

      productSelect.disabled = !supplierId;

      productSelect.innerHTML = supplierId
        ? `
          <option value="">Selecione o produto...</option>
          ${products.map(function(product) {
            return `
              <option value="${product.id}">
                ${escapeHTML(product.sku)} — ${escapeHTML(product.name)}
                (${money(product.price)})
              </option>
            `;
          }).join("")}
        `
        : `<option value="">Selecione o fornecedor primeiro...</option>`;

      updateSaleTotal();
    }

    function updateSaleTotal() {
      let total = 0;

      document.querySelectorAll(".sale-line").forEach(function(line) {
        const product = getProduct(line.querySelector(".sale-product")?.value);
        const quantity = Number(line.querySelector(".sale-quantity")?.value || 0);
        const lineTotal = product ? product.price * quantity : 0;

        total += lineTotal;

        const display = line.querySelector(".line-total");

        if (display) {
          display.textContent = money(lineTotal);
        }
      });

      document.getElementById("sale-total").textContent = money(total);
    }

    document.getElementById("sale-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const clientId = document.getElementById("sale-client").value;
      const items = [];

      document.querySelectorAll(".sale-line").forEach(function(line) {
        const supplierId = line.querySelector(".sale-supplier").value;
        const productId = line.querySelector(".sale-product").value;
        const quantity = Number(line.querySelector(".sale-quantity").value || 0);
        const product = getProduct(productId);

        if (!supplierId || !product || quantity <= 0) {
          return;
        }

        if (product.supplierId !== supplierId) {
          alert("O fornecedor selecionado não corresponde ao produto.");
          return;
        }

        items.push({
          productId: product.id,
          supplierId: supplierId,
          sku: product.sku,
          quantity: quantity,
          price: product.price,
          warrantyActive: false,
          warrantyStart: "",
          warrantyEnd: ""
        });
      });

      if (!clientId) {
        alert("Selecione o cliente.");
        return;
      }

      if (!items.length) {
        alert("Adicione pelo menos um item válido.");
        return;
      }

      database.sales.push({
        id: id("sale"),
        clientId: clientId,
        date: document.getElementById("sale-date").value,
        seller: document.getElementById("sale-seller").value.trim(),
        channel: document.getElementById("sale-channel").value,
        notes: document.getElementById("sale-notes").value.trim(),
        items: items
      });

      saveDatabase();
      closeModal("sale-modal");
      renderAll();

      alert("Venda registrada com sucesso.");
    });

    function openOrder(saleId) {
      const sale = database.sales.find(function(item) {
        return item.id === saleId;
      });

      if (!sale) return;

      const client = getClient(sale.clientId);

      const rows = sale.items.map(function(item) {
        const product = getProduct(item.productId);
        const supplier = getSupplier(item.supplierId);

        return `
          <tr>
            <td>
              <strong>${escapeHTML(product?.name || "Produto removido")}</strong>
              <br>
              <span class="muted">SKU: ${escapeHTML(item.sku || product?.sku || "—")}</span>
            </td>

            <td>${supplier ? getSupplierChip(supplier, true) : "—"}</td>
            <td>${item.quantity}</td>
            <td>${money(item.price)}</td>
            <td class="green">${money(item.quantity * item.price)}</td>
            <td>
              ${
                item.warrantyActive
                  ? `<span class="badge badge-active">Ativa</span>`
                  : `<span class="badge badge-inactive">Inativa</span>`
              }
            </td>
          </tr>
        `;
      }).join("");

      document.getElementById("order-details").innerHTML = `
        <div class="card">
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

        <div class="table-container" style="margin-top:15px">
          <table>
            <thead>
              <tr>
                <th>Produto</th>
                <th>Fornecedor</th>
                <th>Quantidade</th>
                <th>Preço</th>
                <th>Total</th>
                <th>Garantia</th>
              </tr>
            </thead>
            <tbody>${rows}</tbody>
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

        <div class="actions">
          <button
            class="button primary"
            onclick="downloadOrderPDF('${sale.id}')">
            Baixar pedido em PDF
          </button>

          <button
            class="button"
            onclick="closeModal('order-modal')">
            Fechar
          </button>
        </div>
      `;

      document.getElementById("order-modal").classList.add("open");
    }

    function downloadOrderPDF(saleId) {
      const sale = database.sales.find(function(item) {
        return item.id === saleId;
      });

      if (!sale) return;

      const client = getClient(sale.clientId);
      const PDF = window.jspdf?.jsPDF;

      if (!PDF) {
        alert("A biblioteca de PDF não foi carregada. Verifique a conexão.");
        return;
      }

      const documentPDF = new PDF();
      let y = 20;

      documentPDF.setFillColor(229, 9, 20);
      documentPDF.rect(0, 0, 210, 10, "F");

      documentPDF.setTextColor(0, 0, 0);
      documentPDF.setFontSize(18);
      documentPDF.text("PEDIDO COMERCIAL", 15, y);

      y += 10;
      documentPDF.setFontSize(10);

      documentPDF.text("Cliente: " + (client?.name || "—"), 15, y);
      y += 6;

      documentPDF.text("Telefone: " + (client?.phone || "—"), 15, y);
      y += 6;

      documentPDF.text("Data: " + dateBR(sale.date), 15, y);
      y += 6;

      documentPDF.text(
        "Vendedor: " + (sale.seller || "—") +
        " | Canal: " + (sale.channel || "—"),
        15,
        y
      );

      y += 12;

      documentPDF.setFillColor(40, 40, 40);
      documentPDF.setTextColor(255, 255, 255);
      documentPDF.rect(15, y - 5, 180, 8, "F");

      documentPDF.text("Produto / SKU", 18, y);
      documentPDF.text("Fornecedor", 95, y);
      documentPDF.text("Qtd.", 135, y);
      documentPDF.text("Total", 173, y);

      y += 9;
      documentPDF.setTextColor(0, 0, 0);
      documentPDF.setFontSize(9);

      sale.items.forEach(function(item) {
        const product = getProduct(item.productId);
        const supplier = getSupplier(item.supplierId);
        const productText = (product?.name || "Produto removido") +
          " / " +
          (item.sku || "—");

        documentPDF.text(productText.substring(0, 42), 18, y);
        documentPDF.text((supplier?.name || "—").substring(0, 22), 95, y);
        documentPDF.text(String(item.quantity), 137, y);
        documentPDF.text(money(item.quantity * item.price), 173, y);

        y += 7;

        if (y > 270) {
          documentPDF.addPage();
          y = 20;
        }
      });

      y += 8;
      documentPDF.setFontSize(13);
      documentPDF.text("TOTAL: " + money(getSaleTotal(sale)), 145, y);

      if (sale.notes) {
        y += 12;
        documentPDF.setFontSize(10);
        documentPDF.text("Observações:", 15, y);
        y += 6;

        const notes = documentPDF.splitTextToSize(sale.notes, 175);
        documentPDF.text(notes, 15, y);
      }

      const filename = (client?.name || "cliente")
        .replace(/[^a-z0-9]/gi, "-")
        .toLowerCase();

      documentPDF.save("pedido-" + filename + "-" + sale.date + ".pdf");
    }

    document.getElementById("settings-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.settings.monthlyGoal = Number(document.getElementById("monthly-goal").value || 0);
      database.settings.dailyGoal = Number(document.getElementById("daily-goal").value || 0);

      saveDatabase();
      closeModal("settings-modal");
      renderDashboard();

      alert("Meta atualizada com sucesso.");
    });

    function openSettingsModal() {
      document.getElementById("monthly-goal").value = database.settings.monthlyGoal || "";
      document.getElementById("daily-goal").value = database.settings.dailyGoal || "";
      document.getElementById("settings-modal").classList.add("open");
    }

    function sendBirthdayMessage(clientId) {
      const client = getClient(clientId);

      if (!client) return;

      if (!client.phone) {
        alert("Esse cliente não possui telefone cadastrado.");
        return;
      }

      const cleanPhone = client.phone.replace(/\D/g, "");

      const message = encodeURIComponent(
        "Olá, " + client.name + "! Desejamos um feliz aniversário, muita saúde e sucesso!"
      );

      window.open("https://wa.me/55" + cleanPhone + "?text=" + message, "_blank");
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

    renderAll();
  </script>
</body>
</html>
