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
      --info-bg: #dbeafe;
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
      width: 245px;
      background: var(--primary-dark);
      color: white;
      padding: 22px 14px;
      position: fixed;
      inset: 0 auto 0 0;
      z-index: 5;
    }

    .brand {
      font-size: 21px;
      font-weight: bold;
      padding: 0 12px 24px;
      border-bottom: 1px solid rgba(255, 255, 255, 0.2);
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
      width: calc(100% - 245px);
      margin-left: 245px;
      padding: 26px;
    }

    .topbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
      margin-bottom: 24px;
    }

    .topbar h1 {
      font-size: 28px;
    }

    .date {
      color: var(--muted);
      font-size: 14px;
      margin-top: 5px;
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

    .card,
    .form-card,
    .table-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 12px;
      box-shadow: var(--shadow);
    }

    .card {
      padding: 19px;
    }

    .form-card,
    .table-card {
      padding: 20px;
      margin-bottom: 20px;
    }

    .indicator-title {
      color: var(--muted);
      font-size: 14px;
      margin-bottom: 9px;
    }

    .indicator-value {
      font-size: 27px;
      font-weight: bold;
    }

    .section-title {
      font-size: 21px;
      margin-bottom: 15px;
    }

    .sub-title {
      font-size: 17px;
      margin: 20px 0 12px;
    }

    .grid-2 {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 18px;
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
      color: #374151;
      font-size: 13px;
      font-weight: bold;
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

    .search {
      margin-bottom: 15px;
    }

    .table-wrapper {
      overflow-x: auto;
    }

    table {
      width: 100%;
      min-width: 700px;
      border-collapse: collapse;
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
      color: var(--muted);
      font-size: 12px;
      text-transform: uppercase;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      padding: 5px 8px;
      border-radius: 999px;
      font-size: 12px;
      font-weight: bold;
      white-space: nowrap;
    }

    .badge-green {
      color: var(--success);
      background: var(--success-bg);
    }

    .badge-yellow {
      color: var(--warning);
      background: var(--warning-bg);
    }

    .badge-red {
      color: var(--danger);
      background: var(--danger-bg);
    }

    .badge-blue {
      color: var(--primary);
      background: var(--info-bg);
    }

    .badge-gray {
      color: #4b5563;
      background: var(--gray-bg);
    }

    .alert-list {
      display: grid;
      gap: 10px;
    }

    .alert-item {
      padding: 13px;
      border-left: 5px solid var(--warning);
      border-radius: 6px;
      background: var(--warning-bg);
    }

    .alert-item strong {
      display: block;
      margin-bottom: 5px;
    }

    .empty {
      padding: 18px 0;
      color: var(--muted);
      font-size: 14px;
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
      padding: 12px;
      border: 1px solid var(--border);
      border-radius: 8px;
      background: #f8fafc;
    }

    .timeline-item::before {
      content: "";
      position: absolute;
      left: -20px;
      top: 17px;
      width: 10px;
      height: 10px;
      border: 3px solid white;
      border-radius: 50%;
      background: var(--primary);
      box-shadow: 0 0 0 1px var(--primary);
    }

    .abc-bar {
      min-width: 120px;
      height: 9px;
      overflow: hidden;
      border-radius: 20px;
      background: #dbeafe;
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
      z-index: 20;
      align-items: center;
      justify-content: center;
      padding: 20px;
      background: rgba(15, 23, 42, 0.62);
    }

    .modal.open {
      display: flex;
    }

    .modal-content {
      width: min(1050px, 100%);
      max-height: 94vh;
      overflow-y: auto;
      padding: 23px;
      border-radius: 12px;
      background: white;
    }

    .modal-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      margin-bottom: 18px;
    }

    .close {
      border: 0;
      color: var(--muted);
      background: transparent;
      font-size: 27px;
    }

    .profile-header {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      gap: 12px;
      margin-bottom: 18px;
    }

    .profile-info {
      padding: 14px;
      border-radius: 8px;
      background: #f8fafc;
      border: 1px solid var(--border);
    }

    .product-sale-row {
      display: grid;
      grid-template-columns: 1fr 120px 150px;
      align-items: center;
      gap: 8px;
      margin-bottom: 8px;
      padding: 9px;
      border-radius: 7px;
      background: #f8fafc;
      border: 1px solid var(--border);
    }

    .status-active {
      color: var(--success);
      font-weight: bold;
    }

    .status-inactive {
      color: var(--muted);
    }

    .analysis-box {
      padding: 15px;
      border-radius: 8px;
      border: 1px solid var(--border);
      background: #f8fafc;
    }

    .analysis-box ul {
      padding-left: 20px;
      line-height: 1.9;
    }

    @media (max-width: 1100px) {
      .cards {
        grid-template-columns: repeat(2, 1fr);
      }

      .grid-2 {
        grid-template-columns: 1fr;
      }

      .profile-header {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 760px) {
      .layout {
        display: block;
      }

      .sidebar {
        position: relative;
        width: 100%;
        height: auto;
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

      .topbar {
        display: block;
      }

      .topbar .actions {
        margin-top: 14px;
      }

      .cards,
      .form-grid {
        grid-template-columns: 1fr;
      }

      .product-sale-row {
        grid-template-columns: 1fr;
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
        <button class="menu-btn" data-view="financeiro">Financeiro</button>
      </nav>
    </aside>

    <main class="content">
      <div class="topbar">
        <div>
          <h1 id="page-title">Dashboard</h1>
          <div id="current-date" class="date"></div>
        </div>

        <div class="actions">
          <button class="btn btn-success" onclick="carregarDadosFicticios()">
            Carregar dados fictícios
          </button>

          <button class="btn btn-outline" onclick="limparDados()">
            Limpar dados
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
            <div class="indicator-title">Vendas realizadas</div>
            <div class="indicator-value" id="indicator-vendas">0</div>
          </div>

          <div class="card">
            <div class="indicator-title">Faturamento</div>
            <div class="indicator-value" id="indicator-faturamento">
              R$ 0,00
            </div>
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
          <h2 class="section-title">Curva ABC geral dos produtos</h2>
          <p class="empty">
            A classificação considera o faturamento acumulado dos produtos.
            A = até 80%, B = até 95% e C = restante.
          </p>

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>ABC</th>
                  <th>Produto</th>
                  <th>Quantidade pedida</th>
                  <th>Faturamento</th>
                  <th>Participação</th>
                  <th>Status de demanda</th>
                </tr>
              </thead>

              <tbody id="abc-products-table"></tbody>
            </table>
          </div>
        </div>

        <div class="table-card">
          <h2 class="section-title">Curva ABC geral dos clientes</h2>

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>ABC</th>
                  <th>Cliente</th>
                  <th>Pedidos</th>
                  <th>Produtos pedidos</th>
                  <th>Faturamento</th>
                  <th>Participação</th>
                </tr>
              </thead>

              <tbody id="abc-clients-table"></tbody>
            </table>
          </div>
        </div>

        <div class="grid-2">
          <div class="table-card">
            <h2 class="section-title">Produtos menos pedidos</h2>

            <div class="table-wrapper">
              <table>
                <thead>
                  <tr>
                    <th>Produto</th>
                    <th>Quantidade</th>
                    <th>Clientes</th>
                    <th>Indicador</th>
                  </tr>
                </thead>

                <tbody id="low-demand-table"></tbody>
              </table>
            </div>
          </div>

          <div class="table-card">
            <h2 class="section-title">Análises gerais</h2>
            <div id="general-analysis" class="analysis-box"></div>
          </div>
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
                <label>Data de aniversário</label>
                <input id="client-birthday" type="date" />
              </div>

              <div class="form-group">
                <label>Empresa, cidade ou região</label>
                <input id="client-company" />
              </div>

              <div class="form-group full">
                <label>Observações</label>
                <textarea id="client-notes"></textarea>
              </div>
            </div>

            <button class="btn btn-primary">
              Cadastrar cliente
            </button>
          </form>
        </div>

        <div class="table-card">
          <h2 class="section-title">Clientes cadastrados</h2>

          <input
            id="client-search"
            class="search"
            placeholder="Pesquisar cliente..."
          />

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Nome</th>
                  <th>Telefone</th>
                  <th>Aniversário</th>
                  <th>Empresa/cidade</th>
                  <th>Pedidos</th>
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
                  <option value="">Selecione o fornecedor</option>
                </select>
              </div>

              <div class="form-group">
                <label>Categoria</label>
                <input id="product-category" />
              </div>

              <div class="form-group">
                <label>Preço unitário</label>
                <input
                  id="product-price"
                  type="number"
                  min="0"
                  step="0.01"
                  required
                />
              </div>
            </div>

            <button class="btn btn-primary">
              Cadastrar produto
            </button>
          </form>
        </div>

        <div class="table-card">
          <h2 class="section-title">Painel de produtos</h2>

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Código interno</th>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Categoria</th>
                  <th>Preço</th>
                  <th>Quantidade pedida</th>
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
                <label>CNPJ ou CPF</label>
                <input id="supplier-document" />
              </div>

              <div class="form-group">
                <label>Observações</label>
                <input id="supplier-notes" />
              </div>
            </div>

            <button class="btn btn-primary">
              Cadastrar fornecedor
            </button>
          </form>
        </div>

        <div class="table-card">
          <h2 class="section-title">Fornecedores cadastrados</h2>

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Fornecedor</th>
                  <th>Telefone</th>
                  <th>Documento</th>
                  <th>Produtos vinculados</th>
                  <th>Ações</th>
                </tr>
              </thead>

              <tbody id="suppliers-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- FINANCEIRO -->
      <section id="financeiro" class="view">
        <div class="form-card">
          <h2 class="section-title">Lançamento financeiro</h2>

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
                <input
                  id="finance-value"
                  type="number"
                  min="0"
                  step="0.01"
                  required
                />
              </div>

              <div class="form-group">
                <label>Vencimento</label>
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

            <button class="btn btn-primary">
              Salvar lançamento
            </button>
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

  <!-- MODAL DO PERFIL DO CLIENTE -->
  <div id="client-modal" class="modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2 id="client-modal-title">Perfil do cliente</h2>

        <button class="close" onclick="fecharModalCliente()">
          &times;
        </button>
      </div>

      <div id="client-profile-content"></div>
    </div>
  </div>

  <script>
    const STORAGE_KEY = "gestao_comercial_corrigido_v1";

    let banco = JSON.parse(localStorage.getItem(STORAGE_KEY)) || {
      clientes: [],
      produtos: [],
      fornecedores: [],
      vendas: [],
      financeiro: []
    };

    let clienteAbertoId = null;

    function salvar() {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(banco));
    }

    function id(prefixo) {
      return prefixo + "_" + Date.now() + "_" +
        Math.random().toString(36).substring(2, 8);
    }

    function moeda(valor) {
      return Number(valor || 0).toLocaleString("pt-BR", {
        style: "currency",
        currency: "BRL"
      });
    }

    function dataAtual() {
      const agora = new Date();
      const dois = numero => String(numero).padStart(2, "0");

      return `${agora.getFullYear()}-${dois(agora.getMonth() + 1)}-${dois(agora.getDate())}`;
    }

    function dataFormatada(data) {
      if (!data) return "-";

      return new Date(data + "T00:00:00").toLocaleDateString("pt-BR");
    }

    function dataHoraFormatada(data) {
      if (!data) return "-";

      return new Date(data).toLocaleString("pt-BR");
    }

    function htmlSeguro(texto) {
      return String(texto || "")
        .replaceAll("&", "&")
        .replaceAll("<", "<")
        .replaceAll(">", ">")
        .replaceAll('"', "&quot;")
        .replaceAll("'", "&#039;");
    }

    function obterCliente(clienteId) {
      return banco.clientes.find(cliente => cliente.id === clienteId);
    }

    function obterProduto(produtoId) {
      return banco.produtos.find(produto => produto.id === produtoId);
    }

    function obterFornecedor(fornecedorId) {
      return banco.fornecedores.find(
        fornecedor => fornecedor.id === fornecedorId
      );
    }

    function gerarCodigoProduto() {
      const maiorCodigo = banco.produtos.reduce((maior, produto) => {
        const numero = parseInt(
          String(produto.codigoInterno || "").replace(/\D/g, ""),
          10
        );

        return Number.isFinite(numero) && numero > maior ? numero : maior;
      }, 0);

      return `P-${String(maiorCodigo + 1).padStart(5, "0")}`;
    }

    function adicionarTimeline(clienteId, tipo, descricao, dados = {}) {
      const cliente = obterCliente(clienteId);

      if (!cliente) return;

      if (!cliente.timeline) {
        cliente.timeline = [];
      }

      cliente.timeline.unshift({
        id: id("timeline"),
        data: new Date().toISOString(),
        tipo,
        descricao,
        dados
      });
    }

    function mostrarAviso(mensagem) {
      alert(mensagem);
    }

    function quantidadePedidosCliente(clienteId) {
      return banco.vendas.filter(venda => venda.clienteId === clienteId).length;
    }

    function quantidadeProdutoGeral(produtoId) {
      return banco.vendas.reduce((total, venda) => {
        const item = venda.itens.find(
          itemVenda => itemVenda.produtoId === produtoId
        );

        return total + (item ? Number(item.quantidade) : 0);
      }, 0);
    }

    function quantidadeProdutoCliente(clienteId, produtoId) {
      return banco.vendas.reduce((total, venda) => {
        if (venda.clienteId !== clienteId) return total;

        const item = venda.itens.find(
          itemVenda => itemVenda.produtoId === produtoId
        );

        return total + (item ? Number(item.quantidade) : 0);
      }, 0);
    }

    function clientesQuePediramProduto(produtoId) {
      return new Set(
        banco.vendas
          .filter(venda =>
            venda.itens.some(item => item.produtoId === produtoId)
          )
          .map(venda => venda.clienteId)
      ).size;
    }

    function totalVenda(venda) {
      return venda.itens.reduce((total, item) => {
        const produto = obterProduto(item.produtoId);

        return total + (
          Number(item.quantidade) * Number(produto?.preco || 0)
        );
      }, 0);
    }

    function faturamentoGeral() {
      return banco.vendas.reduce(
        (total, venda) => total + totalVenda(venda),
        0
      );
    }

    function analiseProdutosGeral() {
      const produtos = banco.produtos.map(produto => {
        const quantidade = quantidadeProdutoGeral(produto.id);
        const faturamento = quantidade * Number(produto.preco || 0);
        const clientes = clientesQuePediramProduto(produto.id);

        return {
          produto,
          quantidade,
          faturamento,
          clientes
        };
      });

      produtos.sort((a, b) => b.faturamento - a.faturamento);

      const faturamentoTotal = produtos.reduce(
        (total, item) => total + item.faturamento,
        0
      );

      let acumulado = 0;

      return produtos.map(item => {
        const participacao = faturamentoTotal
          ? (item.faturamento / faturamentoTotal) * 100
          : 0;

        const classe = acumulado < 80
          ? "A"
          : acumulado < 95
            ? "B"
            : "C";

        acumulado += participacao;

        return {
          ...item,
          participacao,
          classe
        };
      });
    }

    function analiseClientesGeral() {
      const clientes = banco.clientes.map(cliente => {
        const vendas = banco.vendas.filter(
          venda => venda.clienteId === cliente.id
        );

        const produtosPedidos = new Set();

        vendas.forEach(venda => {
          venda.itens.forEach(item => {
            produtosPedidos.add(item.produtoId);
          });
        });

        return {
          cliente,
          pedidos: vendas.length,
          produtosPedidos: produtosPedidos.size,
          faturamento: vendas.reduce(
            (total, venda) => total + totalVenda(venda),
            0
          )
        };
      });

      clientes.sort((a, b) => b.faturamento - a.faturamento);

      const total = clientes.reduce(
        (soma, cliente) => soma + cliente.faturamento,
        0
      );

      let acumulado = 0;

      return clientes.map(item => {
        const participacao = total
          ? (item.faturamento / total) * 100
          : 0;

        const classe = acumulado < 80
          ? "A"
          : acumulado < 95
            ? "B"
            : "C";

        acumulado += participacao;

        return {
          ...item,
          participacao,
          classe
        };
      });
    }

    function classeABC(classe) {
      if (classe === "A") return "badge-green";
      if (classe === "B") return "badge-yellow";
      return "badge-red";
    }

    function statusDemanda(item) {
      if (item.quantidade === 0) {
        return '<span class="badge badge-red">Nunca pedido</span>';
      }

      if (item.quantidade <= 5) {
        return '<span class="badge badge-yellow">Baixa demanda</span>';
      }

      return '<span class="badge badge-green">Demanda registrada</span>';
    }

    function renderizarTudo() {
      renderizarIndicadores();
      renderizarSelects();
      renderizarClientes();
      renderizarProdutos();
      renderizarFornecedores();
      renderizarFinanceiro();
      renderizarGarantias();
      renderizarAniversarios();
      renderizarABCProdutos();
      renderizarABCClientes();
      renderizarProdutosMenosPedidos();
      renderizarAnaliseGeral();

      if (clienteAbertoId) {
        abrirPerfilCliente(clienteAbertoId, false);
      }
    }

    function renderizarIndicadores() {
      document.getElementById("indicator-clientes").textContent =
        banco.clientes.length;

      document.getElementById("indicator-produtos").textContent =
        banco.produtos.length;

      document.getElementById("indicator-vendas").textContent =
        banco.vendas.length;

      document.getElementById("indicator-faturamento").textContent =
        moeda(faturamentoGeral());
    }

    function renderizarSelects() {
      const selectFornecedor = document.getElementById("product-supplier");

      selectFornecedor.innerHTML =
        '<option value="">Selecione o fornecedor</option>' +
        banco.fornecedores.map(fornecedor => `
          <option value="${fornecedor.id}">
            ${htmlSeguro(fornecedor.nome)}
          </option>
        `).join("");
    }

    function renderizarClientes() {
      const termo = (
        document.getElementById("client-search")?.value || ""
      ).toLowerCase();

      const clientes = banco.clientes.filter(cliente =>
        cliente.nome.toLowerCase().includes(termo)
      );

      const tabela = document.getElementById("clients-table");

      if (!clientes.length) {
        tabela.innerHTML = `
          <tr>
            <td colspan="6" class="empty">
              Nenhum cliente cadastrado.
            </td>
          </tr>
        `;
        return;
      }

      tabela.innerHTML = clientes.map(cliente => `
        <tr>
          <td>
            <strong>${htmlSeguro(cliente.nome)}</strong>
          </td>

          <td>${htmlSeguro(cliente.telefone || "-")}</td>
          <td>${dataFormatada(cliente.aniversario)}</td>
          <td>${htmlSeguro(cliente.empresa || "-")}</td>
          <td>${quantidadePedidosCliente(cliente.id)}</td>

          <td>
            <div class="actions">
              <button
                class="btn btn-primary btn-small"
                onclick="abrirPerfilCliente('${cliente.id}')"
              >
                Abrir perfil e vender
              </button>

              ${
                cliente.telefone
                  ? `
                    <button
                      class="btn btn-success btn-small"
                      onclick="enviarWhatsApp('${cliente.id}')"
                    >
                      WhatsApp
                    </button>
                  `
                  : ""
              }

              <button
                class="btn btn-danger btn-small"
                onclick="excluirCliente('${cliente.id}')"
              >
                Excluir
              </button>
            </div>
          </td>
        </tr>
      `).join("");
    }

    function renderizarProdutos() {
      const tabela = document.getElementById("products-table");

      if (!banco.produtos.length) {
        tabela.innerHTML = `
          <tr>
            <td colspan="7" class="empty">
              Nenhum produto cadastrado.
            </td>
          </tr>
        `;
        return;
      }

      const analise = analiseProdutosGeral();

      tabela.innerHTML = banco.produtos.map(produto => {
        const fornecedor = obterFornecedor(produto.fornecedorId);
        const item = analise.find(
          resultado => resultado.produto.id === produto.id
        );

        return `
          <tr>
            <td>
              <span class="badge badge-gray">
                ${htmlSeguro(produto.codigoInterno)}
              </span>
            </td>

            <td><strong>${htmlSeguro(produto.nome)}</strong></td>
            <td>${htmlSeguro(fornecedor?.nome || "-")}</td>
            <td>${htmlSeguro(produto.categoria || "-")}</td>
            <td>${moeda(produto.preco)}</td>
            <td>${item?.quantidade || 0}</td>

            <td>
              <button
                class="btn btn-danger btn-small"
                onclick="excluirProduto('${produto.id}')"
              >
                Excluir
              </button>
            </td>
          </tr>
        `;
      }).join("");
    }

    function renderizarFornecedores() {
      const tabela = document.getElementById("suppliers-table");

      if (!banco.fornecedores.length) {
        tabela.innerHTML = `
          <tr>
            <td colspan="5" class="empty">
              Nenhum fornecedor cadastrado.
            </td>
          </tr>
        `;
        return;
      }

      tabela.innerHTML = banco.fornecedores.map(fornecedor => {
        const produtos = banco.produtos.filter(
          produto => produto.fornecedorId === fornecedor.id
        ).length;

        return `
          <tr>
            <td><strong>${htmlSeguro(fornecedor.nome)}</strong></td>
            <td>${htmlSeguro(fornecedor.telefone || "-")}</td>
            <td>${htmlSeguro(fornecedor.documento || "-")}</td>
            <td>${produtos}</td>

            <td>
              <button
                class="btn btn-danger btn-small"
                onclick="excluirFornecedor('${fornecedor.id}')"
              >
                Excluir
              </button>
            </td>
          </tr>
        `;
      }).join("");
    }

    function renderizarFinanceiro() {
      const tabela = document.getElementById("finance-table");

      if (!banco.financeiro.length) {
        tabela.innerHTML = `
          <tr>
            <td colspan="6" class="empty">
              Nenhum lançamento financeiro.
            </td>
          </tr>
        `;
      } else {
        tabela.innerHTML = banco.financeiro.map(item => `
          <tr>
            <td>
              ${
                item.tipo === "receber"
                  ? '<span class="badge badge-green">A receber</span>'
                  : '<span class="badge badge-red">A pagar</span>'
              }
            </td>

            <td>${htmlSeguro(item.descricao)}</td>
            <td>${moeda(item.valor)}</td>
            <td>${dataFormatada(item.vencimento)}</td>

            <td>
              ${
                item.status === "pago"
                  ? '<span class="badge badge-green">Pago</span>'
                  : '<span class="badge badge-yellow">Pendente</span>'
              }
            </td>

            <td>
              <button
                class="btn btn-danger btn-small"
                onclick="excluirFinanceiro('${item.id}')"
              >
                Excluir
              </button>
            </td>
          </tr>
        `).join("");
      }

      const receber = banco.financeiro
        .filter(item => item.tipo === "receber")
        .reduce((total, item) => total + Number(item.valor), 0);

      const pagar = banco.financeiro
        .filter(item => item.tipo === "pagar")
        .reduce((total, item) => total + Number(item.valor), 0);

      const resultado = receber - pagar;

      document.getElementById("dre-summary").innerHTML = `
        <div class="cards" style="grid-template-columns:repeat(3,1fr); margin:0;">
          <div class="card">
            <div class="indicator-title">Total a receber</div>
            <div class="indicator-value" style="color:var(--success);">
              ${moeda(receber)}
            </div>
          </div>

          <div class="card">
            <div class="indicator-title">Total a pagar</div>
            <div class="indicator-value" style="color:var(--danger);">
              ${moeda(pagar)}
            </div>
          </div>

          <div class="card">
            <div class="indicator-title">Resultado simplificado</div>
            <div
              class="indicator-value"
              style="color:${resultado >= 0 ? "var(--success)" : "var(--danger)"};"
            >
              ${moeda(resultado)}
            </div>
          </div>
        </div>
      `;
    }

    function renderizarGarantias() {
      const caixa = document.getElementById("warranty-alerts");
      const garantias = [];

      banco.vendas.forEach(venda => {
        const cliente = obterCliente(venda.clienteId);

        venda.itens.forEach(item => {
          if (!item.garantiaAtiva) return;

          const produto = obterProduto(item.produtoId);

          garantias.push({
            venda,
            item,
            cliente,
            produto
          });
        });
      });

      if (!garantias.length) {
        caixa.innerHTML = `
          <div class="empty">
            Nenhuma garantia ativa.
          </div>
        `;
        return;
      }

      caixa.innerHTML = garantias.map(garantia => `
        <div class="alert-item">
          <strong>
            Pendência: ${htmlSeguro(garantia.produto?.nome || "Produto")}
          </strong>

          <div>
            Cliente:
            ${htmlSeguro(garantia.cliente?.nome || "Cliente")}
          </div>

          <div style="margin-top:5px; font-size:13px;">
            Venda realizada em ${dataFormatada(garantia.venda.data)}
          </div>

          <div class="actions" style="margin-top:9px;">
            <span class="badge badge-green">Garantia ativa</span>

            <button
              class="btn btn-success btn-small"
              onclick="finalizarGarantia('${garantia.venda.id}', '${garantia.item.id}')"
            >
              Finalizar garantia
            </button>
          </div>
        </div>
      `).join("");
    }

    function renderizarAniversarios() {
      const caixa = document.getElementById("birthday-alerts");
      const hoje = new Date();

      const aniversariantes = banco.clientes.filter(cliente => {
        if (!cliente.aniversario) return false;

        const nascimento = new Date(
          cliente.aniversario + "T00:00:00"
        );

        return (
          nascimento.getDate() === hoje.getDate() &&
          nascimento.getMonth() === hoje.getMonth()
        );
      });

      if (!aniversariantes.length) {
        caixa.innerHTML = `
          <div class="empty">
            Nenhum aniversário hoje.
          </div>
        `;
        return;
      }

      caixa.innerHTML = aniversariantes.map(cliente => `
        <div
          class="alert-item"
          style="
            border-left-color:var(--success);
            background:var(--success-bg);
          "
        >
          <strong>
            Aniversário de ${htmlSeguro(cliente.nome)}
          </strong>

          <div>
            Cliente aniversariante hoje.
          </div>

          ${
            cliente.telefone
              ? `
                <button
                  class="btn btn-success btn-small"
                  style="margin-top:9px;"
                  onclick="enviarParabens('${cliente.id}')"
                >
                  Enviar parabéns
                </button>
              `
              : `
                <span class="badge badge-gray" style="margin-top:9px;">
                  Sem telefone cadastrado
                </span>
              `
          }
        </div>
      `).join("");
    }

    function renderizarABCProdutos() {
      const tabela = document.getElementById("abc-products-table");
      const analise = analiseProdutosGeral();

      if (!analise.length) {
        tabela.innerHTML = `
          <tr>
            <td colspan="6" class="empty">
              Cadastre produtos e lance vendas para gerar a análise.
            </td>
          </tr>
        `;
        return;
      }

      tabela.innerHTML = analise.map(item => `
        <tr>
          <td>
            <span class="badge ${classeABC(item.classe)}">
              ${item.classe}
            </span>
          </td>

          <td>
            <strong>${htmlSeguro(item.produto.nome)}</strong>
            <br />
            <small>${htmlSeguro(item.produto.codigoInterno)}</small>
          </td>

          <td>${item.quantidade}</td>
          <td>${moeda(item.faturamento)}</td>
          <td>${item.participacao.toFixed(1)}%</td>
          <td>${statusDemanda(item)}</td>
        </tr>
      `).join("");
    }

    function renderizarABCClientes() {
      const tabela = document.getElementById("abc-clients-table");
      const analise = analiseClientesGeral();

      if (!analise.length) {
        tabela.innerHTML = `
          <tr>
            <td colspan="6" class="empty">
              Cadastre clientes e lance vendas para gerar a análise.
            </td>
          </tr>
        `;
        return;
      }

      tabela.innerHTML = analise.map(item => `
        <tr>
          <td>
            <span class="badge ${classeABC(item.classe)}">
              ${item.classe}
            </span>
          </td>

          <td>${htmlSeguro(item.cliente.nome)}</td>
          <td>${item.pedidos}</td>
          <td>${item.produtosPedidos}</td>
          <td>${moeda(item.faturamento)}</td>
          <td>${item.participacao.toFixed(1)}%</td>
        </tr>
      `).join("");
    }

    function renderizarProdutosMenosPedidos() {
      const tabela = document.getElementById("low-demand-table");
      const analise = analiseProdutosGeral().sort(
        (a, b) => a.quantidade - b.quantidade
      );

      if (!analise.length) {
        tabela.innerHTML = `
          <tr>
            <td colspan="4" class="empty">
              Nenhum produto cadastrado.
            </td>
          </tr>
        `;
        return;
      }

      tabela.innerHTML = analise.map(item => `
        <tr>
          <td>${htmlSeguro(item.produto.nome)}</td>
          <td><strong>${item.quantidade}</strong></td>
          <td>${item.clientes}</td>
          <td>${statusDemanda(item)}</td>
        </tr>
      `).join("");
    }

    function renderizarAnaliseGeral() {
      const caixa = document.getElementById("general-analysis");
      const analise = analiseProdutosGeral();

      const nuncaPedidos = analise.filter(
        item => item.quantidade === 0
      ).length;

      const baixaDemanda = analise.filter(
        item => item.quantidade > 0 && item.quantidade <= 5
      ).length;

      const produtosClasseA = analise.filter(
        item => item.classe === "A"
      );

      const produtoMaisPedido = [...analise].sort(
        (a, b) => b.quantidade - a.quantidade
      )[0];

      const produtoMenosPedido = [...analise].sort(
        (a, b) => a.quantidade - b.quantidade
      )[0];

      caixa.innerHTML = `
        <ul>
          <li>
            <strong>Produtos nunca pedidos:</strong>
            ${nuncaPedidos}.
          </li>

          <li>
            <strong>Produtos com baixa demanda:</strong>
            ${baixaDemanda}.
          </li>

          <li>
            <strong>Produtos na curva A:</strong>
            ${produtosClasseA.length}.
          </li>

          <li>
            <strong>Produto mais pedido:</strong>
            ${
              produtoMaisPedido
                ? `${htmlSeguro(produtoMaisPedido.produto.nome)}
                   (${produtoMaisPedido.quantidade} unidades)`
                : "Nenhum"
            }.
          </li>

          <li>
            <strong>Produto menos pedido:</strong>
            ${
              produtoMenosPedido
                ? `${htmlSeguro(produtoMenosPedido.produto.nome)}
                   (${produtoMenosPedido.quantidade} unidades)`
                : "Nenhum"
            }.
          </li>
        </ul>
      `;
    }

    /*
      ABRE O PERFIL DO CLIENTE.

      É dentro desta tela que a venda é lançada.
      O painel de produtos continua existindo separadamente
      na aba "Produtos".
    */
    function abrirPerfilCliente(clienteId, abrirModal = true) {
      const cliente = obterCliente(clienteId);

      if (!cliente) return;

      clienteAbertoId = clienteId;

      const vendasCliente = banco.vendas.filter(
        venda => venda.clienteId === clienteId
      );

      const analiseGeral = analiseProdutosGeral();

      const produtosComprados = banco.produtos.filter(produto =>
        vendasCliente.some(venda =>
          venda.itens.some(item => item.produtoId === produto.id)
        )
      );

      const produtosNaoComprados = analiseGeral.filter(item =>
        item.classe !== "C" &&
        quantidadeProdutoCliente(clienteId, item.produto.id) === 0
      );

      const quantidadeTotalGeral = banco.clientes.length || 1;

      const produtosAbaixoDaMedia = analiseGeral.filter(item => {
        const quantidadeCliente = quantidadeProdutoCliente(
          clienteId,
          item.produto.id
        );

        const mediaPorCliente = item.quantidade / quantidadeTotalGeral;

        return (
          quantidadeCliente > 0 &&
          quantidadeCliente < mediaPorCliente
        );
      });

      const produtosParaVenda = banco.produtos;

      document.getElementById("client-modal-title").textContent =
        `Perfil do cliente: ${cliente.nome}`;

      document.getElementById("client-profile-content").innerHTML = `
        <div class="profile-header">
          <div class="profile-info">
            <strong>Cliente</strong>
            <div>${htmlSeguro(cliente.nome)}</div>
          </div>

          <div class="profile-info">
            <strong>Telefone</strong>
            <div>${htmlSeguro(cliente.telefone || "-")}</div>
          </div>

          <div class="profile-info">
            <strong>Total comprado</strong>
            <div>
              ${moeda(
                vendasCliente.reduce(
                  (total, venda) => total + totalVenda(venda),
                  0
                )
              )}
            </div>
          </div>
        </div>

        <div class="form-card" style="box-shadow:none; margin-bottom:20px;">
          <h3 class="sub-title">Lançar venda para este cliente</h3>

          <form id="sale-form">
            <div class="form-grid">
              <div class="form-group">
                <label>Vendedor</label>
                <input id="sale-seller" required />
              </div>

              <div class="form-group">
                <label>Canal da venda</label>
                <select id="sale-channel">
                  <option value="Presencial">Presencial</option>
                  <option value="WhatsApp">WhatsApp</option>
                  <option value="Telefone">Telefone</option>
                  <option value="E-mail">E-mail</option>
                </select>
              </div>

              <div class="form-group full">
                <label>Observação da venda</label>
                <input id="sale-notes" />
              </div>
            </div>

            <div class="form-group">
              <label>Selecione os produtos vendidos</label>

              <div id="sale-products-list">
                ${
                  produtosParaVenda.length
                    ? produtosParaVenda.map(produto => `
                      <div class="product-sale-row">
                        <label style="font-weight:normal;">
                          <input
                            type="checkbox"
                            class="sale-product-check"
                            value="${produto.id}"
                            style="width:auto; margin-right:7px;"
                          />
                          ${htmlSeguro(produto.nome)}
                          <small>
                            (${htmlSeguro(produto.codigoInterno)})
                          </small>
                        </label>

                        <input
                          type="number"
                          min="1"
                          value="1"
                          class="sale-product-quantity"
                          data-product-id="${produto.id}"
                          placeholder="Quantidade"
                        />

                        <label style="font-weight:normal;">
                          <input
                            type="checkbox"
                            class="sale-product-warranty"
                            data-product-id="${produto.id}"
                            style="width:auto; margin-right:5px;"
                          />
                          Ativar garantia
                        </label>
                      </div>
                    `).join("")
                    : `
                      <div class="empty">
                        Cadastre produtos antes de lançar uma venda.
                      </div>
                    `
                }
              </div>
            </div>

            ${
              produtosParaVenda.length
                ? `
                  <button class="btn btn-primary">
                    Salvar venda para ${htmlSeguro(cliente.nome)}
                  </button>
                `
                : ""
            }
          </form>
        </div>

        <div class="grid-2">
          <div class="table-card" style="box-shadow:none;">
            <h3 class="sub-title">
              Curva ABC geral x este cliente
            </h3>

            <p class="empty">
              Produtos da curva A e B que este cliente ainda não pediu.
            </p>

            ${
              produtosNaoComprados.length
                ? `
                  <div class="table-wrapper">
                    <table>
                      <thead>
                        <tr>
                          <th>ABC</th>
                          <th>Produto</th>
                          <th>Total geral</th>
                          <th>Situação</th>
                        </tr>
                      </thead>

                      <tbody>
                        ${produtosNaoComprados.map(item => `
                          <tr>
                            <td>
                              <span class="badge ${classeABC(item.classe)}">
                                ${item.classe}
                              </span>
                            </td>

                            <td>${htmlSeguro(item.produto.nome)}</td>
                            <td>${item.quantidade}</td>
                            <td>
                              <span class="badge badge-red">
                                Não pediu
                              </span>
                            </td>
                          </tr>
                        `).join("")}
                      </tbody>
                    </table>
                  </div>
                `
                : `
                  <div class="empty">
                    Este cliente já pediu todos os produtos relevantes
                    da curva A e B.
                  </div>
                `
            }
          </div>

          <div class="table-card" style="box-shadow:none;">
            <h3 class="sub-title">
              Produtos abaixo da média geral
            </h3>

            <p class="empty">
              Produtos que o cliente já pediu, mas em quantidade inferior
              à média por cliente.
            </p>

            ${
              produtosAbaixoDaMedia.length
                ? `
                  <div class="table-wrapper">
                    <table>
                      <thead>
                        <tr>
                          <th>Produto</th>
                          <th>Cliente</th>
                          <th>Média geral</th>
                          <th>Situação</th>
                        </tr>
                      </thead>

                      <tbody>
                        ${produtosAbaixoDaMedia.map(item => {
                          const quantidadeCliente =
                            quantidadeProdutoCliente(
                              clienteId,
                              item.produto.id
                            );

                          const media =
                            item.quantidade / quantidadeTotalGeral;

                          return `
                            <tr>
                              <td>${htmlSeguro(item.produto.nome)}</td>
                              <td>${quantidadeCliente}</td>
                              <td>${media.toFixed(1)}</td>
                              <td>
                                <span class="badge badge-yellow">
                                  Abaixo da média
                                </span>
                              </td>
                            </tr>
                          `;
                        }).join("")}
                      </tbody>
                    </table>
                  </div>
                `
                : `
                  <div class="empty">
                    Nenhum produto abaixo da média geral.
                  </div>
                `
            }
          </div>
        </div>

        <div class="table-card" style="box-shadow:none;">
          <h3 class="sub-title">
            Produtos comprados por este cliente
          </h3>

          <div class="table-wrapper">
            <table>
              <thead>
                <tr>
                  <th>Produto</th>
                  <th>Quantidade total</th>
                  <th>Garantia ativa</th>
                  <th>Histórico</th>
                </tr>
              </thead>

              <tbody>
                ${
                  produtosComprados.length
                    ? produtosComprados.map(produto => {
                      const quantidade =
                        quantidadeProdutoCliente(
                          clienteId,
                          produto.id
                        );

                      const garantiaAtiva =
                        banco.vendas.some(venda =>
                          venda.clienteId === clienteId &&
                          venda.itens.some(item =>
                            item.produtoId === produto.id &&
                            item.garantiaAtiva
                          )
                        );

                      return `
                        <tr>
                          <td>${htmlSeguro(produto.nome)}</td>
                          <td>${quantidade}</td>
                          <td>
                            ${
                              garantiaAtiva
                                ? '<span class="badge badge-green">Ativa</span>'
                                : '<span class="badge badge-gray">Inativa</span>'
                            }
                          </td>
                          <td>
                            <button
                              class="btn btn-outline btn-small"
                              onclick="verHistoricoProdutoCliente(
                                '${clienteId}',
                                '${produto.id}'
                              )"
                            >
                              Ver timeline
                            </button>
                          </td>
                        </tr>
                      `;
                    }).join("")
                    : `
                      <tr>
                        <td colspan="4" class="empty">
                          Este cliente ainda não possui compras.
                        </td>
                      </tr>
                    `
                }
              </tbody>
            </table>
          </div>
        </div>

        <div class="table-card" style="box-shadow:none;">
          <h3 class="sub-title">Timeline do cliente</h3>

          ${
            cliente.timeline?.length
              ? `
                <div class="timeline">
                  ${cliente.timeline.map(evento => `
                    <div class="timeline-item">
                      <strong>${htmlSeguro(evento.tipo)}</strong>
                      <div style="margin-top:5px;">
                        ${htmlSeguro(evento.descricao)}
                      </div>
                      <small
                        style="
                          display:block;
                          margin-top:7px;
                          color:var(--muted);
                        "
                      >
                        ${dataHoraFormatada(evento.data)}
                      </small>
                    </div>
                  `).join("")}
                </div>
              `
              : `
                <div class="empty">
                  Nenhum evento registrado.
                </div>
              `
          }
        </div>
      `;

      document
        .getElementById("sale-form")
        ?.addEventListener("submit", event => {
          event.preventDefault();
          salvarVendaDentroDoCliente(clienteId);
        });

      if (abrirModal) {
        document.getElementById("client-modal").classList.add("open");
      }
    }

    function salvarVendaDentroDoCliente(clienteId) {
      const cliente = obterCliente(clienteId);

      if (!cliente) return;

      const vendedor = document.getElementById("sale-seller").value.trim();
      const canal = document.getElementById("sale-channel").value;
      const observacao = document.getElementById("sale-notes").value.trim();

      const selecionados = Array.from(
        document.querySelectorAll(".sale-product-check:checked")
      );

      if (!vendedor) {
        mostrarAviso("Informe o vendedor.");
        return;
      }

      if (!selecionados.length) {
        mostrarAviso("Selecione pelo menos um produto.");
        return;
      }

      const itens = selecionados.map(selecionado => {
        const produtoId = selecionado.value;

        const campoQuantidade = document.querySelector(
          `.sale-product-quantity[data-product-id="${produtoId}"]`
        );

        const campoGarantia = document.querySelector(
          `.sale-product-warranty[data-product-id="${produtoId}"]`
        );

        const quantidade = Math.max(
          1,
          Number(campoQuantidade.value) || 1
        );

        return {
          id: id("item"),
          produtoId,
          quantidade,
          garantiaAtiva: campoGarantia.checked,
          garantiaAtivadaEm: campoGarantia.checked
            ? new Date().toISOString()
            : null
        };
      });

      const venda = {
        id: id("venda"),
        clienteId,
        vendedor,
        canal,
        observacao,
        data: dataAtual(),
        criadoEm: new Date().toISOString(),
        itens
      };

      banco.vendas.unshift(venda);

      adicionarTimeline(
        clienteId,
        "Venda lançada",
        `Venda lançada pelo vendedor ${vendedor}, pelo canal ${canal}.`,
        { vendaId: venda.id }
      );

      itens.forEach(item => {
        if (!item.garantiaAtiva) return;

        const produto = obterProduto(item.produtoId);

        adicionarTimeline(
          clienteId,
          "Garantia ativada",
          `Garantia ativada para ${produto?.nome || "produto"}.`,
          {
            vendaId: venda.id,
            produtoId: item.produtoId
          }
        );
      });

      salvar();
      renderizarTudo();

      mostrarAviso("Venda lançada com sucesso.");
    }

    function verHistoricoProdutoCliente(clienteId, produtoId) {
      const cliente = obterCliente(clienteId);
      const produto = obterProduto(produtoId);

      if (!cliente || !produto) return;

      const vendas = banco.vendas.filter(venda =>
        venda.clienteId === clienteId &&
        venda.itens.some(item => item.produtoId === produtoId)
      );

      const eventos = [];

      vendas.forEach(venda => {
        const item = venda.itens.find(
          itemVenda => itemVenda.produtoId === produtoId
        );

        eventos.push(`
          <div class="timeline-item">
            <strong>Venda de produto</strong>
            <div style="margin-top:5px;">
              ${item.quantidade} unidade(s) de
              ${htmlSeguro(produto.nome)}
            </div>
            <div style="margin-top:5px;">
              Vendedor: ${htmlSeguro(venda.vendedor)}
            </div>
            <div style="margin-top:5px;">
              ${
                item.garantiaAtiva
                  ? '<span class="badge badge-green">Garantia ativa</span>'
                  : '<span class="badge badge-gray">Garantia inativa</span>'
              }
            </div>
            <small
              style="
                display:block;
                margin-top:7px;
                color:var(--muted);
              "
            >
              ${dataFormatada(venda.data)}
            </small>
          </div>
        `);
      });

      const conteudo = `
        <div class="modal open" style="z-index:30;">
          <div class="modal-content" style="max-width:700px;">
            <div class="modal-header">
              <h2>
                Histórico: ${htmlSeguro(produto.nome)}
              </h2>

              <button
                class="close"
                onclick="this.closest('.modal').remove()"
              >
                &times;
              </button>
            </div>

            <div class="timeline">
              ${
                eventos.length
                  ? eventos.join("")
                  : '<div class="empty">Nenhum lançamento.</div>'
              }
            </div>
          </div>
        </div>
      `;

      document.body.insertAdjacentHTML("beforeend", conteudo);
    }

    function fecharModalCliente() {
      document.getElementById("client-modal").classList.remove("open");
      clienteAbertoId = null;
    }

    function finalizarGarantia(vendaId, itemId) {
      const venda = banco.vendas.find(vendaItem => vendaItem.id === vendaId);

      if (!venda) return;

      const item = venda.itens.find(itemVenda => itemVenda.id === itemId);

      if (!item) return;

      item.garantiaAtiva = false;
      item.garantiaFinalizadaEm = new Date().toISOString();

      const produto = obterProduto(item.produtoId);

      adicionarTimeline(
        venda.clienteId,
        "Garantia finalizada",
        `Garantia finalizada para ${produto?.nome || "produto"}.`,
        {
          vendaId,
          produtoId: item.produtoId
        }
      );

      salvar();
      renderizarTudo();
    }

    function enviarWhatsApp(clienteId) {
      const cliente = obterCliente(clienteId);

      if (!cliente?.telefone) {
        mostrarAviso("Este cliente não possui telefone.");
        return;
      }

      const telefone = cliente.telefone.replace(/\D/g, "");

      const mensagem =
        `Olá, ${cliente.nome}! Entramos em contato para falar sobre seu atendimento.`;

      window.open(
        `https://wa.me/55${telefone}?text=${encodeURIComponent(mensagem)}`,
        "_blank"
      );
    }

    function enviarParabens(clienteId) {
      const cliente = obterCliente(clienteId);

      if (!cliente?.telefone) {
        mostrarAviso("Este cliente não possui telefone.");
        return;
      }

      const telefone = cliente.telefone.replace(/\D/g, "");

      const mensagem =
        `Olá, ${cliente.nome}! Desejamos a você um feliz aniversário, com muita saúde, felicidade e sucesso!`;

      window.open(
        `https://wa.me/55${telefone}?text=${encodeURIComponent(mensagem)}`,
        "_blank"
      );

      adicionarTimeline(
        clienteId,
        "Contato de aniversário",
        "Mensagem de parabéns preparada para envio pelo WhatsApp."
      );

      salvar();
      renderizarTudo();
    }

    function excluirCliente(clienteId) {
      if (!confirm("Deseja excluir este cliente?")) return;

      banco.clientes = banco.clientes.filter(
        cliente => cliente.id !== clienteId
      );

      banco.vendas = banco.vendas.filter(
        venda => venda.clienteId !== clienteId
      );

      salvar();
      renderizarTudo();
    }

    function excluirProduto(produtoId) {
      if (!confirm("Deseja excluir este produto?")) return;

      banco.produtos = banco.produtos.filter(
        produto => produto.id !== produtoId
      );

      salvar();
      renderizarTudo();
    }

    function excluirFornecedor(fornecedorId) {
      if (!confirm("Deseja excluir este fornecedor?")) return;

      banco.fornecedores = banco.fornecedores.filter(
        fornecedor => fornecedor.id !== fornecedorId
      );

      salvar();
      renderizarTudo();
    }

    function excluirFinanceiro(financeiroId) {
      if (!confirm("Deseja excluir este lançamento?")) return;

      banco.financeiro = banco.financeiro.filter(
        item => item.id !== financeiroId
      );

      salvar();
      renderizarTudo();
    }

    function limparDados() {
      if (!confirm("Deseja apagar todos os dados deste navegador?")) {
        return;
      }

      localStorage.removeItem(STORAGE_KEY);
      location.reload();
    }

    function escolherPonderado(lista) {
      const total = lista.reduce(
        (soma, item) => soma + item.peso,
        0
      );

      let sorteio = Math.random() * total;

      for (const item of lista) {
        sorteio -= item.peso;

        if (sorteio <= 0) {
          return item;
        }
      }

      return lista[lista.length - 1];
    }

    function carregarDadosFicticios() {
      if (
        banco.clientes.length ||
        banco.produtos.length ||
        banco.vendas.length
      ) {
        const continuar = confirm(
          "Já existem dados cadastrados. Deseja adicionar dados fictícios mesmo assim?"
        );

        if (!continuar) return;
      }

      const agora = new Date();
      const dois = numero => String(numero).padStart(2, "0");

      const fornecedoresFicticios = [
        "Moto Parts Brasil",
        "Speed Peças Ltda",
        "Nordeste Motopeças"
      ].map(nome => ({
        id: id("fornecedor"),
        nome,
        telefone: "88999990000",
        documento: "00.000.000/0001-00",
        observacoes: "Cadastro fictício",
        criadoEm: agora.toISOString()
      }));

      banco.fornecedores.push(...fornecedoresFicticios);

      const catalogo = [
        ["Pastilha de freio dianteira", "Freio", 38.90, 30],
        ["Kit relação completo", "Transmissão", 189.90, 24],
        ["Vela de ignição", "Motor", 19.90, 21],
        ["Filtro de óleo", "Motor", 24.50, 18],
        ["Pneu traseiro 90/90-18", "Pneus", 219.00, 12],
        ["Amortecedor traseiro", "Suspensão", 245.00, 8],
        ["Cabo de embreagem", "Controles", 27.50, 6],
        ["Retrovisor par", "Acessórios", 59.90, 5],
        ["Bateria 5Ah", "Elétrica", 169.90, 3],
        ["Lâmpada de farol", "Elétrica", 14.90, 2],
        ["Corrente de comando", "Motor", 89.90, 1],
        ["Disco de freio", "Freio", 129.90, 0.5]
      ];

      const produtosFicticios = catalogo.map(
        ([nome, categoria, preco, peso], indice) => ({
          id: id("produto"),
          codigoInterno: gerarCodigoProduto(),
          nome,
          categoria,
          preco,
          fornecedorId:
            fornecedoresFicticios[indice % fornecedoresFicticios.length].id,
          peso,
          criadoEm: agora.toISOString()
        })
      );

      banco.produtos.push(
        ...produtosFicticios.map(produto => {
          const copia = { ...produto };
          delete copia.peso;
          return copia;
        })
      );

      const clientesBase = [
        ["Oficina do Zé", 30],
        ["Moto Center Silva", 25],
        ["Auto Moto Cariri", 18],
        ["Mecânica Rápida", 12],
        ["Box Moto Peças", 8],
        ["Garagem do Beto", 6],
        ["Moto Service Norte", 5],
        ["Oficina Dois Irmãos", 4],
        ["Moto Fácil", 3],
        ["Renato Mototáxi", 2],
        ["Cleiton Entregas", 1.5],
        ["Lucas Motoboy", 1]
      ];

      const clientesFicticios = clientesBase.map(
        ([nome, peso], indice) => {
          const aniversario = indice === 0
            ? `${1985}-${dois(agora.getMonth() + 1)}-${dois(agora.getDate())}`
            : `1990-${dois((indice % 12) + 1)}-${dois((indice % 27) + 1)}`;

          const cliente = {
            id: id("cliente"),
            nome,
            telefone: "88999991111",
            aniversario,
            empresa: "Juazeiro do Norte",
            observacoes: "Cadastro fictício",
            criadoEm: agora.toISOString(),
            timeline: [{
              id: id("timeline"),
              data: agora.toISOString(),
              tipo: "Cliente cadastrado",
              descricao: "Cadastro fictício realizado."
            }]
          };

          banco.clientes.push(cliente);

          return {
            cliente,
            peso
          };
        }
      );

      const vendedores = ["Carlos", "Ana", "Roberto"];
      const canais = ["Presencial", "WhatsApp", "Telefone"];

      for (let contador = 0; contador < 100; contador++) {
        const clienteEscolhido = escolherPonderado(
          clientesFicticios.map(item => ({
            ...item.cliente,
            peso: item.peso
          }))
        );

        const cliente = obterCliente(clienteEscolhido.id);

        const dataVenda = new Date(agora);
        dataVenda.setDate(
          dataVenda.getDate() - Math.floor(Math.random() * 180)
        );

        const itens = [];
        const quantidadeItens = 1 + Math.floor(Math.random() * 3);

        for (let indice = 0; indice < quantidadeItens; indice++) {
          const produtoEscolhido = escolherPonderado(produtosFicticios);

          if (
            itens.some(item =>
              item.produtoId === produtoEscolhido.id
            )
          ) {
            continue;
          }

          const garantiaAtiva = Math.random() < 0.08;

          itens.push({
            id: id("item"),
            produtoId: produtoEscolhido.id,
            quantidade: 1 + Math.floor(Math.random() * 7),
            garantiaAtiva,
            garantiaAtivadaEm: garantiaAtiva
              ? dataVenda.toISOString()
              : null
          });
        }

        const vendedor =
          vendedores[Math.floor(Math.random() * vendedores.length)];

        const canal =
          canais[Math.floor(Math.random() * canais.length)];

        const venda = {
          id: id("venda"),
          clienteId: cliente.id,
          vendedor,
          canal,
          observacao: "Venda fictícia",
          data: `${dataVenda.getFullYear()}-${dois(dataVenda.getMonth() + 1)}-${dois(dataVenda.getDate())}`,
          criadoEm: dataVenda.toISOString(),
          itens
        };

        banco.vendas.push(venda);

        adicionarTimeline(
          cliente.id,
          "Venda lançada",
          `Venda fictícia lançada pelo vendedor ${vendedor}.`,
          { vendaId: venda.id }
        );

        itens.forEach(item => {
          if (!item.garantiaAtiva) return;

          const produto = obterProduto(item.produtoId);

          adicionarTimeline(
            cliente.id,
            "Garantia ativada",
            `Garantia ativada para ${produto?.nome || "produto"}.`,
            {
              vendaId: venda.id,
              produtoId: produto?.id
            }
          );
        });
      }

      banco.vendas.sort((a, b) =>
        b.data.localeCompare(a.data)
      );

      salvar();
      renderizarTudo();

      mostrarAviso(
        "Dados fictícios carregados com sucesso. Acesse o Dashboard e abra o perfil de qualquer cliente."
      );
    }

    document.querySelectorAll(".menu-btn").forEach(botao => {
      botao.addEventListener("click", () => {
        document.querySelectorAll(".menu-btn").forEach(item =>
          item.classList.remove("active")
        );

        document.querySelectorAll(".view").forEach(view =>
          view.classList.remove("active")
        );

        botao.classList.add("active");

        const viewId = botao.dataset.view;
        document.getElementById(viewId).classList.add("active");

        const titulos = {
          dashboard: "Dashboard",
          clientes: "Clientes",
          produtos: "Produtos",
          fornecedores: "Fornecedores",
          financeiro: "Financeiro"
        };

        document.getElementById("page-title").textContent =
          titulos[viewId];
      });
    });

    document
      .getElementById("client-search")
      .addEventListener("input", renderizarClientes);

    document
      .getElementById("client-form")
      .addEventListener("submit", event => {
        event.preventDefault();

        const cliente = {
          id: id("cliente"),
          nome: document.getElementById("client-name").value.trim(),
          telefone: document.getElementById("client-phone").value.trim(),
          aniversario: document.getElementById("client-birthday").value,
          empresa: document.getElementById("client-company").value.trim(),
          observacoes: document.getElementById("client-notes").value.trim(),
          criadoEm: new Date().toISOString(),
          timeline: [{
            id: id("timeline"),
            data: new Date().toISOString(),
            tipo: "Cliente cadastrado",
            descricao: "Cadastro inicial realizado."
          }]
        };

        banco.clientes.push(cliente);

        salvar();
        event.target.reset();
        renderizarTudo();

        mostrarAviso(
          "Cliente cadastrado. Agora clique em 'Abrir perfil e vender' para lançar os produtos vendidos."
        );
      });

    document
      .getElementById("supplier-form")
      .addEventListener("submit", event => {
        event.preventDefault();

        banco.fornecedores.push({
          id: id("fornecedor"),
          nome: document.getElementById("supplier-name").value.trim(),
          telefone: document.getElementById("supplier-phone").value.trim(),
          documento: document.getElementById("supplier-document").value.trim(),
          observacoes: document.getElementById("supplier-notes").value.trim(),
          criadoEm: new Date().toISOString()
        });

        salvar();
        event.target.reset();
        renderizarTudo();

        mostrarAviso("Fornecedor cadastrado com sucesso.");
      });

    document
      .getElementById("product-form")
      .addEventListener("submit", event => {
        event.preventDefault();

        const nome = document.getElementById("product-name").value.trim();
        const fornecedorId =
          document.getElementById("product-supplier").value;
        const categoria =
          document.getElementById("product-category").value.trim();
        const preco =
          Number(document.getElementById("product-price").value);

        if (!nome || !preco) {
          mostrarAviso("Informe o nome e o preço do produto.");
          return;
        }

        const produto = {
          id: id("produto"),
          codigoInterno: gerarCodigoProduto(),
          nome,
          fornecedorId,
          categoria,
          preco,
          criadoEm: new Date().toISOString()
        };

        banco.produtos.push(produto);

        salvar();
        event.target.reset();
        renderizarTudo();

        mostrarAviso(
          `Produto cadastrado com o código ${produto.codigoInterno}.`
        );
      });

    document
      .getElementById("finance-form")
      .addEventListener("submit", event => {
        event.preventDefault();

        banco.financeiro.push({
          id: id("financeiro"),
          tipo: document.getElementById("finance-type").value,
          descricao:
            document.getElementById("finance-description").value.trim(),
          valor: Number(
            document.getElementById("finance-value").value
          ),
          vencimento:
            document.getElementById("finance-due-date").value,
          status: document.getElementById("finance-status").value,
          criadoEm: new Date().toISOString()
        });

        salvar();
        event.target.reset();
        renderizarTudo();

        mostrarAviso("Lançamento financeiro salvo.");
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
