<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora Clínica | Dr. Jerônimo Sampaio</title>
    <style>
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background-color: #f0f2f5; display: flex; justify-content: center; align-items: center; min-height: 100vh; margin: 0; }
        .container { background: white; padding: 2rem; border-radius: 12px; box-shadow: 0 8px 24px rgba(0,0,0,0.1); width: 100%; max-width: 480px; }
        h2 { color: #10b981; text-align: center; margin-bottom: 1.5rem; display: flex; align-items: center; justify-content: center; gap: 10px; }
        label { display: block; margin: 15px 0 5px; font-weight: 600; color: #374151; }
        input, select { width: 100%; padding: 12px; border: 1px solid #d1d5db; border-radius: 8px; box-sizing: border-box; font-size: 1rem; transition: border-color 0.3s; }
        input:focus, select:focus { border-color: #10b981; outline: none; }
        
        .checkbox-group { display: flex; gap: 15px; flex-wrap: wrap; margin-top: 10px; }
        .checkbox-item { display: flex; align-items: center; font-weight: normal; cursor: pointer; }
        .checkbox-item input { width: auto; margin-right: 8px; }

        button { width: 100%; padding: 15px; background-color: #10b981; color: white; border: none; border-radius: 8px; font-size: 1.1rem; font-weight: bold; cursor: pointer; margin-top: 25px; transition: background-color 0.3s; }
        button:hover { background-color: #059669; }

        #resultado { display: none; margin-top: 25px; animation: fadeIn 0.5s; }
        .card { padding: 15px; border-radius: 8px; margin-bottom: 10px; }
        .card-gotejamento { background-color: #ecfdf5; border-left: 5px solid #10b981; color: #064e3b; }
        .card-sugestao { background-color: #eff6ff; border-left: 5px solid #3b82f6; color: #1e40af; }
        .card-alerta { background-color: #fef2f2; border-left: 5px solid #ef4444; color: #991b1b; }
        
        @keyframes fadeIn { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }
    </style>
</head>
<body>

<div class="container">
    <h2>💉 SoroCalc <small style="font-size: 0.6em; color: #6b7280;">v1.0</small></h2>
    
    <label>Peso do Paciente (kg):</label>
    <input type="number" id="peso" placeholder="Ex: 70.5" step="0.1">

    <label>Objetivo do Tratamento:</label>
    <select id="objetivo">
        <option value="energia">⚡ Energia / Fadiga (Mitocondrial)</option>
        <option value="imunidade">🛡️ Imunidade</option>
        <option value="pos_bariatrica">🍽️ Pós-Bariátrica</option>
        <option value="ressaca">🥴 Hidratação / Detox</option>
        <option value="dor">💊 Dor Crônica (Protocolo GGOH)</option>
    </select>

    <label>Volume da Bolsa (ml):</label>
    <select id="volume">
        <option value="100">100 ml (Rápido)</option>
        <option value="250">250 ml (Padrão)</option>
        <option value="500">500 ml (Hidratação)</option>
        <option value="1000">1000 ml (Hospitalar)</option>
    </select>

    <label>Tempo de Infusão (minutos):</label>
    <input type="number" id="tempo" value="60">

    <label>Comorbidades (Segurança):</label>
    <div class="checkbox-group">
        <label class="checkbox-item"><input type="checkbox" id="hipertensao"> Hipertensão</label>
        <label class="checkbox-item"><input type="checkbox" id="diabetes"> Diabetes</label>
        <label class="checkbox-item"><input type="checkbox" id="renal"> Insuf. Renal</label>
    </div>

    <button onclick="calcularSoro()">CALCULAR PROTOCOLO</button>

    <div id="resultado"></div>
</div>

<script>
    function calcularSoro() {
        // Coletar Inputs
        const peso = parseFloat(document.getElementById('peso').value);
        const volume = parseInt(document.getElementById('volume').value);
        const tempo = parseInt(document.getElementById('tempo').value);
        const objetivo = document.getElementById('objetivo').value;
        const isHipertenso = document.getElementById('hipertensao').checked;
        const isRenal = document.getElementById('renal').checked;

        // Validação básica
        if (!peso || !tempo) {
            alert("Por favor, preencha o peso e o tempo.");
            return;
        }

        // 1. Cálculo Matemático (Macrogotas)
        const gotejamento = (volume * 20) / tempo;

        // 2. Lógica Farmacêutica (Protocolos)
        let sugestao = "";
        switch (objetivo) {
            case 'energia': sugestao = "Sugestão: Protocolo Mitocondrial (PQQ + Coenzima Q10 + L-Carnitina)."; break;
            case 'imunidade': sugestao = "Sugestão: Protocolo Shield (Vit C Alta Dose + Zinco + Lisina)."; break;
            case 'pos_bariatrica': sugestao = "Sugestão: Reposição de Ferro + Complexo B + Citrato de Magnésio."; break;
            case 'ressaca': sugestao = "Sugestão: Soro Glicofisiológico + Ondansetrona + Magnésio."; break;
            case 'dor': sugestao = "Sugestão: Geranilgeraniol (IM preferencial) + B12 + Magnésio Dimalato."; break;
        }

        // 3. Sistema de Alerta de Segurança
        let alertas = [];
        if (isHipertenso && volume > 250) {
            alertas.push("⚠️ ALERTA HIPERTENSÃO: Volume > 250ml. Risco de pico hipertensivo. Monitore a PA.");
        }
        if (isRenal) {
            alertas.push("🚨 ALERTA RENAL: Ajuste obrigatório pela Taxa de Filtração Glomerular (TFG). Cuidado com Potássio.");
        }
        if (gotejamento > 80 && volume > 100) {
            alertas.push("ℹ️ Velocidade alta: Observe sinais de flebite ou desconforto.");
        }

        // 4. Renderizar Resultado
        const divResultado = document.getElementById('resultado');
        let html = `
            <div class="card card-gotejamento">
                <h3>💧 ${gotejamento.toFixed(0)} gotas/minuto</h3>
                <small>Volume total: ${volume}ml em ${tempo} min</small>
            </div>
            <div class="card card-sugestao">
                <strong>👨‍⚕️ Dr. Jerônimo recomenda:</strong><br>${sugestao}
            </div>
        `;

        alertas.forEach(msg => {
            html += `<div class="card card-alerta">${msg}</div>`;
        });

        divResultado.innerHTML = html;
        divResultado.style.display = 'block';
    }
</script>

</body>
</html>
