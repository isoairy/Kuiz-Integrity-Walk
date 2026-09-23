<!DOCTYPE html>
<html lang="ms">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Integrity Walk JPN Pahang 2026</title>

    <style>
        /* -------------------------------------------------------------
           1. MODERN MOBILE-FIRST ATHLETIC THEME (CSS)
           ------------------------------------------------------------- */
        @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;700;800&display=swap');

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Plus Jakarta Sans', sans-serif;
            -webkit-tap-highlight-color: transparent;
        }

        :root {
            --primary-blue: #0284c7;
            --primary-dark: #0f172a;
            --sports-orange: #f97316;
            --sports-amber: #f59e0b;
            --sports-green: #10b981;
            --bg-gradient: linear-gradient(160deg, #0f172a 0%, #1e293b 50%, #0369a1 100%);
            --glass-bg: rgba(255, 255, 255, 0.96);
            --card-shadow: 0 12px 32px rgba(0, 0, 0, 0.3);
        }

        body {
            background: var(--bg-gradient);
            background-attachment: fixed;
            min-height: 100vh;
            padding: 12px;
            color: #1e293b;
        }

        .container {
            max-width: 480px;
            margin: 0 auto;
            padding-bottom: 24px;
        }

        /* Glass Cards */
        .glass-card {
            background: var(--glass-bg);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border-radius: 24px;
            box-shadow: var(--card-shadow);
            padding: 20px;
            margin-bottom: 16px;
            border: 1px solid rgba(255, 255, 255, 0.5);
            position: relative;
            overflow: hidden;
        }

        /* Header */
        header {
            text-align: center;
            padding: 18px 14px;
            background: #ffffff;
            border-bottom: 5px solid var(--sports-orange);
        }

        .badge-tag {
            display: inline-flex;
            align-items: center;
            gap: 4px;
            background: #fff7ed;
            color: #c2410c;
            font-size: 0.68rem;
            font-weight: 800;
            padding: 5px 12px;
            border-radius: 20px;
            text-transform: uppercase;
            letter-spacing: 0.8px;
            margin-bottom: 8px;
            border: 1px solid #ffedd5;
        }

        header h1 {
            font-size: 1.35rem;
            font-weight: 800;
            color: var(--primary-dark);
            line-height: 1.2;
            letter-spacing: -0.5px;
        }

        header h1 span {
            color: var(--sports-orange);
        }

        .event-stats-bar {
            display: flex;
            justify-content: space-around;
            background: #f8fafc;
            border-radius: 12px;
            padding: 8px;
            margin-top: 12px;
            border: 1px solid #e2e8f0;
            font-size: 0.72rem;
            font-weight: 700;
            color: #475569;
        }

        .stat-item { display: flex; align-items: center; gap: 4px; }

        /* Action Buttons Mobile Optimized */
        .btn-action {
            width: 100%;
            min-height: 54px;
            border: none;
            border-radius: 18px;
            padding: 14px 18px;
            margin-bottom: 12px;
            font-weight: 800;
            font-size: 0.92rem;
            color: #ffffff;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 6px 16px rgba(0, 0, 0, 0.15);
            transition: transform 0.1s ease, box-shadow 0.1s ease;
        }

        .btn-action:active {
            transform: scale(0.97);
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
        }

        .btn-primary { background: linear-gradient(135deg, #0284c7, #2563eb); }
        .btn-warning { background: linear-gradient(135deg, #ea580c, #f59e0b); }
        .btn-success { background: linear-gradient(135deg, #059669, #10b981); }

        .btn-secondary {
            background: #f1f5f9;
            color: #334155;
            font-weight: 700;
            padding: 12px 16px;
            border-radius: 14px;
            font-size: 0.8rem;
            border: 1px solid #cbd5e1;
            cursor: pointer;
            width: 100%;
            margin-bottom: 14px;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 6px;
        }

        .btn-secondary:active { background: #e2e8f0; }

        /* Helpers */
        .hidden { display: none !important; }
        .text-center { text-align: center; }
        .mb-2 { margin-bottom: 8px; }
        .mb-3 { margin-bottom: 12px; }
        .mb-4 { margin-bottom: 16px; }

        /* Select Mobile Custom */
        select {
            width: 100%;
            min-height: 50px;
            padding: 12px 16px;
            border-radius: 16px;
            border: 2px solid #38bdf8;
            font-weight: 700;
            font-size: 0.95rem;
            background-color: #f0f9ff;
            color: #0c4a6e;
            text-align: center;
            margin-bottom: 14px;
            outline: none;
            appearance: none;
            -webkit-appearance: none;
            box-shadow: inset 0 2px 4px rgba(0,0,0,0.02);
        }

        /* Checkpoint Selection Grid (Penjana QR) */
        .cp-select-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 12px;
            margin-top: 10px;
        }

        .btn-cp-card {
            background: #ffffff;
            border: 2px solid #e2e8f0;
            border-radius: 18px;
            padding: 16px 12px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 6px;
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
            transition: all 0.15s ease;
        }

        .btn-cp-card:active {
            transform: scale(0.96);
            border-color: var(--sports-orange);
            background: #fff7ed;
        }

        .btn-cp-card .cp-num {
            font-size: 1.1rem;
            font-weight: 800;
            color: var(--primary-dark);
        }

        .btn-cp-card .cp-tag {
            font-size: 0.65rem;
            font-weight: 800;
            background: #e0f2fe;
            color: #0369a1;
            padding: 3px 8px;
            border-radius: 10px;
        }

        /* Grid Masa Ketibaan */
        .grid-teams {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 8px;
            max-height: 320px;
            overflow-y: auto;
            padding: 4px;
        }

        .btn-team-square {
            background: #fffbeb;
            color: #78350f;
            font-weight: 800;
            padding: 12px 4px;
            border-radius: 14px;
            border: 1px solid #fde68a;
            cursor: pointer;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 52px;
        }

        .btn-team-square:active {
            background: #f59e0b;
            color: #ffffff;
            transform: scale(0.92);
        }

        /* Modal Overlay (Universal) */
        .modal-overlay {
            position: fixed;
            top: 0; left: 0; right: 0; bottom: 0;
            background: rgba(15, 23, 42, 0.82);
            backdrop-filter: blur(6px);
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 200;
            padding: 18px;
        }

        .modal-box {
            background: #ffffff;
            border-radius: 24px;
            padding: 24px;
            max-width: 340px;
            width: 100%;
            text-align: center;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.35);
            animation: modalPop 0.2s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        @keyframes modalPop {
            0% { transform: scale(0.8); opacity: 0; }
            100% { transform: scale(1); opacity: 1; }
        }

        .modal-time {
            font-size: 1.35rem;
            font-weight: 800;
            color: #1e3a8a;
            background: #eff6ff;
            padding: 10px;
            border-radius: 14px;
            margin: 10px 0;
            border: 1px solid #bfdbfe;
        }

        .modal-actions {
            display: flex;
            gap: 10px;
        }

        .modal-actions button {
            flex: 1;
            padding: 14px;
            border-radius: 14px;
            border: none;
            font-weight: 800;
            font-size: 0.82rem;
            cursor: pointer;
        }

        /* Quiz Buttons (Touch Friendly) */
        .quiz-option-btn {
            width: 100%;
            min-height: 52px;
            text-align: left;
            padding: 14px 16px;
            border-radius: 16px;
            border: 2px solid #e2e8f0;
            background: #ffffff;
            font-weight: 600;
            font-size: 0.88rem;
            margin-bottom: 10px;
            cursor: pointer;
            line-height: 1.4;
            color: #334155;
            transition: all 0.15s ease;
            box-shadow: 0 2px 4px rgba(0,0,0,0.02);
        }

        .quiz-option-btn:active {
            transform: scale(0.98);
        }

        .quiz-option-btn.selected {
            background: #eff6ff;
            border-color: #2563eb;
            color: #1e40af;
            font-weight: 700;
            box-shadow: 0 0 0 2px rgba(37, 99, 235, 0.2);
        }

        /* Leaderboard Mobile Cards */
        .leaderboard-list {
            display: flex;
            flex-direction: column;
            gap: 12px;
            max-height: 420px;
            overflow-y: auto;
            padding-right: 2px;
        }

        .team-card {
            background: #ffffff;
            border: 1px solid #e2e8f0;
            border-radius: 18px;
            padding: 14px;
            display: flex;
            flex-direction: column;
            gap: 10px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.03);
        }

        .team-card-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .team-title {
            font-weight: 800;
            color: #0f172a;
            font-size: 0.9rem;
        }

        .team-score-badge {
            background: #fffbeb;
            color: #d97706;
            border: 1px solid #fde68a;
            font-weight: 800;
            font-size: 0.82rem;
            padding: 4px 12px;
            border-radius: 20px;
        }

        .cp-grid {
            display: grid;
            grid-template-columns: repeat(6, 1fr);
            gap: 4px;
            background: #f8fafc;
            padding: 8px;
            border-radius: 12px;
            text-align: center;
            font-size: 0.68rem;
            font-weight: 700;
            border: 1px solid #f1f5f9;
        }

        .cp-item {
            display: flex;
            flex-direction: column;
            gap: 2px;
        }

        .cp-label {
            color: #94a3b8;
            font-size: 0.58rem;
        }

        .team-card-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-size: 0.75rem;
            color: #64748b;
        }

        .finish-time-text {
            color: #059669;
            font-weight: 800;
        }

        .btn-edit-small {
            background: #f1f5f9;
            color: #334155;
            border: 1px solid #cbd5e1;
            padding: 6px 12px;
            border-radius: 10px;
            font-weight: 700;
            font-size: 0.7rem;
            cursor: pointer;
        }

        .flash-screen {
            background: #ecfdf5;
            border: 2px solid #10b981;
            color: #065f46;
            padding: 14px;
            border-radius: 16px;
            font-weight: 700;
            margin-bottom: 12px;
        }

        /* Progress Bar Checkpoint Kuiz */
        .quiz-progress {
            height: 6px;
            width: 100%;
            background: #e2e8f0;
            border-radius: 10px;
            overflow: hidden;
            margin-bottom: 14px;
        }
        .quiz-progress-bar {
            height: 100%;
            background: var(--sports-orange);
            width: 50%;
            transition: width 0.2s ease;
        }

        /* -------------------------------------------------------------
           2. FORMAT PRINT / PDF LAPORAN RASMI (CSS)
           ------------------------------------------------------------- */
        @media print {
            body {
                background: #ffffff !important;
                color: #000000 !important;
                padding: 0 !important;
            }

            .container {
                max-width: 100% !important;
                padding: 0 !important;
            }

            header, 
            #view-home, 
            #view-admin-qr, 
            #view-finish-recorder, 
            #view-participant-start, 
            #view-quiz, 
            #view-completion,
            .btn-secondary,
            .btn-edit-small,
            .no-print {
                display: none !important;
            }

            #view-leaderboard {
                display: block !important;
                background: none !important;
                box-shadow: none !important;
                border: none !important;
                padding: 0 !important;
            }

            .print-header {
                display: block !important;
                text-align: center;
                border-bottom: 2px solid #000000;
                padding-bottom: 12px;
                margin-bottom: 20px;
            }

            .print-header h1 {
                font-size: 1.5rem;
                color: #000000;
                text-transform: uppercase;
            }

            .leaderboard-list {
                max-height: none !important;
                overflow: visible !important;
                display: grid !important;
                grid-template-columns: repeat(2, 1fr) !important;
                gap: 10px !important;
            }

            .team-card {
                border: 1px solid #000000 !important;
                box-shadow: none !important;
                break-inside: avoid;
                page-break-inside: avoid;
            }

            .print-footer {
                display: flex !important;
                justify-content: space-between;
                margin-top: 40px;
                padding-top: 20px;
                page-break-inside: avoid;
            }

            .sig-box {
                text-align: center;
                width: 200px;
            }

            .sig-line {
                border-bottom: 1px solid #000000;
                margin-top: 50px;
                margin-bottom: 5px;
            }
        }

        .print-header, .print-footer {
            display: none;
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- HEADER UTAMA -->
        <header class="glass-card">
            <span class="badge-tag">🏃 JPN PAHANG OFFICIAL 🏃</span>
            <h1>INTEGRITY WALK <span>2026</span></h1>
            
            <div class="event-stats-bar">
                <div class="stat-item">📍 <span>3.0 KM</span></div>
                <div class="stat-item">🏁 <span>6 Checkpoint</span></div>
                <div class="stat-item">👥 <span>25 Kumpulan</span></div>
            </div>
        </header>

        <!-- 1. MUKA DEPAN (PANEL URUS SETIA) -->
        <div id="view-home" class="glass-card text-center">
            <h2 style="font-size: 0.85rem; font-weight: 800; color: #64748b; letter-spacing: 0.5px;" class="mb-3">PANEL KAWALAN UTAMA</h2>
            
            <button onclick="showAdminQRView()" class="btn-action btn-primary">
                <span>Papar Kod QR Checkpoint (1-6)</span>
                <span>➔</span>
            </button>

            <button onclick="accessFinishRecorder()" class="btn-action btn-warning">
                <span>Rekod Masa Ketibaan Penamat</span>
                <span>➔</span>
            </button>

            <button onclick="showLeaderboard()" class="btn-action btn-success">
                <span>Live Update Markah & Carta</span>
                <span>➔</span>
            </button>
        </div>

        <!-- 2. PAPARAN CHECKPOINT QR (URUS SETIA - GRID BUTTONS) -->
        <div id="view-admin-qr" class="glass-card text-center hidden">
            <button onclick="showView('view-home')" class="btn-secondary">← Kembali ke Halaman Utama</button>
            <h2 style="font-size: 1rem; font-weight: 800;" class="mb-1">Penjana Kod QR Checkpoint</h2>
            <p style="font-size: 0.72rem; color: #64748b;" class="mb-3">Tekan butang checkpoint di bawah untuk memaparkan Kod QR:</p>

            <!-- Grid Butang Checkpoint -->
            <div class="cp-select-grid">
                <div class="btn-cp-card" onclick="openQRModal(1)">
                    <span class="cp-num">Checkpoint 1</span>
                    <span class="cp-tag">0.5 KM</span>
                </div>
                <div class="btn-cp-card" onclick="openQRModal(2)">
                    <span class="cp-num">Checkpoint 2</span>
                    <span class="cp-tag">1.0 KM</span>
                </div>
                <div class="btn-cp-card" onclick="openQRModal(3)">
                    <span class="cp-num">Checkpoint 3</span>
                    <span class="cp-tag">1.5 KM</span>
                </div>
                <div class="btn-cp-card" onclick="openQRModal(4)">
                    <span class="cp-num">Checkpoint 4</span>
                    <span class="cp-tag">2.0 KM</span>
                </div>
                <div class="btn-cp-card" onclick="openQRModal(5)">
                    <span class="cp-num">Checkpoint 5</span>
                    <span class="cp-tag">2.5 KM</span>
                </div>
                <div class="btn-cp-card" onclick="openQRModal(6)">
                    <span class="cp-num">Checkpoint 6</span>
                    <span class="cp-tag">3.0 KM (Penamat)</span>
                </div>
            </div>
        </div>

        <!-- MODAL POPUP QR CODE -->
        <div id="qr-modal" class="modal-overlay hidden">
            <div class="modal-box">
                <h3 id="qr-modal-title" style="font-weight: 800; font-size: 1.1rem; color: #0f172a;">CHECKPOINT X</h3>
                <p style="font-size: 0.7rem; color: #64748b;" class="mb-3">Imbas Kod QR ini menggunakan peranti untuk menjawab kuiz.</p>
                
                <div style="background: #ffffff; padding: 12px; border-radius: 16px; display: inline-block; border: 2px dashed #38bdf8;" class="mb-3">
                    <img id="qr-modal-img" src="" alt="Kod QR Checkpoint" style="width: 190px; height: 190px; display: block; margin: 0 auto;">
                </div>

                <div class="modal-actions">
                    <button onclick="closeQRModal()" style="background: #e2e8f0; color: #334155;">TUTUP</button>
                </div>
            </div>
        </div>

        <!-- 3. PAPARAN REKOD MASA KETIBAAN -->
        <div id="view-finish-recorder" class="glass-card text-center hidden">
            <button onclick="showView('view-home')" class="btn-secondary">← Kembali ke Halaman Utama</button>
            <h2 style="font-size: 1rem; font-weight: 800;" class="mb-1">Rekod Masa Penamat</h2>
            <p style="font-size: 0.72rem; color: #64748b;" class="mb-3">Tekan nombor kumpulan yang baru tiba di Garisan Penamat:</p>

            <!-- Flash Screen -->
            <div id="finish-flash-screen" class="flash-screen hidden">
                <div id="flash-team-name" style="font-size: 0.8rem;">KUMPULAN X</div>
                <div id="flash-time-val" style="font-size: 1.35rem; font-weight: 800; margin: 2px 0;">00:00:00 AM</div>
                <div style="font-size: 0.7rem;">✔ Masa Ketibaan Berjaya Direkodkan!</div>
            </div>

            <!-- Modal Pengesahan Masa Ketibaan -->
            <div id="confirm-modal" class="modal-overlay hidden">
                <div class="modal-box">
                    <h3 id="modal-team-title" style="font-weight: 800; font-size: 1rem; color: #0f172a;">KUMPULAN XX</h3>
                    <p style="font-size: 0.72rem; color: #64748b;" class="mb-2">Masa ketibaan semasa:</p>
                    <div id="modal-time-display" class="modal-time">00:00:00 AM</div>
                    <p style="font-size: 0.72rem; font-weight: 700; color: #ea580c;" class="mb-3">Adakah anda pasti mahu merekodkan masa ini?</p>
                    <div class="modal-actions">
                        <button onclick="closeConfirmModal()" style="background: #e2e8f0; color: #334155;">BATAL</button>
                        <button onclick="commitFinishTime()" style="background: #f59e0b; color: #ffffff;">PASTI</button>
                    </div>
                </div>
            </div>

            <!-- Grid Kumpulan 1-25 Mobile -->
            <div id="finish-teams-grid" class="grid-teams"></div>
        </div>

        <!-- 4. PAPARAN PESERTA: PILIH KUMPULAN -->
        <div id="view-participant-start" class="glass-card hidden">
            <div id="participant-cp-title" style="background: #fff7ed; color: #c2410c; border: 1px solid #ffedd5; text-align: center; font-weight: 800; padding: 10px; border-radius: 14px; font-size: 0.9rem;" class="mb-3">
                📍 CHECKPOINT X
            </div>
            <h2 style="font-size: 0.9rem; font-weight: 800;" class="mb-2">Sila Pilih Nombor Kumpulan Anda:</h2>
            <select id="select-team">
                <option value="">-- Pilih Nombor Kumpulan --</option>
            </select>
            <button onclick="startParticipantQuiz()" class="btn-action btn-warning" style="justify-content: center; font-size: 0.95rem;">MULA JAWAB KUIZ ➔</button>
        </div>

        <!-- 5. PAPARAN SOALAN KUIZ PESERTA -->
        <div id="view-quiz" class="glass-card hidden">
            <div style="display: flex; justify-content: space-between; align-items: center;" class="mb-2">
                <span id="quiz-team-badge" style="background: #eff6ff; color: #1d4ed8; font-size: 0.72rem; font-weight: 800; padding: 4px 12px; border-radius: 14px;"></span>
                <span id="quiz-cp-badge" style="background: #fff7ed; color: #c2410c; font-size: 0.72rem; font-weight: 800; padding: 4px 12px; border-radius: 14px;"></span>
            </div>

            <div class="quiz-progress">
                <div id="quiz-progress-bar" class="quiz-progress-bar"></div>
            </div>

            <div id="question-number" style="font-size: 0.72rem; font-weight: 800; color: #0284c7;" class="mb-2">Soalan 1 daripada 2</div>
            <h3 id="question-text" style="font-size: 0.9rem; font-weight: 700; line-height: 1.45; color: #0f172a;" class="mb-3"></h3>

            <div id="options-container" class="mb-3"></div>

            <div style="display: flex; justify-content: space-between; margin-top: 10px; gap: 8px;">
                <button id="btn-prev" onclick="prevQuestion()" class="btn-secondary hidden" style="width: auto; margin-bottom:0;">← Sebelum</button>
                <button id="btn-next" onclick="nextQuestion()" class="btn-secondary" style="background: #0284c7; color: #ffffff; width: auto; margin-left: auto; margin-bottom:0; border:none;" disabled>Seterusnya ➔</button>
            </div>
        </div>

        <!-- 6. PAPARAN TAHNIAH / SELESAI -->
        <div id="view-completion" class="glass-card text-center hidden">
            <h2 id="completion-title" style="font-size: 1.35rem; font-weight: 800; color: #0f172a;">🎉 TAHNIAH!</h2>
            <p id="completion-msg" style="font-size: 0.78rem; color: #475569; margin: 8px 0;"></p>
            <div style="background: #fffbeb; border: 2px solid #fde68a; padding: 16px; border-radius: 18px; max-width: 240px; margin: 14px auto;">
                <div style="font-size: 0.68rem; font-weight: 800; color: #92400e;">MARKAH DIPEROLEHI</div>
                <div id="cp-score-display" style="font-size: 2rem; font-weight: 800; color: #d97706; margin: 2px 0;">0 / 20</div>
            </div>
            <p id="completion-subtext" style="font-size: 0.72rem; color: #64748b;">Teruskan perjalanan anda ke Checkpoint seterusnya!</p>
        </div>

        <!-- 7. PAPARAN CARTA MARKAH (MOBILE CARDS & CETAKAN) -->
        <div id="view-leaderboard" class="glass-card hidden">
            <!-- HEADER KHAS UNTUK CETAKAN / PDF -->
            <div class="print-header">
                <h1>Laporan Keputusan Rasmi</h1>
                <h2>INTEGRITY WALK JPN PAHANG 2026</h2>
                <p style="font-size: 0.8rem; margin-top: 4px;">Tarikh Cetakan: <span id="print-date-display"></span></p>
            </div>

            <div style="display: flex; justify-content: space-between; align-items: center;" class="mb-3 no-print">
                <h2 style="font-size: 0.9rem; font-weight: 800; color: #0f172a;">Live Leaderboard</h2>
                <div style="display: flex; gap: 6px;">
                    <button onclick="printPDFReport()" class="btn-secondary" style="width: auto; margin-bottom: 0; padding: 8px 12px; background: #0284c7; color: #ffffff; border: none;">
                        🖨️ PDF
                    </button>
                    <button onclick="exportToCSV()" class="btn-secondary" style="width: auto; margin-bottom: 0; padding: 8px 12px; background: #059669; color: #ffffff; border: none;">
                        📥 CSV
                    </button>
                    <button onclick="showView('view-home')" class="btn-secondary" style="width: auto; margin-bottom: 0; padding: 8px 12px;">
                        Utama
                    </button>
                </div>
            </div>

            <!-- Senarai Kad Kumpulan Terkini -->
            <div id="leaderboard-card-container" class="leaderboard-list"></div>

            <!-- FOOTER KHAS PENGESAHAN TANDATANGAN (PRINT ONLY) -->
            <div class="print-footer">
                <div class="sig-box">
                    <div class="sig-line"></div>
                    <p style="font-size: 0.8rem; font-weight: bold;">Disediakan Oleh</p>
                    <p style="font-size: 0.75rem;">Urus Setia Integrity Walk</p>
                </div>
                <div class="sig-box">
                    <div class="sig-line"></div>
                    <p style="font-size: 0.8rem; font-weight: bold;">Disahkan Oleh</p>
                    <p style="font-size: 0.75rem;">Pengerusi Jawatankuasa</p>
                </div>
            </div>
        </div>
    </div>

    <!-- -------------------------------------------------------------
         3. VANILLA JAVASCRIPT LOGIC
         ------------------------------------------------------------- -->
    <script>
        // --- BANK SOALAN ---
        const masterQuestions = [
            { id: 1, q: "Puan Melati Madu tidak hadir bertugas selama tiga (3) hari tanpa kebenaran dan tanpa sebab munasabah. Apakah interpretasi tatatertib yang tepat?\nI. Tidak hadir tanpa cuti\nII. Boleh dikenakan tindakan tatatertib\nIII. Secara automatik dibuang kerja\nIV. Dimaafkan jika pegawai memaklumkan selepas itu", options: ["I dan II sahaja", "I dan IV sahaja", "I, II dan III sahaja", "I sahaja"], correct: 0 },
            { id: 2, q: "Encik Donald Duck aktif menggunakan media sosial dan sentiasa up to date dengan berita terkini. Beliau selalu 'Like' dan 'Share' hantaran kempen politik seorang calon di Facebook. Apakah tafsiran integriti bagi situasi ini?\nI. Boleh dianggap sebagai penglibatan dalam politik\nII. Melanggar ketetapan neutraliti penjawat awam\nIII. Dibenarkan jika tidak menulis komen\nIV. Boleh dikenakan tindakan tatatertib", options: ["I dan IV sahaja", "II dan III sahaja", "I, II dan IV sahaja", "Semua di atas"], correct: 2 },
            { id: 3, q: "Puan Ranee Mukherjee hadir ke pejabat jam 8.55 pagi dan keluar minum jam 9.30 pagi untuk menikmati teh tarik buih dan Nasi Kambing Mengamuk. Beliau pulang semula jam 10.15 pagi dan menggantikan semula masa tersebut dengan bekerja lebih masa. Apakah tafsiran integriti bagi situasi ini?\nI. Pematuhan waktu bekerja bukan sekadar jumlah jam bekerja, tetapi keberadaan di tempat kerja\nII. Tidak menjadi kesalahan kerana beliau sangat lapar\nIII. Dibenarkan jika produktiviti tetap sama\nIV. Boleh dianggap melanggar peraturan waktu bekerja", options: ["I dan II sahaja", "I dan IV sahaja", "I, III dan IV sahaja", "I sahaja"], correct: 1 },
            { id: 4, q: "Encik Mustar sering memuji penampilan Puan Seri Indah seperti berikut: 'Awak ni kalau senyum memang buat pejabat berseri..'\nPada awalnya Puan Seri Indah hanya tersenyum sopan tetapi mula rasa tidak selesa apabila pujian terlalu kerap dan bernada peribadi. Situasi ini boleh ditafsirkan sebagai:\nI. Pujian berulang boleh menyebabkan rasa tidak selesa dan dikategori gangguan seksual\nII. Niat bukan ukuran, tapi kesan kepada mangsa adalah utama\nIII. Tidak salah kerana sekadar memuji\nIV. Ayat digunakan tidak membawa maksud seksual", options: ["I dan II sahaja", "I, III dan IV sahaja", "I, II dan IV sahaja", "Semua di atas"], correct: 0 },
            { id: 5, q: "Berikut adalah hukuman tatatertib yang boleh dikenakan kepada pegawai yang didapati melanggar tatakelakuan:\nI. Lucut Hak Emolumen\nII. Denda\nIII. Tangguh pergerakan gaji\nIV. Pertukaran\nV. Teguran\nVI. Amaran", options: ["I, II dan III sahaja", "I, II, III dan IV sahaja", "I, II, III dan V sahaja", "I, II, III dan VI sahaja"], correct: 3 },
            { id: 6, q: "Suapan rasuah hanya berbentuk wang tunai sahaja.", options: ["Betul", "Salah"], correct: 1 },
            { id: 7, q: "Sarip Dol mempunyai masalah hutang yang banyak dan telah menjadi pemakan gaji tidak solven tetapi tidak melaporkan masalah itu kepada Ketua Jabatannya kerana ia adalah masalah peribadi. Adakah tindakan Encik Sarip Dol betul atau salah?", options: ["Betul", "Salah"], correct: 1 },
            { id: 8, q: "Seseorang pegawai hanya mengisytiharkan harta miliknya tetapi tidak mengisytiharkan harta yang dimiliki oleh pasangan dan anak-anak beliau. Adakah tindakan Encik Sarip Dol betul atau salah?", options: ["Betul", "Salah"], correct: 1 },
            { id: 9, q: "Secara umumnya kegagalan melaporkan pemberian, janji, penawaran rasuah di bawah Seksyen 25(1) dan (2) boleh dikenakan denda tidak melebihi RM100,000.00 atau penjara tidak melebihi 10 tahun atau kedua-duanya sekali.", options: ["Betul", "Salah"], correct: 0 },
            { id: 10, q: "Peraturan 3A, P.U (A) 395/1993 mewajibkan pegawai untuk mematuhi peraturan berkaitan tatakelakuan. Pelanggaran mana-mana peruntukan boleh menyebabkan pegawai dikenakan tindakan tatatertib.", options: ["Betul", "Salah"], correct: 0 },
            { id: 11, q: "Encik Jebat ingin memohon pertukaran ke negeri kelahirannya atas alasan menjaga ibu bapa yang sakit. Namun, permohonannya belum diluluskan. Beliau kemudian meminta bantuan sahabat lamanya yang merupakan Ahli Parlimen kawasan untuk mengeluarkan surat sokongan bagi 'mempercepatkan proses'. Tindakan Encik Jebat dari sudut integriti adalah:", options: ["Tidak salah kerana hal keluarga mendesak", "Tidak salah kerana tidak melibatkan wang", "Salah kerana membawa pengaruh luar untuk menyokong permohonan", "Dibenarkan"], correct: 2 },
            { id: 12, q: "Jika pegawai gagal mengemukakan Surat Tunjuk Sebab dalam tempoh yang ditetapkan, maka:", options: ["Kes dianggap selesai kerana tiada jawapan", "Pegawai dianggap tidak bersalah", "Prosiding boleh dimulakan terhadap pegawai", "Surat baharu perlu dikeluarkan"], correct: 2 },
            { id: 13, q: "Hadir ke pejabat tetapi tidak melaksanakan tugas dengan sengaja atau malas boleh ditafsirkan sebagai:", options: ["Tidak berdisiplin", "Tidak pandai mengurus masa", "Kurang berusaha", "Kecuaian"], correct: 2 },
            { id: 14, q: "Seseorang pegawai yang disabitkan dengan kesalahan rasuah boleh dikenakan tindakan berikut KECUALI:", options: ["Dikenakan tindakan tatatertib", "Dikenakan tindakan di bawah Akta SPRM", "Diberikan teguran atau amaran bertulis oleh Ketua Jabatan", "Ditukarkan jabatan"], correct: 2 },
            { id: 15, q: "Pengisytiharan harta hendaklah dibuat dalam keadaan berikut KECUALI:", options: ["Sekali dalam tempoh lima (5) tahun", "Lantikan pertama", "Bila-bila masa yang dikehendaki oleh Kerajaan", "Setiap kali bertukar Jabatan atau tempat bertugas"], correct: 3 }
        ];

        // --- PEMBOLEH UBAH GLOBAL ---
        let currentTeam = null;
        let currentCP = "1";
        let currentQIndex = 0;
        let userAnswers = [-1, -1];
        let currentActiveQuestions = [];
        let pendingTeamId = null;
        let pendingTimeStr = "";

        // Navigation
        function showView(viewId) {
            const views = ['view-home', 'view-admin-qr', 'view-finish-recorder', 'view-participant-start', 'view-quiz', 'view-completion', 'view-leaderboard'];
            views.forEach(v => document.getElementById(v).classList.add('hidden'));
            document.getElementById(viewId).classList.remove('hidden');
        }

        function showAdminQRView() {
            showView('view-admin-qr');
        }

        // Modal QR Functions
        function openQRModal(cpNum) {
            const baseUrl = window.location.href.split('?')[0];
            const targetUrl = `${baseUrl}?cp=${cpNum}`;
            
            document.getElementById('qr-modal-title').innerText = `CHECKPOINT ${cpNum}`;
            document.getElementById('qr-modal-img').src = `https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=${encodeURIComponent(targetUrl)}`;
            document.getElementById('qr-modal').classList.remove('hidden');
        }

        function closeQRModal() {
            document.getElementById('qr-modal').classList.add('hidden');
        }

        // Populate Options & Grid
        const selectTeam = document.getElementById('select-team');
        const finishTeamsGrid = document.getElementById('finish-teams-grid');

        for(let i=1; i<=25; i++) {
            const opt = document.createElement('option');
            opt.value = i;
            opt.textContent = `KUMPULAN ${i}`;
            selectTeam.appendChild(opt);

            const btn = document.createElement('button');
            btn.className = "btn-team-square";
            btn.innerHTML = `<span style="font-size:0.5rem; opacity:0.8;">KMP</span><span style="font-size:1rem;">${i}</span>`;
            btn.onclick = () => openConfirmModal(i);
            finishTeamsGrid.appendChild(btn);
        }

        // AUTO-DETECT SCAN QR PARAMETER (DIRECT TO PARTICIPANT START)
        window.onload = () => {
            const urlParams = new URLSearchParams(window.location.search);
            const cpParam = urlParams.get('cp');
            if (cpParam) {
                currentCP = cpParam;
                showView('view-participant-start');
                document.getElementById('participant-cp-title').innerText = `📍 CHECKPOINT ${currentCP}`;
            }
        };

        // Masa Ketibaan
        function accessFinishRecorder() {
            const pass = prompt("Sila masukkan kata laluan Urus Setia untuk Masa Ketibaan:");
            if (pass === "2022") {
                showView('view-finish-recorder');
            } else if (pass !== null) {
                alert("Kata laluan salah!");
            }
        }

        function getCurrentTimeFormatted() {
            const now = new Date();
            let hours = now.getHours();
            const minutes = String(now.getMinutes()).padStart(2, '0');
            const seconds = String(now.getSeconds()).padStart(2, '0');
            const ampm = hours >= 12 ? 'PM' : 'AM';
            hours = hours % 12 || 12;
            return `${String(hours).padStart(2, '0')}:${minutes}:${seconds} ${ampm}`;
        }

        function openConfirmModal(teamId) {
            pendingTeamId = teamId;
            pendingTimeStr = getCurrentTimeFormatted();

            document.getElementById('modal-team-title').innerText = `KUMPULAN ${teamId}`;
            document.getElementById('modal-time-display').innerText = pendingTimeStr;
            document.getElementById('confirm-modal').classList.remove('hidden');
        }

        function closeConfirmModal() {
            document.getElementById('confirm-modal').classList.add('hidden');
            pendingTeamId = null;
            pendingTimeStr = "";
        }

        function commitFinishTime() {
            if(!pendingTeamId) return;

            let appData = JSON.parse(localStorage.getItem('integrity_walk_data')) || {};
            if(!appData[`Team_${pendingTeamId}`]) appData[`Team_${pendingTeamId}`] = {};
            appData[`Team_${pendingTeamId}`].finishTime = pendingTimeStr;
            localStorage.setItem('integrity_walk_data', JSON.stringify(appData));

            document.getElementById('flash-team-name').innerText = `KUMPULAN ${pendingTeamId}`;
            document.getElementById('flash-time-val').innerText = pendingTimeStr;
            document.getElementById('finish-flash-screen').classList.remove('hidden');

            closeConfirmModal();

            setTimeout(() => {
                document.getElementById('finish-flash-screen').classList.add('hidden');
            }, 2000);
        }

        // Logik Kuiz
        function getQuestionsForTeamAndCP(teamId, cpNum) {
            const t = parseInt(teamId) || 1;
            const c = parseInt(cpNum) || 1;
            const hash = (t * 7 + c * 13) % masterQuestions.length;
            return [masterQuestions[hash], masterQuestions[(hash + 5) % masterQuestions.length]];
        }

        function startParticipantQuiz() {
            currentTeam = selectTeam.value;
            if(!currentTeam) { alert("Sila pilih Nombor Kumpulan anda!"); return; }

            let appData = JSON.parse(localStorage.getItem('integrity_walk_data')) || {};
            const teamData = appData[`Team_${currentTeam}`] || {};

            if (teamData[`CP${currentCP}`] !== undefined) {
                showAlreadyCompletedScreen(teamData[`CP${currentCP}`]);
                return;
            }

            currentQIndex = 0;
            userAnswers = [-1, -1];
            currentActiveQuestions = getQuestionsForTeamAndCP(currentTeam, currentCP);

            document.getElementById('quiz-team-badge').innerText = `KUMPULAN ${currentTeam}`;
            document.getElementById('quiz-cp-badge').innerText = `CHECKPOINT ${currentCP}`;

            showView('view-quiz');
            renderQuestion();
        }

        function showAlreadyCompletedScreen(score) {
            document.getElementById('completion-title').innerText = "CHECKPOINT SELESAI!";
            document.getElementById('completion-msg').innerText = `Kumpulan ${currentTeam} telah menghantar jawapan untuk Checkpoint ${currentCP}. Jawapan terkunci.`;
            document.getElementById('cp-score-display').innerText = `${score} / 20`;
            showView('view-completion');
        }

        function renderQuestion() {
            const qData = currentActiveQuestions[currentQIndex];

            document.getElementById('question-number').innerText = `Soalan ${currentQIndex + 1} daripada 2`;
            document.getElementById('question-text').innerText = qData.q;
            document.getElementById('quiz-progress-bar').style.width = `${((currentQIndex + 1) / 2) * 100}%`;

            document.getElementById('btn-prev').classList.toggle('hidden', currentQIndex === 0);
            const btnNext = document.getElementById('btn-next');
            btnNext.disabled = userAnswers[currentQIndex] === -1;
            btnNext.innerText = (currentQIndex === 1) ? 'Hantar Jawapan ➔' : 'Seterusnya ➔';

            const container = document.getElementById('options-container');
            container.innerHTML = '';
            const selectedAns = userAnswers[currentQIndex];

            qData.options.forEach((optText, idx) => {
                const btn = document.createElement('button');
                btn.className = `quiz-option-btn ${selectedAns === idx ? 'selected' : ''}`;
                btn.innerText = `${String.fromCharCode(65 + idx)}. ${optText}`;
                btn.onclick = () => { userAnswers[currentQIndex] = idx; renderQuestion(); };
                container.appendChild(btn);
            });
        }

        function prevQuestion() { if (currentQIndex > 0) { currentQIndex--; renderQuestion(); } }
        function nextQuestion() {
            if (currentQIndex < 1) { currentQIndex++; renderQuestion(); }
            else { finishCheckpoint(); }
        }

        function finishCheckpoint() {
            let cpScore = 0;
            userAnswers.forEach((ans, idx) => {
                if (ans === currentActiveQuestions[idx].correct) cpScore += 10;
            });

            let appData = JSON.parse(localStorage.getItem('integrity_walk_data')) || {};
            if(!appData[`Team_${currentTeam}`]) appData[`Team_${currentTeam}`] = {};
            appData[`Team_${currentTeam}`][`CP${currentCP}`] = cpScore;
            localStorage.setItem('integrity_walk_data', JSON.stringify(appData));

            document.getElementById('completion-title').innerText = "🎉 TAHNIAH!";
            document.getElementById('completion-msg').innerText = `Kumpulan ${currentTeam} telah berjaya menjawab Checkpoint ${currentCP}!`;
            document.getElementById('cp-score-display').innerText = `${cpScore} / 20`;

            showView('view-completion');
        }

        // Leaderboard - Format Kad Mesra Mobile
        function showLeaderboard() {
            showView('view-leaderboard');

            let appData = JSON.parse(localStorage.getItem('integrity_walk_data')) || {};
            const container = document.getElementById('leaderboard-card-container');
            container.innerHTML = '';
            let teamsList = [];

            for (let i = 1; i <= 25; i++) {
                const teamKey = `Team_${i}`;
                const cpData = appData[teamKey] || {};
                const cp1 = cpData.CP1 !== undefined ? cpData.CP1 : '-';
                const cp2 = cpData.CP2 !== undefined ? cpData.CP2 : '-';
                const cp3 = cpData.CP3 !== undefined ? cpData.CP3 : '-';
                const cp4 = cpData.CP4 !== undefined ? cpData.CP4 : '-';
                const cp5 = cpData.CP5 !== undefined ? cpData.CP5 : '-';
                const cp6 = cpData.CP6 !== undefined ? cpData.CP6 : '-';
                const finishTime = cpData.finishTime || '-';

                const total = (typeof cp1 === 'number' ? cp1 : 0) + (typeof cp2 === 'number' ? cp2 : 0) +
                              (typeof cp3 === 'number' ? cp3 : 0) + (typeof cp4 === 'number' ? cp4 : 0) +
                              (typeof cp5 === 'number' ? cp5 : 0) + (typeof cp6 === 'number' ? cp6 : 0);
                
                teamsList.push({ id: i, cp1, cp2, cp3, cp4, cp5, cp6, finishTime, total });
            }

            teamsList.sort((a, b) => b.total - a.total);

            teamsList.forEach((t) => {
                const card = document.createElement('div');
                card.className = "team-card";
                card.innerHTML = `
                    <div class="team-card-header">
                        <span class="team-title">KUMPULAN ${t.id}</span>
                        <span class="team-score-badge">${t.total} / 120 Pts</span>
                    </div>
                    <div class="cp-grid">
                        <div class="cp-item"><span class="cp-label">CP1</span><span>${t.cp1}</span></div>
                        <div class="cp-item"><span class="cp-label">CP2</span><span>${t.cp2}</span></div>
                        <div class="cp-item"><span class="cp-label">CP3</span><span>${t.cp3}</span></div>
                        <div class="cp-item"><span class="cp-label">CP4</span><span>${t.cp4}</span></div>
                        <div class="cp-item"><span class="cp-label">CP5</span><span>${t.cp5}</span></div>
                        <div class="cp-item"><span class="cp-label">CP6</span><span>${t.cp6}</span></div>
                    </div>
                    <div class="team-card-footer">
                        <span>Penamat: <span class="finish-time-text">${t.finishTime}</span></span>
                        <button onclick="editTeamData(${t.id})" class="btn-edit-small">Ubah</button>
                    </div>
                `;
                container.appendChild(card);
            });
        }

        // Edit Admin
        function editTeamData(teamId) {
            const pass = prompt(`Masukkan kata laluan untuk pembetulan Kumpulan ${teamId}:`);
            if (pass !== "2022") {
                alert("Kata laluan salah!");
                return;
            }

            let appData = JSON.parse(localStorage.getItem('integrity_walk_data')) || {};
            const choice = prompt(`Pilihan KUMPULAN ${teamId}:\n1. Kemaskini Markah Checkpoint\n2. Kemaskini/Padam Masa Ketibaan\n3. Buka Semula Kunci Kuiz (Allow Retake)\n4. Padam Data Kumpulan\n\nTaip nombor (1-4):`);

            if (choice === "1") {
                const cpNum = prompt("Nombor Checkpoint (1-6):");
                if (cpNum >= 1 && cpNum <= 6) {
                    const newScore = prompt(`Markah baharu CP${cpNum} (0, 10, 20):`);
                    if (newScore !== null && !isNaN(newScore)) {
                        if(!appData[`Team_${teamId}`]) appData[`Team_${teamId}`] = {};
                        appData[`Team_${teamId}`][`CP${cpNum}`] = parseInt(newScore);
                        localStorage.setItem('integrity_walk_data', JSON.stringify(appData));
                        alert("Markah dikemaskini!");
                        showLeaderboard();
                    }
                }
            } else if (choice === "2") {
                const newTime = prompt(`Masukkan masa ketibaan (contoh: 10:30:15 AM) ATAU biarkan kosong untuk padam:`);
                if(!appData[`Team_${teamId}`]) appData[`Team_${teamId}`] = {};
                if (newTime === "") delete appData[`Team_${teamId}`].finishTime;
                else if (newTime !== null) appData[`Team_${teamId}`].finishTime = newTime;
                localStorage.setItem('integrity_walk_data', JSON.stringify(appData));
                alert("Masa ketibaan dikemaskini!");
                showLeaderboard();
            } else if (choice === "3") {
                const cpNum = prompt("Nombor Checkpoint untuk buka kunci (1-6):");
                if (cpNum >= 1 && cpNum <= 6 && appData[`Team_${teamId}`]) {
                    delete appData[`Team_${teamId}`][`CP${cpNum}`];
                    localStorage.setItem('integrity_walk_data', JSON.stringify(appData));
                    alert(`Kunci CP${cpNum} dibuka.`);
                    showLeaderboard();
                }
            } else if (choice === "4") {
                if (confirm(`Padam KESELURUHAN data Kumpulan ${teamId}?`)) {
                    delete appData[`Team_${teamId}`];
                    localStorage.setItem('integrity_walk_data', JSON.stringify(appData));
                    alert("Data dipadam.");
                    showLeaderboard();
                }
            }
        }

        // --- FUNGSI EKSPORT DATA KE CSV / EXCEL ---
        function exportToCSV() {
            let appData = JSON.parse(localStorage.getItem('integrity_walk_data')) || {};
            let csvContent = "\uFEFFKumpulan,CP1,CP2,CP3,CP4,CP5,CP6,Jumlah Markah,Masa Ketibaan\n";

            for (let i = 1; i <= 25; i++) {
                const teamKey = `Team_${i}`;
                const cpData = appData[teamKey] || {};

                const cp1 = cpData.CP1 !== undefined ? cpData.CP1 : 0;
                const cp2 = cpData.CP2 !== undefined ? cpData.CP2 : 0;
                const cp3 = cpData.CP3 !== undefined ? cpData.CP3 : 0;
                const cp4 = cpData.CP4 !== undefined ? cpData.CP4 : 0;
                const cp5 = cpData.CP5 !== undefined ? cpData.CP5 : 0;
                const cp6 = cpData.CP6 !== undefined ? cpData.CP6 : 0;
                const finishTime = cpData.finishTime ? `"${cpData.finishTime}"` : '"-"';

                const total = cp1 + cp2 + cp3 + cp4 + cp5 + cp6;

                const row = [`Kumpulan ${i}`, cp1, cp2, cp3, cp4, cp5, cp6, total, finishTime].join(",");
                csvContent += row + "\n";
            }

            const blob = new Blob([csvContent], { type: 'text/csv;charset=utf-8;' });
            const url = URL.createObjectURL(blob);
            const link = document.createElement("a");
            
            const today = new Date().toISOString().slice(0, 10);
            link.setAttribute("href", url);
            link.setAttribute("download", `Keputusan_Integrity_Walk_JPNPahang_${today}.csv`);
            
            document.body.appendChild(link);
            link.click();
            document.body.removeChild(link);
        }

        // --- FUNGSI CETAK LAPORAN PDF RASMI ---
        function printPDFReport() {
            const now = new Date();
            const dateStr = now.toLocaleDateString('ms-MY', { 
                day: 'numeric', 
                month: 'long', 
                year: 'numeric',
                hour: '2-digit',
                minute: '2-digit'
            });
            
            document.getElementById('print-date-display').innerText = dateStr;
            window.print();
        }
    </script>
</body>
</html>
