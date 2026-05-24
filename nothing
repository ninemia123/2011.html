<!DOCTYPE html>
<html lang="el">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
    <title>ΦΡΟΥΡΑ ΕΙΔΙΚΟ · 2026</title>
    <style>
        :root {
            --primary: #1b4d2b;
            --primary-light: #2e6b3e;
            --secondary: #5a7c5a;
            --bg: #f4f7f2;
            --card: #ffffff;
            --text: #1e2a1e;
            --shadow: 0 4px 12px rgba(0,20,0,0.08);
            --border-soft: #dde8dd;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
        }

        body {
            background-color: var(--bg);
            color: var(--text);
            padding: 0.75rem;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }

        .container {
            max-width: 600px;
            margin: 0 auto;
            width: 100%;
            overflow-x: hidden;
        }

        h2 {
            font-size: 1.6rem;
            color: var(--primary);
            margin: 0.25rem 0 1rem 0;
            border-bottom: 3px solid var(--primary);
            padding-bottom: 0.4rem;
            letter-spacing: -0.01em;
        }

        h3 {
            font-size: 1.3rem;
            color: var(--primary);
            margin: 1.2rem 0 0.8rem 0;
        }

        h4 {
            font-size: 1.1rem;
            color: var(--primary-light);
            margin: 0.8rem 0 0.3rem 0;
        }

        .tabs-container {
            display: flex;
            gap: 0.4rem;
            margin-bottom: 1.2rem;
            position: sticky;
            top: 0;
            z-index: 5;
            background: var(--bg);
            padding: 0.5rem 0 0.2rem 0;
        }

        .tab-button {
            flex: 1;
            padding: 0.9rem 0.2rem;
            font-size: 1rem;
            font-weight: 600;
            border: none;
            border-radius: 40px;
            background-color: #dde8dd;
            color: #1e3a2a;
            cursor: pointer;
            transition: all 0.2s;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
            letter-spacing: 0.3px;
            touch-action: manipulation;
        }

        .tab-button.active {
            background: var(--primary);
            color: white;
            box-shadow: 0 4px 8px rgba(27,77,43,0.3);
        }

        .tab-content {
            display: none;
            background: var(--card);
            border-radius: 28px 20px 20px 20px;
            padding: 1.3rem 1rem;
            box-shadow: var(--shadow);
            margin-bottom: 1.2rem;
        }

        .tab-content.active {
            display: block;
        }

        .form-group {
            margin-bottom: 1.2rem;
        }

        .deduction-selector {
            display: flex;
            align-items: center;
            gap: 1rem;
            background: #e1d7f0;
            padding: 0.8rem 1rem;
            border-radius: 40px;
            margin-bottom: 0.8rem;
        }
        
        .deduction-selector label {
            margin-bottom: 0;
            flex: 1;
            color: #4a2e7a;
            font-weight: 600;
        }
        
        .deduction-selector select {
            width: auto;
            flex: 0.5;
            background: white;
            border: 1px solid #8f79b0;
        }

        label {
            display: block;
            font-weight: 600;
            font-size: 0.95rem;
            color: var(--primary);
            margin-bottom: 0.3rem;
            padding-left: 0.2rem;
        }

        input, select {
            width: 100%;
            padding: 0.9rem 1rem;
            border: 1.5px solid var(--border-soft);
            border-radius: 24px;
            font-size: 1rem;
            background: white;
            transition: 0.15s;
            -webkit-appearance: none;
            appearance: none;
        }

        input:focus, select:focus {
            border-color: var(--primary);
            outline: none;
            box-shadow: 0 0 0 3px rgba(27,77,43,0.2);
        }

        input[readonly] {
            background-color: #ecf3ec;
            font-weight: 600;
            color: #0f3a1a;
        }

        .section-title {
            color: var(--primary);
            border-bottom: 2px solid var(--primary);
            padding-bottom: 0.5rem;
            margin: 1.5rem 0 1rem 0;
            font-size: 1.25rem;
        }

        .main-grid {
            display: flex;
            flex-direction: column;
            gap: 1.2rem;
        }

        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 0.8rem;
        }

        .grid-3 {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 0.8rem;
        }

        .result-card {
            background: var(--card);
            padding: 1.2rem 1rem;
            border-radius: 28px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border-soft);
            width: 100%;
            overflow: hidden;
        }

        .results-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 0.7rem;
            margin: 0.8rem 0;
        }

        .result-item {
            background: #eef4ea;
            border-radius: 20px;
            padding: 0.7rem 0.3rem;
            text-align: center;
            box-shadow: inset 0 1px 4px rgba(0,0,0,0.02);
        }

        .result-item label {
            font-size: 0.75rem;
            margin-bottom: 0.2rem;
            color: #2b4b2b;
        }

        .result-item .value {
            font-size: 1.2rem;
            font-weight: 700;
            color: var(--primary);
            line-height: 1.3;
            word-break: break-word;
        }

        .value.tax { color: #b13e3e; }
        .value.net { color: #113e5e; }

        .table-container {
            overflow-x: auto;
            border-radius: 20px;
            background: white;
            margin: 0.8rem 0;
            -webkit-overflow-scrolling: touch;
            max-width: 100%;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            font-size: 0.85rem;
        }

        th {
            background: var(--primary);
            color: white;
            padding: 0.6rem 0.2rem;
            font-weight: 600;
            font-size: 0.8rem;
            white-space: nowrap;
        }

        td {
            padding: 0.5rem 0.2rem;
            border: 1px solid #cbdccb;
            text-align: center;
        }

        .badge {
            background: #f2c94c;
            color: #1e3a2a;
            padding: 0.2rem 0.6rem;
            border-radius: 40px;
            font-size: 0.7rem;
            font-weight: 700;
            display: inline-block;
            margin-left: 0.3rem;
            white-space: nowrap;
        }

        .info-box {
            background: #e2efe2;
            border-left: 5px solid var(--primary);
            padding: 1rem;
            border-radius: 20px;
            margin: 1rem 0;
            font-size: 0.95rem;
        }

        .coeff-row {
            display: flex;
            flex-wrap: wrap;
            gap: 0.7rem;
            background: #edf3ed;
            padding: 1rem 0.8rem;
            border-radius: 30px;
            margin: 1rem 0;
            align-items: center;
        }

        .coeff-box {
            flex: 1 1 100px;
            min-width: 80px;
        }

        .coeff-box label {
            font-size: 0.75rem;
            margin-bottom: 0.1rem;
        }

        .coeff-input {
            background: white;
            font-weight: 700;
            text-align: center;
            padding: 0.6rem 0.2rem;
        }

        .night-penhmero-wrapper {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        @media (min-width: 420px) {
            .night-penhmero-wrapper {
                display: grid;
                grid-template-columns: 1fr 1fr;
                gap: 1rem;
            }
        }

        .night-box, .penhmero-box {
            background: #f0f7ee;
            border-radius: 24px;
            padding: 1rem;
        }

        .night-box input, .penhmero-box input {
            background: white;
        }

        .extra-total {
            background: #fff1cf;
            border-radius: 40px;
            padding: 1rem 1.2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-weight: 700;
            flex-wrap: wrap;
            margin-top: 1rem;
        }

        .informational-table td {
            font-weight: 500;
        }

        ul, ol {
            padding-left: 1.4rem;
            margin-bottom: 1rem;
        }

        li {
            margin-bottom: 0.3rem;
        }

        .instructions-content {
            font-size: 1rem;
            line-height: 1.6;
        }

        .note, .warning {
            border-radius: 24px;
        }

        button, select, input {
            touch-action: manipulation;
        }

        footer {
            text-align: center;
            font-size: 0.8rem;
            color: #5f735f;
            margin: 1.5rem 0 0.2rem;
        }

        .compact-table table {
            font-size: 0.75rem;
        }
        .compact-table td, .compact-table th {
            padding: 0.4rem 0.1rem;
            white-space: normal;
        }

        .pre-1993-toggle {
            background: #e6e0c1;
            border-radius: 40px;
            padding: 1rem;
            margin-bottom: 1rem;
            border: 2px solid #c9b561;
        }
        
        .extra-deductions-container {
            background: #e1d7f0;
            border-radius: 40px;
            padding: 1rem;
            margin-bottom: 1rem;
            border: 2px solid #8f79b0;
        }
        
        .extra-deduction-item {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 0.8rem;
        }
        
        .extra-deduction-item label {
            margin-bottom: 0;
            flex: 1;
            color: #4a2e7a;
            font-size: 1rem;
        }
        
        .extra-deduction-item select {
            width: auto;
            flex: 0.4;
            background: white;
            border: 1px solid #8f79b0;
        }
        
        .extra-deduction-item:last-child {
            margin-bottom: 0;
        }
        
        .border-top-dashed {
            border-top: 2px dashed #c9b561;
            margin-top: 1rem;
            padding-top: 1rem;
        }

        /* Μικρή προσαρμογή για τα αποτελέσματα νυχτών/πενθήμερων */
        .night-detail, .penhmero-detail {
            font-size: 0.85rem;
            color: #2b4b2b;
            background: #dde8dd;
            border-radius: 30px;
            padding: 0.6rem;
            margin-top: 0.5rem;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="container">
    <h2>📱 ΦΡΟΥΡΑ ΕΙΔΙΚΟ ΥΠΟΛΟΓΙΣΜΟΣ</h2>

    <div class="tabs-container">
        <button class="tab-button active" onclick="openTab('calculator')" id="tabCalculator">🧮 Υπολογιστής</button>
        <button class="tab-button" onclick="openTab('instructions')" id="tabInstructions">📖 Οδηγίες</button>
    </div>

    <div id="calculator" class="tab-content active">

        <!-- ΠΡΟ 1993 ΕΠΙΛΟΓΗ -->
        <div class="pre-1993-toggle">
            <div style="display: flex; align-items: center; gap: 1rem;">
                <label style="margin-bottom: 0; font-size: 1.1rem; color: #5a4700;">📜 Προ 1993</label>
                <select id="pre1993Select" style="width: auto; flex: 1; background: #faf5e4;">
                    <option value="no">Όχι</option>
                    <option value="yes">Ναι</option>
                </select>
            </div>
        </div>
        
        <!-- ΝΕΕΣ ΕΠΙΛΟΓΕΣ ΚΡΑΤΗΣΕΩΝ (στυλ Προ 1993) -->
        <div class="extra-deductions-container">
            <h4 style="margin-top: 0; margin-bottom: 1rem; color: #4a2e7a;">➕ Επιπλέον Κρατήσεις</h4>
            
            <div class="extra-deduction-item">
                <label for="tameioAllilov">Ταμείο Αλληλοβοήθειας (5,83€)</label>
                <select id="tameioAllilov">
                    <option value="no">Όχι</option>
                    <option value="yes">Ναι</option>
                </select>
            </div>
            
            <div class="extra-deduction-item">
                <label for="kladYgeias">Κλάδος Υγείας (1,5%)</label>
                <select id="kladYgeias">
                    <option value="no">Όχι</option>
                    <option value="yes">Ναι</option>
                </select>
            </div>
            
            <div style="font-size: 0.9rem; color: #4a2e7a; margin-top: 0.8rem; font-style: italic;">
                * Ισχύουν για όλους (προ και μετά 1993)
            </div>
        </div>

        <div class="result-card" style="padding-bottom: 0.8rem;">
            <h3 class="section-title" style="margin-top: 0;">📋 Βασικοί μισθοί (Κατ. Γ)</h3>
            <div class="table-container">
                <table>
                    <thead><tr><th>Κλιμ.</th><th>Έτη</th><th>Μισθός (€)</th></tr></thead>
                    <tbody id="salaryScaleTable"></tbody>
                </table>
            </div>

            <div class="coeff-row">
                <div class="coeff-box" style="flex: 2 1 180px;">
                    <label for="scaleSelect">📌 Επιλογή κλιμακίου</label>
                    <select id="scaleSelect"></select>
                </div>
                <div class="coeff-box"><label>ΦΡ</label><input type="text" id="coefFR" value="1,03" class="coeff-input" readonly></div>
                <div class="coeff-box"><label>ΥΠΡΧ</label><input type="text" id="coefYPRX" value="1,04" class="coeff-input" readonly></div>
                <div class="coeff-box"><label>ΑΡΧΦ</label><input type="text" id="coefARXF" value="1,07" class="coeff-input" readonly></div>
                <div class="coeff-box" style="flex:1.8">
                    <label for="coefSelect">Συντελεστής</label>
                    <select id="coefSelect">
                        <option value="1.00">-- Κανένας --</option>
                        <option value="1.03">ΦΡ (1,03)</option>
                        <option value="1.04">ΥΠΡΧ (1,04)</option>
                        <option value="1.07">ΑΡΧΦ (1,07)</option>
                    </select>
                </div>
            </div>
        </div>

        <div class="grid-2" style="gap: 1rem;">
            <div class="result-card">
                <h4>💰 Επιδόματα</h4>
                <div class="form-group"><label>Επικίνδυνο (€)</label><input type="number" id="dangerousBonus" value="150" step="0.01"></div>
                <div class="form-group"><label>Ιδ. Καθηκόντων (€)</label><input type="number" id="idsynBonus" value="100" step="0.01"></div>
                <div class="form-group"><label>Επίδομα τέκνων (€)</label><input type="number" id="childrenBonus" value="70" step="0.01"></div>
                <!-- ΝΕΟ ΠΕΔΙΟ: Επίδομα Παραμεθορίου -->
                <div class="form-group border-top-dashed">
                    <label>🏔️ Επίδομα Παραμεθορίου (€)</label>
                    <input type="number" id="borderBonus" value="0" step="0.01">
                </div>
            </div>
            <div class="result-card">
                <h4>⚙️ Παράμετροι</h4>
                <div class="form-group"><label>👶 Αριθμός τέκνων</label>
                    <select id="numChildrenSelect">
                        <option value="0">0</option><option value="1" selected>1</option><option value="2">2</option>
                        <option value="3">3</option><option value="4">4</option><option value="5">5+</option>
                    </select>
                </div>
                <div class="form-group"><label>📅 Ηλικία</label>
                    <select id="ageGroup">
                        <option value="over30">Άνω 30</option><option value="under30">25-30</option><option value="under25">Έως 25</option>
                    </select>
                </div>
                <div class="form-group"><label>💳 ΠΟΥΦ (€) <span class="badge">αφαίρεση</span></label>
                    <input type="number" id="input-pouf" value="4" step="0.01">
                </div>
            </div>
        </div>

        <div class="form-group" style="margin-top:0.5rem">
            <label>Βασικός μισθός αποδοχών (με συντελεστή)</label>
            <input type="number" id="basicSalary" step="0.01" readonly>
        </div>

        <div class="result-card">
            <h3 class="section-title">📈 Αποτελέσματα</h3>
            <div class="results-grid">
                <div class="result-item"><label>Μην. Μεικτά</label><div class="value" id="display-monthly-gross">0 €</div></div>
                <div class="result-item"><label>Κρατήσεις</label><div class="value" id="display-monthly-deductions">0 €</div></div>
                <div class="result-item"><label>Προ φόρου</label><div class="value" id="display-pre-tax">0 €</div></div>
                <div class="result-item"><label>Ετήσιο φορολ.</label><div class="value" id="display-annual-taxable">0 €</div></div>
                <div class="result-item"><label>Φόρος 2026</label><div class="value tax" id="display-tax">0 €</div></div>
                <div class="result-item"><label>Καθαρό μήνα</label><div class="value net" id="display-monthly-net">0 €</div></div>
                <div class="result-item"><label>15νθήμερο</label><div class="value" id="display-fortnight">0 €</div></div>
                <div class="result-item"><label>Ετήσιο καθαρό</label><div class="value" id="display-annual-net">0 €</div></div>
            </div>
        </div>

        <div class="result-card">
            <h3 class="section-title" style="margin-top:0;">🌙 Νυχτερινά / Πενθήμερα</h3>
            <div class="night-penhmero-wrapper">
                <!-- Τροποποιημένο τμήμα για Νυχτερινά: ο χρήστης βάζει αριθμό νυχτών -->
                <div class="night-box">
                    <label>Νυχτερινά (αριθμός νυχτών)</label>
                    <input type="number" id="nightCount" value="1" min="0" step="1">
                    <input type="hidden" id="nightValue" value="3.3" step="0.01"> <!-- κρυφή τιμή ωρομισθίου -->
                    <div style="background:#e2f0e2; border-radius:40px; padding:0.6rem; margin-top:0.7rem; text-align:center; font-weight:bold;" id="nightHoursDisplay">8 ώρες</div>
                    <div style="background:#e2f0e2; border-radius:40px; padding:0.6rem; margin-top:0.2rem; text-align:center; font-weight:bold;" id="nightGrossTotal">26,40 €</div>
                    <!-- Λεπτομέρειες κρατήσεων για νυχτερινά -->
                    <div class="night-detail" id="nightDetails">
                        Μεικτό: 26,40 €<br>
                        Εισφ Αλλ 2%: 0,53 €<br>
                        ΜΤΠΥ 2%: 0,53 €<br>
                        Υπόλοιπο: 25,34 €<br>
                        Φόρος 20%: 5,07 €<br>
                        <strong>Καθαρό: 20,27 €</strong>
                    </div>
                </div>
                <!-- Τροποποιημένο τμήμα για Πενθήμερα -->
                <div class="penhmero-box">
                    <label>Πενθήμερα (αριθμός)</label>
                    <input type="number" id="penhmeroCount" value="1" min="0" step="1">
                    <label style="margin-top:0.5rem;">Τιμή μονάδας (€)</label>
                    <input type="number" id="penhmeroValue" value="46" step="0.01">
                    <div style="background:#e2f0e2; border-radius:40px; padding:0.6rem; margin-top:0.7rem; text-align:center; font-weight:bold;" id="penhmeroGrossTotal">46,00 €</div>
                    <!-- Λεπτομέρειες κρατήσεων για πενθήμερα -->
                    <div class="penhmero-detail" id="penhmeroDetails">
                        Μεικτό: 46,00 €<br>
                        Εισφ Αλλ 2%: 0,92 €<br>
                        Υπόλοιπο: 45,08 €<br>
                        Φόρος 20%: 9,02 €<br>
                        <strong>Καθαρό: 36,06 €</strong>
                    </div>
                </div>
            </div>
            <div class="extra-total">
                <span>Σύνολο extras (καθαρά)</span>
                <span style="font-size:1.5rem; color:var(--primary);" id="nightPenhmeroTotal">56,33 €</span>
            </div>
        </div>

        <div class="result-card">
            <h4>🔍 Αναλυτικές κρατήσεις</h4>
            <div class="table-container">
                <table id="detailed-table">
                    <thead><tr><th>Περιγραφή</th><th>Ποσό (€)</th></tr></thead>
                    <tbody id="detailed-table-body"></tbody>
                </table>
            </div>
        </div>

        <div class="grid-2">
            <div class="result-card informational-table compact-table">
                <h4>👶 Επίδομα τέκνων</h4>
                <table>
                    <thead><tr><th>Τέκνα</th><th>Ποσό</th></tr></thead>
                    <tbody><tr><td>1</td><td>70 €</td></tr><tr><td>2</td><td>120 €</td></tr><tr><td>3</td><td>170 €</td></tr><tr><td>4</td><td>220 €</td></tr><tr><td>5</td><td>290 €</td></tr></tbody>
                </table>
            </div>
            <div class="result-card informational-table compact-table">
                <h4>🛡️ Σωμάτων Ασφ.</h4>
                <table>
                    <thead><tr><th>Κατηγορία</th><th>Ποσό</th></tr></thead>
                    <tbody><tr><td>ΕΠΙΚ/ΙΔ.ΣΥΝΘ</td><td>155 €</td></tr><tr><td>ΕΓΓΑΜΟΣ</td><td>225 €</td></tr><tr><td>ΜΕ ΤΕΚΝΑ</td><td>285 €</td></tr></tbody>
                </table>
            </div>
        </div>

        <div class="result-card">
            <h4>📋 Φορολογική κλίμακα 2026 (άνω 30)</h4>
            <div class="table-container">
                <table>
                    <thead><tr><th>Εισόδημα</th><th>0τ</th><th>1τ</th><th>2τ</th><th>3τ</th><th>4+τ</th></tr></thead>
                    <tbody>
                        <tr><td>0-10.000</td><td>9%</td><td>9%</td><td>9%</td><td>9%</td><td>0%</td></tr>
                        <tr><td>10-20.000</td><td>20%</td><td>18%</td><td>16%</td><td>9%</td><td>0%</td></tr>
                        <tr><td>20-30.000</td><td>26%</td><td>24%</td><td>22%</td><td>20%</td><td>18%</td></tr>
                        <tr><td>30-40.000</td><td>34%</td><td>34%</td><td>34%</td><td>34%</td><td>34%</td></tr>
                        <tr><td>40-60.000</td><td>39%</td><td>39%</td><td>39%</td><td>39%</td><td>39%</td></tr>
                        <tr><td>60.001+</td><td>44%</td><td>44%</td><td>44%</td><td>44%</td><td>44%</td></tr>
                    </tbody>
                </table>
            </div>
            <div style="margin-top:0.8rem;" class="info-box">
                <strong>Έκπτωση φόρου:</strong> 0τ:777, 1τ:900, 2τ:1120, 3τ:1340, 4τ:1580, 5τ:1780 +220/παιδί<br>Μείωση 20€/1000€ >12.000€
            </div>
        </div>
    </div>

    <div id="instructions" class="tab-content">
        <div class="result-card instructions-content">
            <h3>📖 Οδηγίες χρήσης</h3>
            <h4>🔹 Βήμα 1</h4>
            <p>Επιλέξτε κλιμάκιο από τον πίνακα. Ο βασικός μισθός ενημερώνεται αυτόματα. Μπορείτε να εφαρμόσετε συντελεστή βαθμού (ΦΡ, ΥΠΡΧ, ΑΡΧΦ).</p>
            <h4>🔹 Βήμα 2</h4>
            <p>Συμπληρώστε τα συνήθη επιδόματα (επικίνδυνο, ιδ. συνθηκών, τέκνων). Τα ποσά είναι ενδεικτικά – μπορείτε να τα τροποποιήσετε.</p>
            <h4>🔹 Βήμα 3 - Νέο</h4>
            <p><strong>Επίδομα Παραμεθορίου:</strong> Προστέθηκε νέο πεδίο με αρχική τιμή 0€. Λειτουργεί ακριβώς όπως τα άλλα επιδόματα και υπόκειται στις ίδιες κρατήσεις (κανονικές ή Προ 1993).</p>
            <h4>🔹 Βήμα 4</h4>
            <p>Ορίστε αριθμό τέκνων (για φόρο), ηλικιακή ομάδα και ΠΟΥΦ. Ο υπολογισμός γίνεται ζωντανά.</p>
            <h4>🔹 Προ 1993</h4>
            <p>Η επιλογή "Προ 1993" εφαρμόζει μειωμένες κρατήσεις στα επιδόματα (συμπεριλαμβανομένου και του νέου Παραμεθορίου): μόνο Υγειονομική (2,05%), Ανεργία (2%) και ΜΤΠΥ (1%). Ο βασικός μισθός κρατάει τις κανονικές κρατήσεις.</p>
            <h4>🔹 Νέες επιλογές κρατήσεων</h4>
            <p><strong>Ταμείο Αλληλοβοήθειας:</strong> σταθερή κράτηση 5,83€ από τα μηνιαία μεικτά.<br>
            <strong>Κλάδος Υγείας 1,5%:</strong> επιπλέον ποσοστιαία κράτηση στο σύνολο των μεικτών.</p>
            <h4>🔹 Νυχτερινά / Πενθήμερα</h4>
            <p><strong>Νυχτερινά:</strong> Ο χρήστης εισάγει αριθμό νυχτών (π.χ. 2). Αυτό πολλαπλασιάζεται με 8 ώρες και στη συνέχεια με 3,3€/ώρα. Από το μεικτό ποσό αφαιρείται 2% Εισφορά Αλληλεγγύης και 2% ΜΤΠΥ, και από το υπόλοιπο υπολογίζεται φόρος 20% για να προκύψει το καθαρό.<br>
            <strong>Πενθήμερα:</strong> Από το μεικτό ποσό (π.χ. 46€) αφαιρείται 2% Εισφορά Αλληλεγγύης και από το υπόλοιπο υπολογίζεται φόρος 20% για το καθαρό.</p>
            <div class="note">
                <strong>⚠️ Δοκιμαστική έκδοση</strong> — Ειναι καθαρα δοκιμαστικο προκειμενου οταν εχουμε πραγματικη εικονα να στηθει το κανονικο.ΔΕΝ ΕΧΕΙ ΣΥΜΠΕΡΙΛΗΦΘΕΙ ΟΙ ΝΕΟΔΙΟΡΙΣΤΟΙ.Οι σειρες ισως να εχουν διαφορετικη αντιμετωπιση πχ η πρωτη σειρα και οι πρωην δηματικοι δεν θα μπορεσουν να ενταχθουν σε αλλα ταμεια σωματων ασφαλειας , οι σειρες Β,Γ,νεοι θα πρεπει να γινει μελετη σε περιπτωση που τεθει θεμα. Τα σωματα ασφαλεις εχουν συνδεση επιδοματων με οικογενειακη κατασταση , εχει συμπεριεληφθει πινακας αναλογος μπορει καποιος να πειραματιστει και με αυτο τον ενδεχομενο.Για αυτο τον λογο τα πλαισια στα επιδοματα ειναι ελυεθερα. ΔΕΝ ΕΙΝΑΙ 100% ΕΤΟΙΜΟ Ειναι μια βαση για μελλοντικη εργασια.πενθημερα νυχτερινα προ κρατησεων κ φορου δοκιμαστικη εκδοση.
            </div>
            <p style="border-top:1px dashed #a0b9a0; padding-top:0.8rem;">Τελευταία ενημέρωση: Φεβρ. 2026</p>
        </div>
    </div>
    <footer>Φρουρά Ειδικό · έκδοση για κινητά</footer>
</div>

<script>
    function openTab(tabName) {
        document.querySelectorAll('.tab-content').forEach(c => c.classList.remove('active'));
        document.querySelectorAll('.tab-button').forEach(b => b.classList.remove('active'));
        document.getElementById(tabName).classList.add('active');
        document.getElementById('tab' + (tabName === 'calculator' ? 'Calculator' : 'Instructions')).classList.add('active');
    }

    const salaryScale = [
        { scale: 1,  years: "0-1",   amount: 998  },
        { scale: 2,  years: "1-3",   amount: 1058 },
        { scale: 3,  years: "3-5",   amount: 1118 },
        { scale: 4,  years: "5-7",   amount: 1178 },
        { scale: 5,  years: "7-9",   amount: 1238 },
        { scale: 6,  years: "9-11",  amount: 1298 },
        { scale: 7,  years: "11-13", amount: 1358 },
        { scale: 8,  years: "13-15", amount: 1418 },
        { scale: 9,  years: "15-17", amount: 1478 },
        { scale: 10, years: "17-19", amount: 1538 },
        { scale: 11, years: "19-21", amount: 1598 },
        { scale: 12, years: "21-23", amount: 1658 },
        { scale: 13, years: "23-25", amount: 1718 },
        { scale: 14, years: "25-27", amount: 1778 },
        { scale: 15, years: "27-29", amount: 1838 },
        { scale: 16, years: "29-31", amount: 1898 },
        { scale: 17, years: "31-33", amount: 1958 },
        { scale: 18, years: "33-35", amount: 2018 },
        { scale: 19, years: "35-37", amount: 2078 },
        { scale: 20, years: "37-39", amount: 2138 },
        { scale: 21, years: "39-40", amount: 2198 }
    ];

    function populateTables() {
        const tbody = document.getElementById('salaryScaleTable');
        tbody.innerHTML = salaryScale.map(item => `<tr><td>${item.scale}</td><td>${item.years}</td><td>${item.amount.toFixed(2)} €</td></tr>`).join('');
        const select = document.getElementById('scaleSelect');
        select.innerHTML = '<option value="">-- Επιλογή --</option>' + salaryScale.map(item => `<option value="${item.amount}">Κλ.${item.scale} (${item.years}) ${item.amount} €</option>`).join('');
    }

    function calculateTax2026(annual, children, age) {
        if (age === 'under25') { if (annual <= 20000) return 0; let rem = annual - 20000, tax = 0; [10000,10000,20000,Infinity].forEach((lim, i) => { let bracket = Math.min(rem, lim); tax += bracket * (i === 0 ? 0.26 : i === 1 ? 0.34 : i === 2 ? 0.39 : 0.44); rem -= bracket; }); return tax; }
        if (age === 'under30') { let t = 0, r = annual; let steps = [10000,10000,10000,10000,20000]; let rates = [0.09,0.09,0.26,0.34,0.39,0.44]; for (let i=0; i<steps.length && r>0; i++) { let b = Math.min(r, steps[i]); t += b * rates[i]; r -= b; } if (r>0) t += r * 0.44; return t; }
        let tax = 0, rem = annual; const rates = (c) => { if (c >= 4) return [0,0,18,34,39,44]; return [[9,20,26,34,39,44],[9,18,24,34,39,44],[9,16,22,34,39,44],[9,9,20,34,39,44]][c] || [9,20,26,34,39,44]; };
        let r = rates(children); let br = [10000,10000,10000,10000,20000]; for (let i=0; i<br.length && rem>0; i++) { let b = Math.min(rem, br[i]); tax += b * r[i]/100; rem -= b; } if (rem>0) tax += rem * r[5]/100; return tax;
    }

    function taxCredit(annual, children, age) {
        if (age === 'under25') return 0;
        let base = [777,900,1120,1340,1580,1780]; let idx = Math.min(children,5); let credit = base[idx] + (children>5 ? (children-5)*220 : 0);
        if (annual <= 12000) return credit;
        let red = Math.floor((annual - 12000) / 1000) * 20;
        return Math.max(0, credit - red);
    }

    function formatMoney(v) { return v.toFixed(2).replace('.',',') + ' €'; }

    // Συνάρτηση υπολογισμού νυχτερινών και πενθήμερων με κρατήσεις & φόρο
    function calculateExtras() {
        // Νυχτερινά: αριθμός νυχτών -> ώρες = νύχτες * 8, μεικτό = ώρες * 3,3
        const nightCount = parseFloat(document.getElementById('nightCount')?.value) || 0;
        const nightHourly = 3.3; // σταθερό ωρομίσθιο
        const nightHours = nightCount * 8;
        const nightGross = nightHours * nightHourly;
        
        // Κρατήσεις νυχτερινών: 2% Εισφ Αλλ, 2% ΜΤΠΥ, μετά φόρος 20% στο υπόλοιπο
        const eisforiaAllNight = nightGross * 0.02;
        const mtpyNight = nightGross * 0.02;
        const afterDeductionsNight = nightGross - eisforiaAllNight - mtpyNight;
        const taxNight = afterDeductionsNight * 0.20;
        const nightNet = afterDeductionsNight - taxNight;

        // Πενθήμερα: μεικτό = αριθμός * τιμή μονάδας
        const penhmeroCount = parseFloat(document.getElementById('penhmeroCount')?.value) || 0;
        const penhmeroValue = parseFloat(document.getElementById('penhmeroValue')?.value) || 0;
        const penhmeroGross = penhmeroCount * penhmeroValue;
        
        // Κρατήσεις πενθημέρων: 2% Εισφ Αλλ, μετά φόρος 20% στο υπόλοιπο
        const eisforiaAllPenh = penhmeroGross * 0.02;
        const afterDeductionsPenh = penhmeroGross - eisforiaAllPenh;
        const taxPenh = afterDeductionsPenh * 0.20;
        const penhmeroNet = afterDeductionsPenh - taxPenh;

        // Ενημέρωση οθόνης
        document.getElementById('nightHoursDisplay').innerText = nightHours + ' ώρες';
        document.getElementById('nightGrossTotal').innerText = nightGross.toFixed(2).replace('.',',') + ' €';
        document.getElementById('nightDetails').innerHTML = 
            `Μεικτό: ${formatMoney(nightGross)}<br>` +
            `Εισφ Αλλ 2%: ${formatMoney(eisforiaAllNight)}<br>` +
            `ΜΤΠΥ 2%: ${formatMoney(mtpyNight)}<br>` +
            `Υπόλοιπο: ${formatMoney(afterDeductionsNight)}<br>` +
            `Φόρος 20%: ${formatMoney(taxNight)}<br>` +
            `<strong>Καθαρό: ${formatMoney(nightNet)}</strong>`;

        document.getElementById('penhmeroGrossTotal').innerText = penhmeroGross.toFixed(2).replace('.',',') + ' €';
        document.getElementById('penhmeroDetails').innerHTML = 
            `Μεικτό: ${formatMoney(penhmeroGross)}<br>` +
            `Εισφ Αλλ 2%: ${formatMoney(eisforiaAllPenh)}<br>` +
            `Υπόλοιπο: ${formatMoney(afterDeductionsPenh)}<br>` +
            `Φόρος 20%: ${formatMoney(taxPenh)}<br>` +
            `<strong>Καθαρό: ${formatMoney(penhmeroNet)}</strong>`;

        const totalNet = nightNet + penhmeroNet;
        document.getElementById('nightPenhmeroTotal').innerText = totalNet.toFixed(2).replace('.',',') + ' €';
    }

    function calculateAll() {
        const basic = parseFloat(document.getElementById('basicSalary').value) || 0;
        const dang = parseFloat(document.getElementById('dangerousBonus').value) || 0;
        const ids = parseFloat(document.getElementById('idsynBonus').value) || 0;
        const kidBonus = parseFloat(document.getElementById('childrenBonus').value) || 0;
        const borderBonus = parseFloat(document.getElementById('borderBonus').value) || 0;
        
        const children = parseInt(document.getElementById('numChildrenSelect').value) || 0;
        const age = document.getElementById('ageGroup').value;
        const pouf = parseFloat(document.getElementById('input-pouf').value) || 0;
        const pre1993 = document.getElementById('pre1993Select').value === 'yes';
        
        const tameioAllilov = document.getElementById('tameioAllilov').value === 'yes';
        const kladYgeias = document.getElementById('kladYgeias').value === 'yes';

        const totalBonuses = dang + ids + kidBonus + borderBonus;
        const totalGross = basic + totalBonuses;

        const basicDeductions = basic * 0.2222; // 22,22%

        let bonusDeductions;
        if (pre1993) {
            const pre1993Rate = 0.0205 + 0.02 + 0.01; // 5,05%
            bonusDeductions = totalBonuses * pre1993Rate;
        } else {
            bonusDeductions = totalBonuses * 0.2222;
        }

        let extraDeductions = 0;
        if (tameioAllilov) extraDeductions += 5.83;
        if (kladYgeias) extraDeductions += totalGross * 0.015;

        const totalDeductions = basicDeductions + bonusDeductions + extraDeductions;
        const monthlyPreTax = totalGross - totalDeductions;
        const annualTax = monthlyPreTax * 12;
        const rawTax = calculateTax2026(annualTax, children, age);
        const credit = taxCredit(annualTax, children, age);
        const finalTax = Math.max(0, rawTax - credit);
        const annualNet = annualTax - finalTax;
        const monthlyNet = (annualNet / 12) - pouf;
        const fortnight = monthlyNet / 2;

        const idsMap = ['display-monthly-gross','display-monthly-deductions','display-pre-tax','display-annual-taxable','display-tax','display-monthly-net','display-fortnight','display-annual-net'];
        [totalGross, totalDeductions, monthlyPreTax, annualTax, finalTax, monthlyNet, fortnight, annualNet].forEach((val, i) => {
            let el = document.getElementById(idsMap[i]); if (el) el.textContent = formatMoney(val);
        });

        const tbody = document.getElementById('detailed-table-body');
        if (tbody) {
            let detailsHtml = `
                <tr><td>Βασ. Μισθός</td><td>${formatMoney(basic)}</td></tr>
                <tr><td>Επικίνδυνο</td><td>${formatMoney(dang)}</td></tr>
                <tr><td>Ιδ. Καθηκόντων</td><td>${formatMoney(ids)}</td></tr>
                <tr><td>Επίδ. τέκνων</td><td>${formatMoney(kidBonus)}</td></tr>
                <tr><td>🏔️ Επίδ. Παραμεθορίου</td><td>${formatMoney(borderBonus)}</td></tr>
                <tr><th colspan="2" style="background:#dde8dd">Κρατήσεις Βασικού Μισθού (22,22%)</th></tr>
                <tr><td>ΤΠΔΥ (4%)</td><td>${formatMoney(basic*0.04)}</td></tr>
                <tr><td>ΜΤΠΥ (4,5%)</td><td>${formatMoney(basic*0.045)}</td></tr>
                <tr><td>ΤΕΑΔΥ (3%)</td><td>${formatMoney(basic*0.03)}</td></tr>
                <tr><td>Υγειονομική (2,05%)</td><td>${formatMoney(basic*0.0205)}</td></tr>
                <tr><td>ΕΦΚΑ σύνταξη (6,67%)</td><td>${formatMoney(basic*0.0667)}</td></tr>
                <tr><td>Ανεργία (2%)</td><td>${formatMoney(basic*0.02)}</td></tr>
            `;

            if (pre1993) {
                detailsHtml += `
                    <tr><th colspan="2" style="background:#e6e0c1">Κρατήσεις Επιδομάτων (Προ 1993: 2,05%+2%+1%)</th></tr>
                    <tr><td>Υγειονομική (2,05%)</td><td>${formatMoney(totalBonuses*0.0205)}</td></tr>
                    <tr><td>Ανεργία (2%)</td><td>${formatMoney(totalBonuses*0.02)}</td></tr>
                    <tr><td>ΜΤΠΥ (1%)</td><td>${formatMoney(totalBonuses*0.01)}</td></tr>
                `;
            } else {
                detailsHtml += `
                    <tr><th colspan="2" style="background:#dde8dd">Κρατήσεις Επιδομάτων (22,22%)</th></tr>
                    <tr><td>ΤΠΔΥ (4%)</td><td>${formatMoney(totalBonuses*0.04)}</td></tr>
                    <tr><td>ΜΤΠΥ (4,5%)</td><td>${formatMoney(totalBonuses*0.045)}</td></tr>
                    <tr><td>ΤΕΑΔΥ (3%)</td><td>${formatMoney(totalBonuses*0.03)}</td></tr>
                    <tr><td>Υγειονομική (2,05%)</td><td>${formatMoney(totalBonuses*0.0205)}</td></tr>
                    <tr><td>ΕΦΚΑ σύνταξη (6,67%)</td><td>${formatMoney(totalBonuses*0.0667)}</td></tr>
                    <tr><td>Ανεργία (2%)</td><td>${formatMoney(totalBonuses*0.02)}</td></tr>
                `;
            }
            
            if (tameioAllilov || kladYgeias) {
                detailsHtml += `<tr><th colspan="2" style="background:#e1d7f0">Επιπλέον Κρατήσεις</th></tr>`;
                if (tameioAllilov) {
                    detailsHtml += `<tr><td>Ταμείο Αλληλοβοήθειας</td><td>${formatMoney(5.83)}</td></tr>`;
                }
                if (kladYgeias) {
                    detailsHtml += `<tr><td>Κλάδος Υγείας (1,5%)</td><td>${formatMoney(totalGross*0.015)}</td></tr>`;
                }
            }

            detailsHtml += `
                <tr><th>ΣΥΝΟΛΟ ΚΡΑΤ.</th><td>${formatMoney(totalDeductions)}</td></tr>
                <tr><td>Προ φόρου (μήνας)</td><td>${formatMoney(monthlyPreTax)}</td></tr>
                <tr><td>Ετήσιο φορολογητέο</td><td>${formatMoney(annualTax)}</td></tr>
                <tr><td>Φόρος πριν έκπτ.</td><td>${formatMoney(rawTax)}</td></tr>
                <tr><td>Έκπτωση φόρου</td><td>${formatMoney(credit)}</td></tr>
                <tr><th>ΤΕΛΙΚΟΣ ΦΟΡΟΣ</th><td>${formatMoney(finalTax)}</td></tr>
                <tr><td>ΠΟΥΦ</td><td>${formatMoney(pouf)}</td></tr>
                <tr><th>ΚΑΘΑΡΟ ΜΗΝΑ</th><td>${formatMoney(monthlyNet)}</td></tr>
            `;
            tbody.innerHTML = detailsHtml;
        }
        // Υπολογίζουμε και τα extras (νυχτερινά/πενθήμερα) μαζί
        calculateExtras();
    }

    function updateBasicSalary() {
        const base = parseFloat(document.getElementById('scaleSelect').value) || 1140;
        const coef = parseFloat(document.getElementById('coefSelect').value) || 1.0;
        document.getElementById('basicSalary').value = (base * coef).toFixed(2);
        calculateAll();
    }

    function attachListeners() {
        const ids = ['dangerousBonus','idsynBonus','childrenBonus','borderBonus','numChildrenSelect','ageGroup','input-pouf','scaleSelect','coefSelect','nightCount','penhmeroCount','penhmeroValue','pre1993Select','tameioAllilov','kladYgeias'];
        ids.forEach(id => {
            const el = document.getElementById(id);
            if (!el) return;
            const clone = el.cloneNode(true);
            el.parentNode.replaceChild(clone, el);
            clone.addEventListener('input', (e) => {
                if (e.target.id === 'scaleSelect' || e.target.id === 'coefSelect') updateBasicSalary();
                else calculateAll();
                // calculateExtras καλείται μέσα από calculateAll
            });
            clone.addEventListener('change', (e) => {
                if (e.target.id === 'scaleSelect' || e.target.id === 'coefSelect') updateBasicSalary();
                else calculateAll();
            });
        });
        updateBasicSalary();
        calculateExtras(); // αρχικός υπολογισμός extras
    }

    populateTables();
    if (document.readyState === 'loading') document.addEventListener('DOMContentLoaded', attachListeners);
    else attachListeners();
</script>
</body>
</html>
