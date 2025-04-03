<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Cadastro de Fornecedores e Produtos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
        }
        button {
            background-color: #0079BF;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin-right: 10px;
        }
        button[type="reset"] {
            background-color: #CF513D;
        }
        .categoria-select {
            margin-bottom: 20px;
        }
    </style>
</head>
<body>
    <form id="cadastroForm">
        <h2>Cadastro de Fornecedor</h2>
        
        <div class="form-group">
            <label for="categoria">Categoria do Fornecedor:</label>
            <select id="categoria" name="categoria" required>
                <option value="">Selecione uma categoria</option>
                <option value="pet">Produtos PET</option>
                <option value="eletricos">Materiais Elétricos</option>
                <option value="veiculos">Acessórios de Veículos</option>
                <option value="cameras">Câmeras e Controles</option>
                <option value="livros">Livros</option>
            </select>
        </div>

        <div class="form-group">
            <label for="fornecedorNome">Nome do Fornecedor:</label>
            <input type="text" id="fornecedorNome" name="fornecedorNome" required>
        </div>

        <div class="form-group">
            <label for="fornecedorCNPJ">CNPJ:</label>
            <input type="text" id="fornecedorCNPJ" name="fornecedorCNPJ" pattern="\d{2}\.\d{3}\.\d{3}/\d{4}-\d{2}" placeholder="00.000.000/0000-00" required>
        </div>

        <div class="form-group">
            <label for="fornecedorEndereco">Endereço Completo:</label>
            <textarea id="fornecedorEndereco" name="fornecedorEndereco" rows="3" required></textarea>
        </div>

        <div class="form-group">
            <label for="fornecedorContato">Nome do Contato:</label>
            <input type="text" id="fornecedorContato" name="fornecedorContato" required>
        </div>

        <div class="form-group">
            <label for="fornecedorTelefone">Telefone:</label>
            <input type="tel" id="fornecedorTelefone" name="fornecedorTelefone" pattern="\(\d{2}\)\s\d{4,5}-\
