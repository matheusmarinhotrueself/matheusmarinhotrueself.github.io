<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Conceitos Financeiros Essenciais</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .banner {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
        }

        .header {
            text-align: center;
            margin-bottom: 40px;
        }

        .header h1 {
            color: #2c3e50;
            font-size: 2.5rem;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .header p {
            color: #7f8c8d;
            font-size: 1.2rem;
        }

        .concepts-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }

        .concept-card {
            background: #fff;
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border-left: 5px solid;
        }

        .concept-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.15);
        }

        .inflacao {
            border-left-color: #e74c3c;
        }

        .renda-fixa {
            border-left-color: #27ae60;
        }

        .selic {
            border-left-color: #3498db;
        }

        .ipca {
            border-left-color: #9b59b6;
        }

        .imposto {
            border-left-color: #f39c12;
        }

        .card-icon {
            font-size: 3rem;
            margin-bottom: 15px;
            text-align: center;
        }

        .inflacao .card-icon { color: #e74c3c; }
        .renda-fixa .card-icon { color: #27ae60; }
        .selic .card-icon { color: #3498db; }
        .imposto .card-icon { color: #f39c12; }

        .card-title {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 15px;
            color: #2c3e50;
        }

        .card-description {
            color: #5a6c7d;
            line-height: 1.6;
            margin-bottom: 20px;
        }

        .card-examples {
            background: #f8f9fa;
            border-radius: 10px;
            padding: 15px;
            margin-top: 15px;
        }

        .card-examples h4 {
            color: #2c3e50;
            font-size: 0.9rem;
            margin-bottom: 10px;
            text-transform: uppercase;
            font-weight: 600;
        }

        .examples-list {
            list-style: none;
            padding: 0;
        }

        .examples-list li {
            color: #5a6c7d;
            margin-bottom: 5px;
            padding-left: 20px;
            position: relative;
        }

        .examples-list li::before {
            content: "•";
            position: absolute;
            left: 0;
            color: #3498db;
            font-weight: bold;
        }

        .highlight-box {
            background: linear-gradient(135deg, #74b9ff, #0984e3);
            color: white;
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            margin-top: 30px;
        }

        .highlight-box h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }

        .highlight-box p {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        @media (max-width: 768px) {
            .banner {
                padding: 20px;
            }
            
            .header h1 {
                font-size: 2rem;
            }
            
            .concepts-grid {
                grid-template-columns: 1fr;
                gap: 20px;
            }
        }

        .percentage {
            font-size: 1.2rem;
            font-weight: bold;
            color: #e74c3c;
        }

        .rate {
            font-size: 1.2rem;
            font-weight: bold;
            color: #3498db;
        }

        .tax-rate {
            font-size: 1.2rem;
            font-weight: bold;
            color: #f39c12;
        }
    </style>
</head>
<body>
    <div class="banner">
        <div class="header">
            <h1>💰 Conceitos Financeiros Essenciais</h1>
            <p>Entenda de forma simples os pilares do mercado financeiro brasileiro</p>
        </div>

        <div class="concepts-grid">
            <div class="concept-card inflacao">
                <div class="card-icon">📈</div>
                <h3 class="card-title">Inflação</h3>
                <p class="card-description">
                    É o aumento generalizado dos preços na economia. Quando há inflação, seu dinheiro perde poder de compra ao longo do tempo.
                </p>
                <div class="card-examples">
                    <h4>Na prática:</h4>
                    <ul class="examples-list">
                        <li>Um produto que custava R$ 100 pode custar R$ <span class="percentage">105</span> no ano seguinte</li>
                        <li>Meta atual no Brasil: <span class="percentage">3% ao ano</span></li>
                        <li>Medida pelo IPCA (Índice de Preços)</li>
                    </ul>
                </div>
            </div>

            <div class="concept-card renda-fixa">
                <div class="card-icon">🏦</div>
                <h3 class="card-title">Renda Fixa</h3>
                <p class="card-description">
                    Investimentos onde você empresta dinheiro e recebe de volta com juros. É mais seguro que ações, mas com menor potencial de ganho.
                </p>
                <div class="card-examples">
                    <h4>Principais tipos:</h4>
                    <ul class="examples-list">
                        <li><strong>CDB:</strong> Empréstimo para bancos</li>
                        <li><strong>LCI:</strong> Financia setor imobiliário</li>
                        <li><strong>LCA:</strong> Financia agronegócio</li>
                        <li>LCI e LCA são <strong>isentas de IR</strong></li>
                    </ul>
                </div>
            </div>

            <div class="concept-card selic">
                <div class="card-icon">🎯</div>
                <h3 class="card-title">Taxa Selic</h3>
                <p class="card-description">
                    É a taxa básica de juros da economia brasileira, definida pelo Banco Central. Influencia todas as outras taxas do mercado.
                </p>
                <div class="card-examples">
                    <h4>Como funciona:</h4>
                    <ul class="examples-list">
                        <li>Taxa atual: cerca de <span class="rate">10,5% ao ano</span></li>
                        <li>Selic alta = renda fixa mais atrativa</li>
                        <li>Selic baixa = incentivo ao consumo</li>
                        <li>Definida a cada 45 dias pelo Copom</li>
                    </ul>
                </div>
            </div>

            <div class="concept-card imposto">
                <div class="card-icon">📋</div>
                <h3 class="card-title">Imposto de Renda</h3>
                <p class="card-description">
                    Taxa cobrada sobre os ganhos dos investimentos. Varia conforme o tipo de investimento e tempo de aplicação.
                </p>
                <div class="card-examples">
                    <h4>Tabela regressiva (CDB, LC):</h4>
                    <ul class="examples-list">
                        <li>Até 180 dias: <span class="tax-rate">22,5%</span></li>
                        <li>181 a 360 dias: <span class="tax-rate">20%</span></li>
                        <li>361 a 720 dias: <span class="tax-rate">17,5%</span></li>
                        <li>Acima de 720 dias: <span class="tax-rate">15%</span></li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="highlight-box">
            <h3>💡 Dica Importante</h3>
            <p>
                Para vencer a inflação, seus investimentos devem render mais que ela. 
                Por isso é importante diversificar e escolher produtos que ofereçam rentabilidade real positiva!
            </p>
        </div>
    </div>
</body>
</html>
