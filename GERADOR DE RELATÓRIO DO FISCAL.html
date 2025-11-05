<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
    <title>Gerador de relatório do fiscal - 9° BPM / BPTRAN</title>
    <style>
        /* Paleta: Azul Escuro (#0d47a1), Azul Sóbrio (#1a3a5e), Cinza Claro (#f0f2f5), Branco (#ffffff) */
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; 
            margin: 0;
            padding: 0;
            background-color: #f0f2f5; 
            display: flex;
            justify-content: center; 
            align-items: flex-start;
            min-height: 10vh; 
            box-sizing: border-box; 
            padding: 10px 0; 
            color: #000; /* Cor de texto padrão para o modo claro */
        }

        /* ------------------------------------------- */
        /* ESTILOS DO MODO ESCURO */
        /* ------------------------------------------- */
        
        .dark-mode {
            background-color: #121212; /* Fundo escuro principal */
            color: #e0e0e0; /* Cor de texto principal para o modo escuro */
        }
        
        .dark-mode .container {
            background: #1e1e1e; /* Fundo do container escuro */
            box-shadow: 0 6px 15px rgba(255, 255, 255, 0.08); 
            border-top-color: #4a90e2; /* Borda superior em destaque */
        }

        .dark-mode .header-title h1 {
            color: #4a90e2; /* Título principal em azul claro */
        }
        
        .dark-mode .header-title {
            border-bottom: 2px solid #333; 
        }

        .dark-mode label {
            color: #bbbbbb; /* Labels em cinza mais claro */
        }

        .dark-mode input[type="text"],
        .dark-mode input[type="time"],
        .dark-mode textarea,
        .dark-mode select {
            background-color: #2c2c2c;
            color: #e0e0e0;
            border: 1px solid #444;
        }

        .dark-mode input:focus, 
        .dark-mode select:focus, 
        .dark-mode textarea:focus {
            border-color: #4a90e2; 
            box-shadow: 0 0 0 1px #4a90e2;
        }

        .dark-mode .dynamic-input-container {
            border: 1px solid #333;
            background-color: #252525;
        }
        
        .dark-mode #reportOutput {
            border: 1px solid #444;
            background-color: #2c2c2c; 
            color: #4a90e2; /* Cor destacada para o relatório */
        }

        .dark-mode h2 {
            color: #bbbbbb;
            border-bottom: 1px dashed #555;
        }

        .dark-mode #toastMessage {
            background-color: #555;
            color: #f0f0f0;
        }
        
        /* Ajuste do botão Adicionar/Remover no modo escuro */
        .dark-mode .add-btn {
            background-color: #4a90e2; 
        }
        .dark-mode .add-btn:hover {
            background-color: #6aabf7;
        }
        /* Fim dos estilos do modo escuro */
        
        /* ------------------------------------------- */
        /* ESTILOS PADRÃO (CLARO) */
        /* ------------------------------------------- */
        
        @media (max-height: 900px) {
            body {
                align-items: center; 
            }
        }

        .container {
            width: 95%; 
            max-width: 650px; 
            background: #ffffff;
            padding: 30px 25px; 
            border-radius: 4px; 
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1); 
            box-sizing: border-box;
            border-top: 5px solid #0d47a1; 
            position: relative; /* Para posicionar o botão de tema */
        }

        /* Removendo a sombra em mobile para um look mais nativo */
        @media (max-width: 600px) {
            .container {
                padding: 20px 15px;
                border-radius: 0;
                box-shadow: none;
                border-top: none;
            }
        }
        
        /* ESTILOS DO CABEÇALHO */
        .header-title {
            text-align: center;
            padding-bottom: 15px;
            margin-bottom: 25px;
            border-bottom: 2px solid #ddd; 
        }
        .header-title h1 {
            color: #1a3a5e; 
            margin: 0; 
            font-size: clamp(20px, 5vw, 30px); 
            font-weight: 600; 
        }
        
        /* Botão de tema (NOVO) */
        #themeToggle {
            position: absolute;
            top: 15px;
            right: 15px;
            background: none;
            border: none;
            cursor: pointer;
            font-size: 20px;
            color: #1a3a5e; /* Cor do ícone no modo claro */
            padding: 5px;
            transition: color 0.3s;
        }

        .dark-mode #themeToggle {
            color: #e0e0e0; /* Cor do ícone no modo escuro */
        }
        
        /* Estilos dos campos */
        .field-group {
            margin-bottom: 20px; 
        }
        label {
            display: block;
            margin-bottom: 6px;
            font-weight: 700; 
            color: #333333; 
            font-size: 0.9em;
            text-transform: uppercase; 
        }
        .required-asterisk {
            color: #d9534f;
            margin-left: 3px;
        }

        input[type="text"],
        input[type="time"],
        textarea,
        select {
            width: 100%;
            padding: 12px; 
            border: 1px solid #c4c4c4;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 16px;
            transition: border-color 0.3s;
        }

        textarea {
            resize: vertical;
            min-height: 80px;
        }

        input:focus, select:focus, textarea:focus {
            border-color: #0d47a1; 
            box-shadow: 0 0 0 1px #0d47a1;
            outline: none;
        }
        
        /* Estilos para campos dinâmicos */
        .dynamic-input-container {
            border: 1px solid #e0e0e0;
            padding: 15px;
            border-radius: 4px;
            margin-top: 10px;
            background-color: #f9f9f9;
        }
        .dynamic-input-row {
            display: flex;
            align-items: center;
            margin-bottom: 10px;
            gap: 8px; 
        }
        .dynamic-input-row input {
            flex-grow: 1;
            margin-right: 0; 
        }

        /* Botões de campo dinâmico */
        .add-btn, .remove-btn {
            padding: 10px;
            font-size: 14px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.2s, transform 0.1s;
        }
        .add-btn {
            background-color: #1a3a5e; 
            color: white;
            margin-top: 10px;
            width: 100%;
        }
        .add-btn:hover {
            background-color: #0d47a1;
            transform: translateY(-1px);
        }
        .remove-btn {
            background-color: #d9534f; 
            color: white;
        }
        .dynamic-input-row .remove-btn {
             width: 80px; 
        }
        .remove-btn:hover {
            background-color: #c9302c;
        }
        
        /* Estilos dos botões de ação final */
        .button-group {
            text-align: center;
            margin-top: 30px;
            display: flex;
            flex-direction: column; 
            gap: 15px; 
        }
        .button-group button {
            width: 100%; 
            margin: 0;
            padding: 14px; 
            font-weight: 600;
        }
        @media (min-width: 450px) {
            .button-group {
                flex-direction: row;
                flex-wrap: wrap;
                justify-content: space-between; 
            }
            .button-group button {
                flex-grow: 1;
                max-width: 32%; 
            }
            .button-group.full-width button {
                max-width: 48%; 
                margin-bottom: 10px; 
            }
        }
        @media (min-width: 650px) {
             .button-group.full-width button {
                max-width: 24%; 
                margin-bottom: 0; 
            }
        }
        
        /* Cores dos botões */
        #generateBtn {
            background-color: #28a745; 
            color: white;
        }
        #generateBtn:hover {
            background-color: #218838;
        }
        #generateBtnNoHeader { 
            background-color: #0d47a1; 
            color: white;
        }
        #generateBtnNoHeader:hover {
            background-color: #1a3a5e; 
        }
        #copyBtn {
            background-color: #007bff; 
            color: white;
            display: none; 
        }
        #copyBtn:hover {
            background-color: #0056b3;
        }
        #clearBtn {
            background-color: #6c757d; 
            color: white;
        }
        #clearBtn:hover {
            background-color: #5a6268;
        }
        
        /* Estilos para o Output do Relatório */
        #reportOutput {
            margin-top: 25px;
            border: 1px solid #ddd;
            padding: 15px;
            white-space: pre-wrap;
            background-color: #eef1f4; 
            border-radius: 4px;
            min-height: 100px;
            font-size: 14px;
            color: #333;
            line-height: 1.5;
            font-family: monospace, sans-serif; 
        }
        h2 {
            color: #1a3a5e;
            font-size: 1.2em;
            border-bottom: 1px dashed #ccc;
            padding-bottom: 5px;
        }

        /* TOAST MESSAGE */
        #toastMessage {
            visibility: hidden;
            min-width: 250px;
            background-color: #333;
            color: #fff;
            text-align: center;
            border-radius: 4px;
            padding: 12px 20px;
            position: fixed;
            z-index: 1000;
            left: 50%;
            bottom: 30px;
            transform: translateX(-50%);
            font-size: 15px;
            opacity: 0;
            transition: opacity 0.5s, visibility 0.5s;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        #toastMessage.show {
            visibility: visible;
            opacity: 1;
        }
    </style>
</head>
<body>

    <div class="container">
        
        <button id="themeToggle" aria-label="Alternar Tema">☀️</button> <div class="header-title">
            <h1>GERADOR DE RELATÓRIO DO FISCAL</h1>
            <span style="color: #6c757d; font-size: 0.9em;">9° BPM / BPTRAN</span>
        </div>

        <form id="reportForm">
            <div class="field-group">
                <label for="data">Data (DD/MM/AA) <span class="required-asterisk">*</span>:</label>
                <input type="text" id="data" value="" inputmode="numeric">
            </div>

            <div class="field-group">
                <label for="turno">Turno <span class="required-asterisk">*</span>:</label>
                <select id="turno">
                    <option value="1° TURNO">1° TURNO</option>
                    <option value="2° TURNO">2° TURNO</option>
                </select>
            </div>

            <div class="field-group">
                <label for="bst">NÚMERO DO BST <span class="required-asterisk">*</span>:</label>
                <input type="text" id="bst" value="" inputmode="numeric">
            </div>

            <div class="field-group">
                <label for="ppe">NÚMERO DO PPE <span class="required-asterisk">*</span>:</label>
                <input type="text" id="ppe" value="">
            </div>

            <div class="field-group">
                <label for="chegadaEquipe">HORÁRIO DE CHEGADA DA EQUIPE <span class="required-asterisk">*</span>:</label>
                <input type="time" id="chegadaEquipe" value="">
            </div>

            <div class="field-group">
                <label for="acionamentoPericia">HORÁRIO DE ACIONAMENTO DA PERÍCIA <span class="required-asterisk">*</span>:</label>
                <input type="time" id="acionamentoPericia" value="">
            </div>

            <div class="field-group">
                <label for="chegadaPericia">HORÁRIO DE CHEGADA DA PERÍCIA <span class="required-asterisk">*</span>:</label>
                <input type="time" id="chegadaPericia" value="">
            </div>

            <div class="field-group">
                <label for="nomePerito">NOME DO PERITO <span class="required-asterisk">*</span>:</label>
                <input type="text" id="nomePerito" value="">
            </div>

            <div class="field-group">
                <label for="terminoOcorrencia">HORÁRIO DO TÉRMINO DA OCORRÊNCIA <span class="required-asterisk">*</span>:</label>
                <input type="time" id="terminoOcorrencia" value="">
            </div>

            <div class="field-group">
                <label>AUTO DE INFRAÇÃO (Opcional):</label>
                <div id="autosInfracaoContainer" class="dynamic-input-container">
                    <div class="dynamic-input-row">
                        <input type="text" class="auto-infracao-input" value="">
                        <button type="button" class="remove-btn" onclick="removeField(this)">Remover</button>
                    </div>
                </div>
                <button type="button" class="add-btn" onclick="addField('autosInfracaoContainer', 'auto-infracao-input', '', '')">Adicionar Auto Extra</button>
            </div>
            
            <div class="field-group">
                <label>TERMO DE CONSTATAÇÃO (Opcional):</label>
                <div id="termoConstatacaoContainer" class="dynamic-input-container">
                    <div class="dynamic-input-row">
                        <input type="text" class="termo-input" value="" inputmode="numeric">
                        <button type="button" class="remove-btn" onclick="removeField(this)">Remover</button>
                    </div>
                </div>
                <button type="button" class="add-btn" onclick="addField('termoConstatacaoContainer', 'termo-input', '', 'numeric')">Adicionar Termo Extra</button>
            </div>

            <div class="field-group">
                <label>TESTE DO ETILÔMETRO (Opcional):</label>
                <div id="testeEtilometroContainer" class="dynamic-input-container">
                    <div class="dynamic-input-row">
                        <input type="text" class="etilometro-input" value="" inputmode="numeric">
                        <button type="button" class="remove-btn" onclick="removeField(this)">Remover</button>
                    </div>
                </div>
                <button type="button" class="add-btn" onclick="addField('testeEtilometroContainer', 'etilometro-input', '', 'numeric')">Adicionar Teste Extra</button>
            </div>
            
            <div class="field-group">
                <label for="outrasInformacoes">OUTRAS INFORMAÇÕES (Opcional):</label>
                <textarea id="outrasInformacoes"></textarea>
            </div>
            
        </form>

        <div class="button-group full-width">
            <button id="generateBtn">Gerar Relatório Padrão</button>
            <button id="generateBtnNoHeader">Gerar Relatório (Sem Cabeçalho)</button>
            <button id="copyBtn">Copiar Relatório</button>
            <button id="clearBtn">Limpar Campos</button>
        </div>

        <h2>RELATÓRIO GERADO</h2>
        <pre id="reportOutput"></pre>
    </div>
    
    <div id="toastMessage"></div>

    
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            setTodayDate();
            // Lógica do tema escuro: Carrega a preferência salva. Inicia em tema claro se não houver preferência.
            loadThemePreference(); 
            
            document.getElementById('generateBtn').addEventListener('click', () => generateReport(true)); 
            document.getElementById('generateBtnNoHeader').addEventListener('click', () => generateReport(false)); 
            document.getElementById('copyBtn').addEventListener('click', copyReport);
            document.getElementById('clearBtn').addEventListener('click', clearFields);
            document.getElementById('themeToggle').addEventListener('click', toggleTheme);
        });

        // -------------------------------------------
        // FUNÇÕES DO TEMA ESCURO (Mantidas para iniciar em tema claro)
        // -------------------------------------------
        
        /**
         * Alterna entre o modo claro e escuro.
         */
        function toggleTheme() {
            const body = document.body;
            const isDarkMode = body.classList.toggle('dark-mode');
            const themeToggle = document.getElementById('themeToggle');
            
            // Atualiza o ícone e a preferência
            themeToggle.textContent = isDarkMode ? '🌙' : '☀️';
            localStorage.setItem('theme', isDarkMode ? 'dark' : 'light');
            
            showToast(isDarkMode ? 'Tema Escuro Ativado.' : 'Tema Claro Ativado.');
        }

        /**
         * Carrega a preferência de tema do localStorage. Inicia no tema claro por padrão.
         */
        function loadThemePreference() {
            const savedTheme = localStorage.getItem('theme');
            const themeToggle = document.getElementById('themeToggle');
            
            let isDarkMode = false;

            // Só ativa o modo escuro se a preferência 'dark' estiver salva
            if (savedTheme === 'dark') {
                isDarkMode = true; 
            }
            // Se não houver preferência salva, isDarkMode permanece false (tema claro)

            if (isDarkMode) {
                document.body.classList.add('dark-mode');
                themeToggle.textContent = '🌙';
            } else {
                // Assegura que o tema claro seja o padrão inicial
                document.body.classList.remove('dark-mode');
                themeToggle.textContent = '☀️';
            }
        }
        
        // -------------------------------------------
        // FUNÇÕES EXISTENTES
        // -------------------------------------------
        
        /**
         * Exibe uma mensagem Toast (flutuante) no rodapé da tela.
         */
        function showToast(message) {
            const toast = document.getElementById("toastMessage");
            toast.textContent = message;
            toast.classList.add("show");
            
            // Esconde o toast após 3 segundos
            setTimeout(function(){ 
                toast.classList.remove("show"); 
            }, 3000);
        }

        /**
         * Preenche o campo de data com a data atual (DD/MM/AA).
         */
        function setTodayDate() {
            const today = new Date();
            const dd = String(today.getDate()).padStart(2, '0');
            const mm = String(today.getMonth() + 1).padStart(2, '0'); 
            const yy = String(today.getFullYear()).slice(-2); 
            document.getElementById('data').value = `${dd}/${mm}/${yy}`;
        }
        
        /**
         * Adiciona uma nova linha de input dinâmico (com placeholder vazio).
         */
        function addField(containerId, inputClass, placeholderText, inputMode = '') {
            const container = document.getElementById(containerId);
            const newRow = document.createElement('div');
            newRow.className = 'dynamic-input-row';
            const newInput = document.createElement('input');
            newInput.type = 'text';
            newInput.className = inputClass;
            newInput.inputMode = inputMode; 
            newInput.placeholder = ''; // Placeholder removido
            const removeButton = document.createElement('button');
            removeButton.type = 'button';
            removeButton.className = 'remove-btn';
            removeButton.textContent = 'Remover';
            removeButton.onclick = function() { removeField(this); };
            newRow.appendChild(newInput);
            newRow.appendChild(removeButton);
            container.appendChild(newRow);
            showToast('Campo extra adicionado.');
        }

        /**
         * Remove uma linha de input dinâmico ou limpa o valor se for o único campo.
         */
        function removeField(button) {
            const rowToRemove = button.parentNode;
            const container = rowToRemove.parentNode;
            if (container.querySelectorAll('.dynamic-input-row').length > 1) {
                rowToRemove.remove();
                showToast('Campo removido.');
            } else {
                rowToRemove.querySelector('input').value = '';
                showToast('Campo limpo.');
            }
        }
        
        /**
         * Coleta os valores dos campos dinâmicos e formata a saída.
         */
        function collectDynamicFields(className) {
            const inputs = document.querySelectorAll(`.${className}`);
            const values = [];
            inputs.forEach(input => {
                const value = input.value.trim();
                if (value) {
                    values.push(value);
                }
            });
            
            const hasValues = values.length > 0;
            let reportValue = '';

            if (hasValues) {
                if (values.length === 1) {
                    reportValue = values[0];
                } else {
                    reportValue = '\n' + values.map(item => `- ${item}`).join('\n');
                }
            }
            
            return {
                hasValues: hasValues,
                value: reportValue
            };
        }
        
        /**
         * Gera o relatório, incluindo condicionalmente os cabeçalhos.
         * @param {boolean} includeHeader - Se deve incluir "RELATÓRIO DO FISCAL", Data e Turno.
         */
        function generateReport(includeHeader) {
            // Coleta de dados dos campos principais
            const data = document.getElementById('data').value.trim();
            const turno = document.getElementById('turno').value.trim();
            const bst = document.getElementById('bst').value.trim();
            const ppe = document.getElementById('ppe').value.trim();
            const chegadaEquipe = document.getElementById('chegadaEquipe').value.trim();
            const acionamentoPericia = document.getElementById('acionamentoPericia').value.trim();
            const chegadaPericia = document.getElementById('chegadaPericia').value.trim();
            const nomePerito = document.getElementById('nomePerito').value.trim();
            const terminoOcorrencia = document.getElementById('terminoOcorrencia').value.trim();
            const outrasInformacoes = document.getElementById('outrasInformacoes').value.trim();
            
            // VERIFICAÇÃO DE CAMPOS OBRIGATÓRIOS
            if (!data || !turno || !bst || !ppe || !chegadaEquipe || !acionamentoPericia || !chegadaPericia || !nomePerito || !terminoOcorrencia) {
                showToast('Atenção: Preencha todos os campos obrigatórios (*).');
                document.getElementById('reportOutput').textContent = 'FALHA NA GERAÇÃO: Preencha todos os campos obrigatórios marcados com (*).';
                document.getElementById('copyBtn').style.display = 'none';
                return;
            }

            // Coleta de dados dos campos dinâmicos
            const autosInfracao = collectDynamicFields('auto-infracao-input');
            const termoConstatacao = collectDynamicFields('termo-input');
            const testeEtilometro = collectDynamicFields('etilometro-input');
            

            // Montagem da parte principal do relatório
            let reportText = ``;
            
            if (includeHeader) {
                reportText += `RELATÓRIO DO FISCAL
DIA ${data} - ${turno}\n`;
            } else {
                 reportText += `\n`; // Adiciona uma quebra de linha para começar no BST
            }

            reportText += `
NÚMERO DO BST: ${bst}
NÚMERO DO PPE: ${ppe}
HORÁRIO DE CHEGADA DA EQUIPE: ${chegadaEquipe}
HORÁRIO DE ACIONAMENTO DA PERÍCIA: ${acionamentoPericia}
HORÁRIO DE CHEGADA DA PERÍCIA: ${chegadaPericia}
NOME DO PERITO: ${nomePerito}
HORÁRIO DO TÉRMINO DA OCORRÊNCIA: ${terminoOcorrencia}`;

            // INCLUSÃO CONDICIONAL: Autos de Infração (Texto de label removido, mas a chave é mantida)
            if (autosInfracao.hasValues) {
                reportText += `\n\nAUTO DE INFRAÇÃO: ${autosInfracao.value}`;
            }

            // INCLUSÃO CONDICIONAL: Termo de Constatação (Texto de label removido, mas a chave é mantida)
            if (termoConstatacao.hasValues) {
                reportText += `\n\nTERMO DE CONSTATAÇÃO: ${termoConstatacao.value}`;
            }

            // INCLUSÃO CONDICIONAL: Teste Etilômetro (Texto de label removido, mas a chave é mantida)
            if (testeEtilometro.hasValues) {
                reportText += `\n\nTESTE DO ETILÔMETRO: ${testeEtilometro.value}`;
            }
            
            // INCLUSÃO CONDICIONAL: Outras Informações
            if (outrasInformacoes) {
                reportText += `\n\nOUTRAS INFORMAÇÕES:\n${outrasInformacoes}`;
            }
            
            // Finaliza o relatório com uma quebra de linha extra para formatação
            reportText += `\n`;


            document.getElementById('reportOutput').textContent = reportText.trim(); // Remove espaços em branco no início e fim
            document.getElementById('copyBtn').style.display = 'inline-block';
            showToast('Relatório gerado com sucesso!');
        }

        /**
         * Copia o relatório gerado para a área de transferência.
         */
        function copyReport() {
            const reportText = document.getElementById('reportOutput').textContent;
            
            // Impede a cópia se o relatório não foi gerado ou está com erro
            if (reportText.includes('FALHA NA GERAÇÃO') || reportText.trim() === '') { 
                showToast('Gere um relatório válido primeiro.');
                return;
            }

            navigator.clipboard.writeText(reportText)
                .then(() => {
                    showToast('Relatório copiado para a área de transferência.');
                })
                .catch(err => {
                    // Fallback para ambientes onde o navigator.clipboard falha
                    const textarea = document.createElement('textarea');
                    textarea.value = reportText;
                    document.body.appendChild(textarea);
                    textarea.select();
                    document.execCommand('copy');
                    document.body.removeChild(textarea);
                    showToast('Copiado! Método fallback utilizado.');
                });
        }

        /**
         * Limpa todos os campos do formulário e redefine os campos dinâmicos.
         */
        function clearFields() {
            // 1. Usa o método reset() para limpar inputs padrão e selects
            document.getElementById('reportForm').reset();

            // 2. Limpa o output do relatório
            document.getElementById('reportOutput').textContent = ''; 
            document.getElementById('copyBtn').style.display = 'none';

            // 3. Lida com os campos dinâmicos (remover linhas adicionais e limpar o campo restante)
            const containers = ['autosInfracaoContainer', 'termoConstatacaoContainer', 'testeEtilometroContainer'];
            containers.forEach(containerId => {
                const container = document.getElementById(containerId);
                const rows = container.querySelectorAll('.dynamic-input-row');
                
                // Limpa o primeiro input
                if (rows.length > 0) {
                    rows[0].querySelector('input').value = '';
                }

                // Remove as linhas extras
                for (let i = rows.length - 1; i > 0; i--) {
                    rows[i].remove();
                }
            });
            
            // 4. Preenche a data novamente
            setTodayDate();

            showToast('Todos os campos foram limpos.');
        }
    </script>
    </body>
</html>
