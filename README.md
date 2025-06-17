# alprazolam-monograph
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alprazolam Monograph - UMT School of Pharmacy</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src="https://translate.google.com/translate_a/element.js?cb=googleTranslateElementInit"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --primary: #2c3e50;
            --secondary: #1a1a1a;
            --light: #f8f9fa;
            --dark: #212529;
            --gray: #495057;
            --light-gray: #e9ecef;
            --warning-red: #8b0000;
            --warning-bg: #fff0f0;
        }

        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
        }

        /* Header Styles */
        .header-banner {
            background: linear-gradient(to right, #000, #1a1a1a);
            color: white;
            padding: 15px 0;
            box-shadow: 0 2px 15px rgba(0,0,0,0.3);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .school-info {
            display: flex;
            align-items: center;
        }

        .logo-placeholder {
            width: 60px;
            height: 60px;
            background: linear-gradient(145deg, #000, #2c3e50);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            font-weight: bold;
            color: white;
            border: 2px solid #fff;
            box-shadow: 0 0 10px rgba(255,255,255,0.2);
        }

        .school-name {
            font-size: 18px;
            font-weight: 600;
        }

        .school-name span {
            font-size: 14px;
            display: block;
            color: #bbb;
        }

        /* Navigation */
        .nav-buttons {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            justify-content: center;
        }

        .nav-btn {
            background: rgba(255,255,255,0.1);
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 30px;
            font-size: 14px;
            cursor: pointer;
            transition: all 0.3s ease;
            white-space: nowrap;
            display: flex;
            align-items: center;
            gap: 8px;
            border: 1px solid rgba(255,255,255,0.2);
        }

        .nav-btn:hover {
            background: rgba(255,255,255,0.2);
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        }

        /* Main Content */
        .container {
            max-width: 1200px;
            margin: 30px auto;
            padding: 0 20px;
        }

        .monograph-header {
            text-align: center;
            margin-bottom: 40px;
            padding-bottom: 20px;
            border-bottom: 2px solid var(--gray);
        }

        .monograph-header h1 {
            font-size: 36px;
            color: var(--dark);
            margin-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .drug-name {
            color: var(--primary);
            font-weight: 700;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }

        .monograph-card {
            background: white;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            padding: 30px;
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
            border: 1px solid var(--light-gray);
        }

        .monograph-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 5px;
            height: 100%;
            background: linear-gradient(to bottom, #000, #2c3e50);
        }

        .section-title {
            color: var(--dark);
            font-size: 24px;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 1px solid var(--light-gray);
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -1px;
            left: 0;
            width: 80px;
            height: 3px;
            background: var(--dark);
        }

        .brand-names {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin: 15px 0;
        }

        .brand-name {
            background: var(--light);
            color: var(--dark);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 14px;
            border: 1px solid var(--light-gray);
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }

        .highlight {
            background-color: #f8f9fa;
            padding: 5px 10px;
            border-radius: 4px;
            font-weight: 600;
            border-left: 3px solid var(--dark);
        }

        .warning {
            background-color: #f8f9fa;
            color: var(--dark);
            padding: 15px;
            border-left: 4px solid var(--dark);
            margin: 20px 0;
            border-radius: 0 4px 4px 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
        }

        .dosing-section {
            margin: 20px 0;
        }

        .dosing-subsection {
            background-color: var(--light);
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 20px;
            border-left: 3px solid var(--gray);
        }

        .dosing-subsection h4 {
            color: var(--dark);
            margin-bottom: 10px;
            font-size: 18px;
        }

        .dosing-list {
            padding-left: 20px;
        }

        .dosing-list li {
            margin-bottom: 10px;
        }

        .interaction-table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05);
            border: 1px solid var(--light-gray);
        }

        .interaction-table th {
            background-color: var(--dark);
            color: white;
            text-align: left;
            padding: 15px;
            font-weight: 600;
        }

        .interaction-table td {
            padding: 12px 15px;
            border-bottom: 1px solid var(--light-gray);
        }

        .interaction-table tr:nth-child(even) {
            background-color: var(--light);
        }

        .interaction-table tr:hover {
            background-color: #e9ecef;
        }

        .image-container {
            text-align: center;
            margin: 25px 0;
        }

        .image-container img {
            max-width: 100%;
            height: auto;
            border: 1px solid var(--light-gray);
            border-radius: 8px;
            box-shadow: 0 3px 12px rgba(0,0,0,0.08);
        }

        .image-caption {
            font-size: 14px;
            color: var(--gray);
            margin-top: 8px;
            font-style: italic;
        }

        .video-container {
            margin: 30px 0;
            text-align: center;
        }

        .video-wrapper {
            position: relative;
            padding-bottom: 56.25%; /* 16:9 aspect ratio */
            height: 0;
            overflow: hidden;
            max-width: 800px;
            margin: 0 auto;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .video-wrapper iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
            border-radius: 8px;
        }

        .brands-table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05);
            border: 1px solid var(--light-gray);
        }

        .brands-table th {
            background-color: var(--dark);
            color: white;
            padding: 15px;
            text-align: left;
        }

        .brands-table td {
            padding: 12px 15px;
            border-bottom: 1px solid var(--light-gray);
        }

        .brands-table tr:nth-child(even) {
            background-color: var(--light);
        }

        .references {
            list-style-type: none;
            padding: 0;
        }

        .references li {
            margin-bottom: 10px;
            padding-left: 20px;
            position: relative;
        }

        .references li::before {
            content: '•';
            position: absolute;
            left: 0;
            color: var(--dark);
            font-weight: bold;
        }

        /* FDA Box Warning */
        .fda-warning {
            background-color: var(--warning-bg);
            border: 2px solid var(--warning-red);
            border-radius: 8px;
            padding: 25px;
            margin: 30px 0;
            position: relative;
            box-shadow: 0 4px 12px rgba(139, 0, 0, 0.15);
        }

        .fda-header {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
            color: var(--warning-red);
        }

        .fda-icon {
            font-size: 28px;
            margin-right: 12px;
        }

        .fda-title {
            font-size: 24px;
            font-weight: 700;
        }

        .fda-content {
            line-height: 1.7;
            font-size: 17px;
        }

        .fda-content p {
            margin-bottom: 15px;
        }

        .fda-content strong {
            color: var(--warning-red);
        }

        /* Auxiliary Labels */
        .auxiliary-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
            margin-top: 25px;
        }

        .aux-label {
            background-color: #fff;
            border-radius: 10px;
            padding: 25px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
            border: 1px solid #e0e0e0;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .aux-label:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
        }

        .aux-label::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 8px;
            height: 100%;
            background: linear-gradient(to bottom, #2c3e50, #1a1a1a);
        }

        .label-title {
            font-size: 20px;
            color: #2c3e50;
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 1px dashed #d0d0d0;
            font-weight: 600;
        }

        .label-content {
            font-size: 16px;
            line-height: 1.6;
        }

        .label-icon {
            display: block;
            text-align: center;
            font-size: 36px;
            margin-bottom: 15px;
            color: #2c3e50;
        }

        /* Footer */
        .footer {
            background: linear-gradient(to right, #000, #1a1a1a);
            color: white;
            padding: 40px 0;
            text-align: center;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .documented-by {
            font-size: 18px;
            margin-bottom: 20px;
            letter-spacing: 0.5px;
        }

        .translation-section {
            margin-top: 30px;
            background: rgba(255,255,255,0.1);
            padding: 20px;
            border-radius: 8px;
            display: inline-block;
        }

        .translation-title {
            margin-bottom: 15px;
            font-size: 18px;
            color: #ddd;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                gap: 15px;
            }
            
            .nav-buttons {
                width: 100%;
                overflow-x: auto;
                padding-bottom: 5px;
                justify-content: flex-start;
            }
            
            .monograph-header h1 {
                font-size: 28px;
            }
            
            .monograph-card {
                padding: 20px 15px;
            }
            
            .nav-btn {
                padding: 8px 12px;
                font-size: 12px;
            }
            
            .auxiliary-container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header Banner -->
    <header class="header-banner">
        <div class="header-container">
            <div class="school-info">
                <div class="logo-placeholder">UMT</div>
                <div class="school-name">
                    UNIVERSITY OF MANAGEMENT AND TECHNOLOGY
                    <span>SCHOOL OF PHARMACY</span>
                </div>
            </div>
            <div class="nav-buttons">
                <button class="nav-btn" onclick="scrollToSection('mechanism')">
                    <i class="fas fa-brain"></i> Mechanism
                </button>
                <button class="nav-btn" onclick="scrollToSection('indications')">
                    <i class="fas fa-stethoscope"></i> Indications
                </button>
                <button class="nav-btn" onclick="scrollToSection('dosing')">
                    <i class="fas fa-pills"></i> Dosing
                </button>
                <button class="nav-btn" onclick="scrollToSection('kinetics')">
                    <i class="fas fa-chart-line"></i> Kinetics
                </button>
                <button class="nav-btn" onclick="scrollToSection('interactions')">
                    <i class="fas fa-exchange-alt"></i> Interactions
                </button>
                <button class="nav-btn" onclick="scrollToSection('safety')">
                    <i class="fas fa-exclamation-triangle"></i> Safety
                </button>
                <button class="nav-btn" onclick="scrollToSection('fda')">
                    <i class="fas fa-exclamation-circle"></i> FDA Warning
                </button>
            </div>
        </div>
    </header>

    <div class="container">
        <!-- Drug Monograph Header -->
        <div class="monograph-header">
            <h1>DRUG MONOGRAPH: <span class="drug-name">ALPRAZOLAM</span></h1>
            <p>(al·pray·zuh·lam)</p>
        </div>

        <!-- Introduction Section -->
        <div class="monograph-card">
            <h2 class="section-title">Introduction</h2>
            <div class="brand-names">
                <div class="brand-name">Xanax</div>
                <div class="brand-name">Alp</div>
                <div class="brand-name">Pralzo</div>
                <div class="brand-name">Alprazolam</div>
                <div class="brand-name">Pranax</div>
                <div class="brand-name">Zenith</div>
            </div>
            
            <p><strong>Chemical Name:</strong> 8-Chloro-1-methyl-6-phenyl-4H-s-triazolo [4,3-α] [1,4] benzodiazepine</p>
            <p><strong>Molecular Formula:</strong> C<sub>17</sub>H<sub>14</sub>ClN<sub>4</sub></p>
            <p><strong>Class:</strong> Benzodiazepines (Schedule IV)</p>
            
            <div class="image-container">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/cb/Alprazolam.svg/800px-Alprazolam.svg.png" alt="Alprazolam Chemical Structure" style="max-width: 300px;">
                <div class="image-caption">Chemical Structure of Alprazolam</div>
            </div>
            
            <p><strong>Introduction:</strong> Anticonvulsant, anxiolytic, muscle relaxant and hypnotic.</p>
            
            <p><span class="highlight">Alprazolam was invented by Jackson Hester Jr. at the Upjohn Company and patented in 1971 and approved for medical use in the United States in 1981.</span> Alprazolam is a Schedule IV controlled substance and is a common drug of abuse. It is available as a generic medication. In 2022, it was the 41st most commonly prescribed medication in the United States, with more than 14 million prescriptions.</p>
        </div>

        <!-- Mechanism of Action -->
        <div class="monograph-card" id="mechanism">
            <h2 class="section-title">Mechanism of Action</h2>
            <p>Alprazolam acts by binding to the benzodiazepine derivatives site on the GABA(A) receptor to enhance the affinity of channel opening by the agonist gamma-Aminobutyric acid (GABA), which leads to central nervous system depression.</p>
            
            <div class="image-container">
                <img src="https://www.mdpi.com/pharmaceuticals/pharmaceuticals-16-00331/article_deploy/html/images/pharmaceuticals-16-00331-g005.png" 
alt="Mechanism of Action" style="max-width: 400px;">
                <div class="image-caption">Alprazolam Mechanism of Action</div>
            </div>
        </div>

        <!-- Indications -->
        <div class="monograph-card" id="indications">
            <h2 class="section-title">Indications</h2>
            <ul class="dosing-list">
                <li><strong>Generalised Anxiety Disorder</strong></li>
                <li><strong>Panic Disorder</strong></li>
            </ul>
        </div>

        <!-- Dosing Section -->
        <div class="monograph-card" id="dosing">
            <h2 class="section-title">Dosing</h2>
            
            <div class="dosing-section">
                <h3>1. Anxiety Disorders</h3>
                <div class="dosing-subsection">
                    <h4>Adults</h4>
                    <ul class="dosing-list">
                        <li><strong>Form:</strong> IR tablets, ODT, oral solution</li>
                        <li><strong>Dose:</strong> 0.25-0.5 mg PO TID</li>
                        <li><strong>Titration:</strong> Increase every 3-4 days by no more than 1 mg/day</li>
                        <li><strong>Maximum:</strong> 4 mg/day</li>
                    </ul>
                </div>
                
                <div class="dosing-subsection">
                    <h4>Geriatric Patients</h4>
                    <ul class="dosing-list">
                        <li><strong>Dose:</strong> 0.25 mg PO BID or TID</li>
                    </ul>
                </div>
            </div>
            
            <div class="dosing-section">
                <h3>2. Panic Disorder</h3>
                <div class="dosing-subsection">
                    <h4>Adults</h4>
                    <p><strong>Immediate-Release / ODT / Solution:</strong></p>
                    <ul class="dosing-list">
                        <li><strong>Initial:</strong> 0.5 mg PO TID</li>
                        <li><strong>Maximum:</strong> 10 mg/day</li>
                    </ul>
                    
                    <p><strong>Extended-Release:</strong></p>
                    <ul class="dosing-list">
                        <li><strong>Initial:</strong> 0.5-1 mg PO once daily</li>
                        <li><strong>Maintenance:</strong> 3-6 mg/day</li>
                        <li><strong>Maximum:</strong> 10 mg/day</li>
                    </ul>
                </div>
                
                <div class="dosing-subsection">
                    <h4>Geriatric Patients</h4>
                    <p><strong>Immediate-Release / ODT / Solution:</strong></p>
                    <ul class="dosing-list">
                        <li><strong>Dose:</strong> 0.25 mg PO BID or TID</li>
                    </ul>
                    
                    <p><strong>Extended-Release:</strong></p>
                    <ul class="dosing-list">
                        <li><strong>Dose:</strong> 0.5 mg PO once daily</li>
                    </ul>
                </div>
            </div>
            
            <div class="dosing-section">
                <h3>3. Dose Adjustments in Hepatic Impairment</h3>
                <div class="dosing-subsection">
                    <ul class="dosing-list">
                        <li><strong>Immediate-Release / ODT:</strong> Recommended dose: 0.25 mg PO BID or TID</li>
                        <li><strong>Extended-Release:</strong> Recommended dose: 0.5 mg PO once daily</li>
                    </ul>
                </div>
                
                <div class="warning">
                    <strong>Note:</strong> Titrate slowly and monitor closely for sedation or respiratory depression due to reduced drug clearance.
                </div>
            </div>
        </div>

        <!-- Off-Label Uses -->
        <div class="monograph-card">
            <h2 class="section-title">Off-Label Uses</h2>
            <ul class="dosing-list">
                <li>Pre menstrual syndrome (PMS)</li>
                <li>Depression</li>
                <li>Insomnia</li>
                <li>Alcohol Withdrawal</li>
            </ul>
        </div>

        <!-- Pharmacokinetics -->
        <div class="monograph-card" id="kinetics">
            <h2 class="section-title">Pharmacokinetics</h2>
            <h3>Pharmacokinetic Parameters of Alprazolam</h3>
            
            <p><strong>Absorption:</strong></p>
            <ul class="dosing-list">
                <li><strong>Route:</strong> Oral</li>
                <li><strong>Bioavailability:</strong> 80% to 100%</li>
                <li><strong>Time to Peak Plasma Concentration (Tmax):</strong> 1 to 2 hours</li>
                <li><strong>Onset of Action:</strong> ~30 minutes</li>
                <li><strong>Formulations:</strong> Immediate-release, extended-release, orally disintegrating tablets, and oral solution</li>
            </ul>
            
            <p><strong>Distribution</strong></p>
            <ul class="dosing-list">
                <li><strong>Plasma Protein Binding:</strong> ~80% (mainly to albumin)</li>
                <li><strong>Volume of Distribution:</strong> 0.8-1.3L/kg</li>
                <li><strong>Crosses the Blood-Brain Barrier and Placenta</strong></li>
            </ul>
            
            <p><strong>Metabolism</strong></p>
            <ul class="dosing-list">
                <li><strong>Primary Site:</strong> Liver</li>
                <li><strong>Primary Enzyme:</strong> Cytochrome P450 3A4 (CYP3A4)</li>
                <li><strong>Metabolites:</strong> Alpha-hydroxyalprazolam, 4-hydroxyalprazolam, Inactive benzophenone derivatives</li>
            </ul>
            
            <p><strong>Excretion</strong></p>
            <ul class="dosing-list">
                <li><strong>Route:</strong> Renal (urine)</li>
                <li><strong>Excreted as:</strong> Metabolites and small amounts of unchanged drug</li>
                <li><strong>Half-life (t½):</strong> Healthy adults: 11.2 hours; Elderly or hepatic impairment: 16-20 hours</li>
            </ul>
            
            <p><strong>Special Considerations</strong></p>
            <ul class="dosing-list">
                <li><strong>Renal Impairment:</strong> Use caution; initiate at low doses</li>
                <li><strong>Hepatic Impairment:</strong> Reduced metabolism—start with lowest effective dose</li>
                <li><strong>Pregnancy Category:</strong> D (crosses placenta, potential neonatal toxicity)</li>
                <li><strong>Lactation:</strong> Detected in breast milk; avoid if possible</li>
            </ul>
        </div>

        <!-- Contraindications -->
        <div class="monograph-card" id="safety">
            <h2 class="section-title">Contraindications</h2>
            <ul class="dosing-list">
                <li>Known hypersensitivity or allergy to alprazolam or other benzodiazepines</li>
                <li>Acute narrow-angle glaucoma</li>
                <li>Severe respiratory insufficiency (e.g., COPD, sleep apnea)</li>
                <li>Myasthenia gravis</li>
                <li>Severe liver impairment (due to metabolism concerns)</li>
                <li>Pregnancy and breastfeeding (due to fetal/neonatal risks)</li>
            </ul>
        </div>

        <!-- Adverse Effects -->
        <div class="monograph-card">
            <h2 class="section-title">Adverse Effects</h2>
            <div style="display: grid; grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)); gap: 20px;">
                <div>
                    <p><strong>Common Effects:</strong></p>
                    <ul class="dosing-list">
                        <li>Memory impairment</li>
                        <li>Poor coordination or balance</li>
                        <li>Drowsiness</li>
                        <li>Slurred speech</li>
                        <li>Headache</li>
                        <li>Sexual dysfunction</li>
                        <li>Dry mouth</li>
                        <li>Constipation</li>
                        <li>Dizziness</li>
                        <li>Nausea</li>
                        <li>Hypotension</li>
                        <li>Fatigue</li>
                        <li>Dermatitis</li>
                    </ul>
                </div>
                <div>
                    <p><strong>Uncommon Effects:</strong></p>
                    <ul class="dosing-list">
                        <li>Paradoxical reactions</li>
                        <li>Menstruation irregular</li>
                        <li>Urinary incontinence</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Pregnancy & Lactation -->
        <div class="monograph-card">
            <h2 class="section-title">Pregnancy Category</h2>
            <div class="warning">
                <p><strong>Category D</strong> — Contraindicated in pregnancy.</p>
                <p>Alprazolam is contraindicated in pregnancy because it crosses the placenta and may cause fetal harm, including congenital malformations (such as cleft lip or palate) when used in the first trimester, and serious neonatal complications like sedation, respiratory depression, hypotonia, and withdrawal symptoms if used later in pregnancy.</p>
            </div>
            
            <h3 style="margin-top: 20px; color: var(--dark);">Lactation</h3>
            <p>Contraindicated or not recommended.</p>
        </div>

        <!-- Drug Interactions -->
        <div class="monograph-card" id="interactions">
            <h2 class="section-title">Drug Interactions</h2>
            <table class="interaction-table">
                <thead>
                    <tr>
                        <th>Interacting drug</th>
                        <th>Mechanism</th>
                        <th>Outcome</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><strong>Ketoconazole, Itraconazole</strong></td>
                        <td>Strong CYP3A4 inhibitor</td>
                        <td>↑ Risk of sedation, ↑ Respiratory depression, ↑ Toxicity</td>
                    </tr>
                    <tr>
                        <td><strong>Rifampin</strong></td>
                        <td>Strong CYP3A4 inducer</td>
                        <td>↓ Reduce therapeutic effect of alprazolam → therapeutic failure</td>
                    </tr>
                    <tr>
                        <td><strong>Opioids</strong></td>
                        <td>Additive CNS depression</td>
                        <td>Profound sedation, respiratory depression, coma or death</td>
                    </tr>
                    <tr>
                        <td><strong>Oral contraceptive</strong></td>
                        <td>Hormonal modulation of CYP enzymes</td>
                        <td>↑ Alprazolam levels in plasma → toxicity</td>
                    </tr>
                    <tr>
                        <td><strong>Grapefruit juice</strong></td>
                        <td>Inhibit CYP3A4 enzyme</td>
                        <td>↑ Bioavailability and Plasma Concentration of alprazolam → toxicity</td>
                    </tr>
                </tbody>
            </table>
            
            <div class="image-container">
                <img src="https://www.drugs.com/pro/images/d9b0e228-17cf-40d7-b62e-5050311c571c/0-5mglabel.jpg" 
alt="Drug Interactions" style="max-width: 500px;">
                <div class="image-caption">Alprazolam Drug Interaction Pathways</div>
            </div>
        </div>

        <!-- FDA Box Warning -->
        <div class="monograph-card" id="fda">
            <h2 class="section-title">FDA Box Warning</h2>
            <div class="fda-warning">
                <div class="fda-header">
                    <div class="fda-icon"><i class="fas fa-exclamation-triangle"></i></div>
                    <div class="fda-title">FDA BLACK BOX WARNING</div>
                </div>
                <div class="fda-content">
                    <p><strong>CONCOMITANT USE OF BENZODIAZEPINES AND OPIOIDS</strong></p>
                    <p>Concomitant use of benzodiazepines and opioids may result in profound sedation, respiratory depression, coma, and death.</p>
                    <p><strong>RISKS INCLUDE:</strong></p>
                    <ul class="dosing-list">
                        <li>Profound sedation</li>
                        <li>Respiratory depression</li>
                        <li>Coma</li>
                        <li>Death</li>
                    </ul>
                    <p><strong>PRESCRIBING RECOMMENDATIONS:</strong></p>
                    <ul class="dosing-list">
                        <li>Reserve concomitant prescribing for patients with inadequate alternative treatment options</li>
                        <li>Limit dosages and durations to the minimum required</li>
                        <li>Monitor patients for signs and symptoms of respiratory depression and sedation</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Auxiliary Labels -->
        <div class="monograph-card" id="auxiliary">
            <h2 class="section-title">Auxiliary Labels</h2>
            <p>Important labels to include with alprazolam prescriptions to ensure safe use:</p>
            
            <div class="auxiliary-container">
                <div class="aux-label">
                    <div class="label-icon"><i class="fas fa-capsules"></i></div>
                    <h3 class="label-title">Take Exactly as Prescribed</h3>
                    <div class="label-content">
                        Do not increase dose or frequency without consulting your healthcare provider. Benzodiazepines can cause dependence.
                    </div>
                </div>
                
                <div class="aux-label">
                    <div class="label-icon"><i class="fas fa-car-crash"></i></div>
                    <h3 class="label-title">May Cause Drowsiness</h3>
                    <div class="label-content">
                        Avoid driving or operating machinery until you know how this medication affects you. Alcohol may increase drowsiness.
                    </div>
                </div>
                
                <div class="aux-label">
                    <div class="label-icon"><i class="fas fa-exclamation-circle"></i></div>
                    <h3 class="label-title">Do Not Stop Suddenly</h3>
                    <div class="label-content">
                        Abrupt discontinuation may cause withdrawal symptoms. Consult your doctor for a gradual tapering schedule.
                    </div>
                </div>
                
                <div class="aux-label">
                    <div class="label-icon"><i class="fas fa-wine-bottle"></i></div>
                    <h3 class="label-title">Avoid Alcohol</h3>
                    <div class="label-content">
                        Alcohol increases sedative effects and risk of respiratory depression. Do not consume alcoholic beverages while taking this medication.
                    </div>
                </div>
                
                <div class="aux-label">
                    <div class="label-icon"><i class="fas fa-pills"></i></div>
                    <h3 class="label-title">Potential for Abuse</h3>
                    <div class="label-content">
                        This medication has potential for abuse and may lead to addiction. Keep in a secure location and never share with others.
                    </div>
                </div>
                
                <div class="aux-label">
                    <div class="label-icon"><i class="fas fa-user-md"></i></div>
                    <h3 class="label-title">Medical Supervision Required</h3>
                    <div class="label-content">
                        Regular monitoring by healthcare provider is essential. Report any unusual thoughts, behaviors, or side effects immediately.
                    </div>
                </div>
            </div>
        </div>

        <!-- Storage -->
        <div class="monograph-card">
            <h2 class="section-title">Storage</h2>
            <p>Store Alprazolam in a cool, dry place away from direct sunlight and moisture, at room temperature (15-25°C).</p>
            
            <div class="video-container">
                <h3>Alprazolam Educational Video</h3>
                <div class="video-wrapper">
                    <iframe src="https://www.youtube.com/embed/lcjISUSwNyk" title="Alprazolam Educational Video" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
                <p class="image-caption">Understanding Alprazolam: Mechanisms, Uses, and Safety</p>
            </div>
        </div>

        <!-- Common Brands -->
        <div class="monograph-card">
            <h2 class="section-title">Common Brands in Pakistan</h2>
            <table class="brands-table">
                <thead>
                    <tr>
                        <th>Brand Name</th>
                        <th>Manufacturer</th>
                        <th>Strength</th>
                        <th>Form</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Xanax</td>
                        <td>Pfizer</td>
                        <td>0.25mg, 0.5mg, 1mg, 2mg</td>
                        <td>Tablets</td>
                    </tr>
                    <tr>
                        <td>Alp</td>
                        <td>High-Q Pharmaceuticals</td>
                        <td>0.25mg, 0.5mg</td>
                        <td>Tablets</td>
                    </tr>
                    <tr>
                        <td>Pralzo</td>
                        <td>Samson's Pharma</td>
                        <td>0.5mg, 1mg</td>
                        <td>Tablets</td>
                    </tr>
                    <tr>
                        <td>Alprazolam</td>
                        <td>Various Generics</td>
                        <td>0.25mg, 0.5mg, 1mg</td>
                        <td>Tablets</td>
                    </tr>
                    <tr>
                        <td>Pranax</td>
                        <td>Wilson's Pharmaceuticals</td>
                        <td>0.5mg, 1mg</td>
                        <td>Tablets</td>
                    </tr>
                    <tr>
                        <td>Zenith</td>
                        <td>Novus Life Sciences</td>
                        <td>0.25mg, 0.5mg</td>
                        <td>Tablets</td>
                    </tr>
                </tbody>
            </table>
        </div>

        <!-- References -->
        <div class="monograph-card">
            <h2 class="section-title">References</h2>
            <ol class="references">
                <li>BNF 2024-25</li>
                <li>PharmaGuide, 31st edition</li>
                <li>Wikipedia - Alprazolam</li>
                <li>Medscape</li>
                <li>NIH - Alprazolam</li>
                <li>FDA Drug Safety Communication (2020)</li>
                <li>Clinical Pharmacology of Alprazolam, Journal of Clinical Psychiatry</li>
            </ol>
        </div>
    </div>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer-content">
            <div class="documented-by">Documented by Adan Ali</div>
            
            <div class="translation-section">
                <div class="translation-title">Translation</div>
                <div id="google_translate_element"></div>
            </div>
        </div>
    </footer>

    <script>
        // Google Translate initialization
        function googleTranslateElementInit() {
            new google.translate.TranslateElement({
                pageLanguage: 'en',
                includedLanguages: 'en,ur',
                layout: google.translate.TranslateElement.InlineLayout.SIMPLE
            }, 'google_translate_element');
        }
        
        // Smooth scrolling to sections
        function scrollToSection(sectionId) {
            const element = document.getElementById(sectionId);
            if (element) {
                window.scrollTo({
                    top: element.offsetTop - 80,
                    behavior: 'smooth'
                });
            }
        }
        
        // Highlight active nav button
        const navButtons = document.querySelectorAll('.nav-btn');
        navButtons.forEach(button => {
            button.addEventListener('click', function() {
                navButtons.forEach(btn => {
                    btn.style.background = 'rgba(255,255,255,0.1)';
                    btn.style.boxShadow = 'none';
                });
                this.style.background = 'rgba(255,255,255,0.2)';
                this.style.boxShadow = '0 4px 8px rgba(0,0,0,0.2)';
            });
        });
    </script>
</body>
</html>
