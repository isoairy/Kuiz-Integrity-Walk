<!DOCTYPE html>
<html lang="ms">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Integrity Walk JPN Pahang - Mobile-Friendly</title>

    <style>
        /* -------------------------------------------------------------
           1. VANILLA CSS STYLES (MOBILE-FIRST REKA BENTUK)
           ------------------------------------------------------------- */
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap');

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Poppins', sans-serif;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 50%, #0284c7 100%);
            min-height: 100vh;
            padding: 10px;
            color: #1f2937;
        }

        .container {
            max-width: 500px;
            margin: 0 auto;
        }

        /* Glassmorphism Card */
        .glass-card {
            background: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(12px);
            border-radius: 1.25rem;
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.3);
            padding: 18px;
            margin-bottom: 16px;
        }

        /* Header */
        header {
            text-align: center;
            border-bottom: 3px solid #f59e0b;
            padding-bottom: 10px;
        }

        header h1 {
            font-size: 1.15rem;
            font-weight: 800;
            color: #1e1b4b;
            line-height: 1.2;
        }

        header h1 span {
            color: #f59e0b;
        }

        header p {
            font-size: 0.7rem;
            font-weight: 600;
            color: #4b5563;
            margin-top: 3px;
        }

        /* Menu Buttons */
        .btn-menu {
            width: 100%;
            border: none;
            border-radius: 0.85rem;
            padding: 14px 16px;
            margin-bottom: 10px;
            font-weight: 700;
            font-size: 0.85rem;
            color: #ffffff;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            transition: transform 0.1s, background-color 0.2s;
        }

        .btn-menu:active {
            transform: scale(0.97);
        }

        .btn-blue { background-color: #1e3a8a; }
        .btn-blue:active { background-color: #172554; }

        .btn-amber { background-color: #f59e0b; }
        .btn-amber:active { background-color: #d97706; }

        .btn-emerald { background-color: #059669; }
        .btn-emerald:active { background-color: #047857; }

        .btn-gray { 
            background-color: #e5e7eb; 
            color: #374151; 
            font-weight: 700; 
            padding: 8px 14px; 
            border-radius: 8px; 
            font-size: 0.75rem; 
            border: none; 
            cursor: pointer; 
            width: 100%;
            margin-bottom: 12px;
        }

        /* Helpers */
        .hidden { display: none !important; }
        .text-center { text-align: center; }
        .mb-3 { margin-bottom: 12px; }
        .mb-4 { margin-bottom: 16px; }

        /* Select Input Mobile Friendly */
        select {
            width: 100%;
            padding: 12px;
            border-radius: 10px;
            border: 2px solid #60a5fa;
            font-weight: 700;
            font-size: 0.9rem;
            background-color: #eff6ff;
            text-align: center;
            margin-bottom: 14px;
            outline: none;
        }

        /* Grid Masa Ketibaan Penamat */
        .grid-teams {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 6px;
            max-height: 280px;
            overflow-y: auto;
            padding: 2px;
        }

        .btn-team-grid {
            background-color: #fef3c7;
            color: #78350f;
            font-weight: 800;
            padding: 8px 4px;
            border-radius: 10px;
            border: 1px solid #fde68a;
            cursor: pointer;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        .btn-team-grid:active { background-color: #f59e0b; color: #ffffff; transform: scale(0.93); }

        /* Pop-up Modal Mobile */
        .modal-overlay {
            position: fixed;
            top: 0; left: 0; right: 0; bottom: 0;
            background: rgba(0, 0, 0, 0.65);
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 100;
            padding: 16px;
        }

        .modal-box {
            background: #ffffff;
            border-radius: 16px;
            padding: 20px;
            max-width: 300px;
            width: 100%;
            text-align: center;
            border: 2px solid #f59e0b;
        }

        .modal-time {
            font-size: 1.3rem;
            font-weight: 900;
            color: #1e3a8a;
            background-color: #eff6ff;
            padding: 8px;
            border-radius: 10px;
            margin: 10px 0;
            border: 1px solid #bfdbfe;
        }

        .flex-gap {
            display: flex;
            gap: 8px;
        }

        .flex-gap button {
            flex: 1;
            padding: 10px;
            border-radius: 8px;
            border: none;
            font-weight: 700;
            font-size: 0.75rem;
            cursor: pointer;
        }

        /* Quiz Options */
        .quiz-option-btn {
            width: 100%;
            text-align: left;
            padding: 12px 14px;
            border-radius: 10px;
            border: 1.5px solid #cbd5e1;
            background-color: #ffffff;
            font-weight: 600;
            font-size: 0.8rem;
            margin-bottom: 8px;
            cursor: pointer;
            line-height: 1.3;
        }

        .quiz-option-btn.selected { 
            background-color: #dbeafe; 
            border-color: #2563eb; 
            color: #1e40af; 
            font-weight: 700; 
        }

        /* Table Style Mobile Horizontal Scroll */
        .table-responsive {
            overflow-x: auto;
            -webkit-overflow-scrolling: touch;
            border-radius: 8px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            font-size: 0.7rem;
            text-align: center;
            white-space: nowrap;
        }

        th {
            background-color: #0f172a;
            color: #ffffff;
            padding: 8px 6px;
        }

        td {
            padding: 8px 6px;
            border-bottom: 1px solid #e2e8f0;
            font-weight: 600;
        }

        .bg-total { background-color: #fef3c7; color: #d97706; font-weight: 900; }
        .bg-time { background-color: #ecfdf5; color: #047857; font-weight: 700; }

        .flash-screen {
            background-color: #d1fae5;
            border: 1.5px solid #34d399;
            color: #065f46;
            padding: 10px;
            border-radius: 10px;
            font-weight: 700;
            margin-bottom: 12px;
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- HEADER UTAMA -->
        <header class="glass-card">
            <h1>INTEGRITY WALK <span>JPN PAHANG</span></h1>
            <p>Sistem Kuiz Checkpoint & Masa Ketibaan</p>
        </header>

        <!-- 1. MUKA DEPAN (PANEL URUS SETIA) -->
        <div id="view-home" class="glass-card text-center">
            <h2 style="font-size: 0.95rem; font-weight: 800; color: #374151;" class="mb-3">PANEL KAWALAN URUS SETIA</h2>
            
            <button onclick="showAdminQRView()" class="btn-menu btn-blue">
                <span>CHECKPOINT QR (1-6)</span>
                <span>➔</span>
            </button>

            <button onclick="accessFinishRecorder()" class="btn-menu btn-amber">
                <span>REKOD MASA KETIBAAN</span>
                <span>➔</span>
            </button>

            <button onclick="showLeaderboard()" class="btn-menu btn-emerald">
                <span>LIVE UPDATE MARKAH</span>
                <span>➔</span>
            </button>
        </div>

        <!-- 2. PAPARAN CHECKPOINT QR (URUS SETIA) -->
        <div id="view-admin-qr" class="glass-card text-center hidden">
            <button onclick="showView('view-home')" class="btn-gray">← Halaman Utama</button>
            <h2 style="font-size: 0.95rem; font-weight: 800;" class="mb-3">Penjana Kod QR Checkpoint</h2>

            <select id="admin-cp-select" onchange="generateAdminQR()">
                <option value="">-- Sila Pilih Checkpoint --</option>
                <option value="1">Checkpoint 1</option>
                <option value="2">Checkpoint 2</option>
                <option value="3">Checkpoint 3</option>
                <option value="4">Checkpoint 4</option>
                <option value="5">Checkpoint 5</option>
                <option value="6">Checkpoint 6</option>
            </select>

            <div id="qr-box-container" style="background: #ffffff; padding: 12px; border-radius: 14px; display: inline-block; border: 2px dashed #cbd5e1;" class="mb-3 hidden">
                <img id="qr-img-element" src="" alt="Kod QR Checkpoint" style="width: 170px; height: 170px; display: block;">
            </div>
            <p id="qr-instruction-text" style="font-size: 0.7rem; font-weight: 600; color: #6b7280;">Pilih checkpoint di atas untuk memaparkan Kod QR.</p>
        </div>

        <!-- 3. PAPARAN REKOD MASA KETIBAAN -->
        <div id="view-finish-recorder" class="glass-card text-center hidden">
            <button onclick="showView('view-home')" class="btn-gray">← Halaman Utama</button>
            <h2 style="font-size: 0.95rem; font-weight: 800;" class="mb-2">Masa Ketibaan Penamat</h2>
            <p style="font-size: 0.7rem; color: #6b7280;" class="mb-3">Tekan nombor kumpulan yang tiba:</p>

            <!-- Skrin Maklum Balas Auto 2 Saat -->
            <div id="finish-flash-screen" class="flash-screen hidden">
                <div id="flash-team-name" style="font-size: 0.8rem;">KUMPULAN X</div>
                <div id="flash-time-val" style="font-size: 1.2rem; font-weight: 900; margin: 2px 0;">00:00:00 AM</div>
                <div style="font-size: 0.7rem;">✔ Masa Berjaya Direkodkan!</div>
            </div>

            <!-- POP-UP MODAL PENGESAHAN MASA -->
            <div id="confirm-modal" class="modal-overlay hidden">
                <div class="modal-box">
                    <h3 id="modal-team-title" style="font-weight: 800; font-size: 0.9rem;">KUMPULAN XX</h3>
                    <p style="font-size: 0.7rem; color: #6b7280;" class="mt-2">Masa ketibaan semasa:</p>
                    <div id="modal-time-display" class="modal-time">00:00:00 AM</div>
                    <p style="font-size: 0.7rem; font-weight: 700; color: #d97706;" class="mb-3">Adakah anda pasti mahu merekodkan masa ini?</p>
                    <div class="flex-gap">
                        <button onclick="closeConfirmModal()" style="background-color: #e5e7eb; color: #374151;">BATAL</button>
                        <button onclick="commitFinishTime()" style="background-color: #f59e0b; color: #ffffff;">PASTI</button>
                    </div>
                </div>
            </div>

            <!-- Grid Kumpulan 1-25 Mobile -->
            <div id="finish-teams-grid" class="grid-teams"></div>
        </div>

        <!-- 4. PAPARAN PESERTA: PILIH KUMPULAN (DIRECT LANDING VIA QR) -->
        <div id="view-participant-start" class="glass-card hidden">
            <div id="participant-cp-title" style="background-color: #fef3c7; color: #78350f; text-align: center; font-weight: 800; padding: 6px; border-radius: 8px; font-size: 0.8rem;" class="mb-3">
                CHECKPOINT X
            </div>
            <h2 style="font-size: 0.85rem; font-weight: 700;" class="mb-3">Sila Pilih Nombor Kumpulan Anda:</h2>
            <select id="select-team">
                <option value="">-- Pilih Nombor Kumpulan --</option>
            </select>
            <button onclick="startParticipantQuiz()" class="btn-menu btn-amber" style="justify-content: center; font-size: 0.85rem;">MULA JAWAB KUIZ</button>
        </div>

        <!-- 5. PAPARAN SOALAN KUIZ PESERTA -->
        <div id="view-quiz" class="glass-card hidden">
            <div style="display: flex; justify-content: space-between; border-bottom: 1px solid #e5e7eb; padding-bottom: 6px;" class="mb-3">
                <span id="quiz-team-badge" style="background-color: #dbeafe; color: #1e40af; font-size: 0.7rem; font-weight: 800; padding: 3px 10px; border-radius: 12px;"></span>
                <span id="quiz-cp-badge" style="background-color: #fef3c7; color: #78350f; font-size: 0.7rem; font-weight: 800; padding: 3px 10px; border-radius: 12px;"></span>
            </div>

            <div id="question-number" style="font-size: 0.7rem; font-weight: 700; color: #9ca3af;" class="mb-2">Soalan 1 / 2</div>
            <h3 id="question-text" style="font-size: 0.85rem; font-weight: 700; line-height: 1.4; color: #111827;" class="mb-3"></h3>

            <div id="options-container" class="mb-3"></div>

            <div style="display: flex; justify-content: space-between; margin-top: 12px;">
                <button id="btn-prev" onclick="prevQuestion()" class="btn-gray hidden" style="width: auto; margin-bottom:0;">Sebelum</button>
                <button id="btn-next" onclick="nextQuestion()" class="btn-gray" style="background-color: #2563eb; color: #ffffff; width: auto; margin-left: auto; margin-bottom:0;" disabled>Seterusnya</button>
            </div>
        </div>

        <!-- 6. PAPARAN TAHNIAH / SELESAI -->
        <div id="view-completion" class="glass-card text-center hidden">
            <h2 id="completion-title" style="font-size: 1.3rem; font-weight: 900; color: #111827;">TAHNIAH!</h2>
            <p id="completion-msg" style="font-size: 0.75rem; color: #4b5563; margin: 6px 0;"></p>
            <div style="background-color: #fffbeb; border: 1px solid #fde68a; padding: 12px; border-radius: 12px; max-width: 220px; margin: 12px auto;">
                <div style="font-size: 0.7rem; font-weight: 800; color: #92400e;">MARKAH DIPEROLEHI</div>
                <div id="cp-score-display" style="font-size: 1.8rem; font-weight: 900; color: #d97706; margin: 2px 0;">0 / 20</div>
            </div>
            <p id="completion-subtext" style="font-size: 0.7rem; color: #9ca3af;">Markah telah dikemas kini ke Carta Markah Utama.</p>
        </div>

        <!-- 7. PAPARAN CARTA MARKAH (LIVE UPDATE) -->
        <div id="view-leaderboard" class="glass-card hidden">
            <div style="display: flex; justify-content: space-between; align-items: center;" class="mb-3">
                <h2 style="font-size: 0.85rem; font-weight: 800;">Carta Markah & Masa</h2>
                <button onclick="showView('view-home')" class="btn-gray" style="width: auto; margin-bottom: 0;">Halaman Utama</button>
            </div>

            <div class="table-responsive">
                <table>
                    <thead>
                        <tr>
                            <th>Kmp</th>
                            <th>CP1</th>
                            <th>CP2</th>
                            <th>CP3</th>
                            <th>CP4</th>
                            <th>CP5</th>
                            <th>CP6</th>
                            <th>Jumlah</th>
                            <th>Penamat</th>
                            <th>Tindakan</th>
                        </tr>
                    </thead>
                    <tbody id="leaderboard-body"></tbody>
                </table>
            </div>
        </div>
    </div>

    <!-- -------------------------------------------------------------
         2. VANILLA JAVASCRIPT LOGIC
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
            document.getElementById('admin-cp-select').value = "";
            document.getElementById('qr-box-container').classList.add('hidden');
            document.getElementById('qr-instruction-text').innerText = "Pilih checkpoint di atas untuk memaparkan Kod QR.";
            showView('view-admin-qr');
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
            btn.className = "btn-team-grid";
            btn.innerHTML = `<span style="font-size:0.55rem;">KMP</span><span style="font-size:0.95rem; font-weight:900;">${i}</span>`;
            btn.onclick = () => openConfirmModal(i);
            finishTeamsGrid.appendChild(btn);
        }

        // AUTO-DETECT SCAN QR PARAMETER (LANGSUNG KE PILIHAN KUMPULAN)
        window.onload = () => {
            const urlParams = new URLSearchParams(window.location.search);
            const cpParam = urlParams.get('cp');
            if (cpParam) {
                currentCP = cpParam;
                showView('view-participant-start');
                document.getElementById('participant-cp-title').innerText = `CHECKPOINT ${currentCP}`;
            }
        };

        // --- PENJANA QR (PENAMBAHABIKAN PAUTAN) ---
        function generateAdminQR() {
            const cp = document.getElementById('admin-cp-select').value;
            const qrBox = document.getElementById('qr-box-container');
            const qrInstruction = document.getElementById('qr-instruction-text');

            if (!cp) {
                qrBox.classList.add('hidden');
                qrInstruction.innerText = "Pilih checkpoint di atas untuk memaparkan Kod QR.";
                return;
            }

            // Memastikan pautan mengandungi pathname asal dan parameter ?cp=X
            const targetUrl = `${window.location.origin}${window.location.pathname}?cp=${cp}`;
            
            const qrImg = document.getElementById('qr-img-element');
            qrImg.src = `https://api.qrserver.com/v1/create-qr-code/?size=180x180&data=${encodeURIComponent(targetUrl)}`;
            
            qrBox.classList.remove('hidden');
            qrInstruction.innerText = `Peserta imbas Kod QR ini untuk Checkpoint ${cp}.`;
        }

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

            document.getElementById('btn-prev').classList.toggle('hidden', currentQIndex === 0);
            const btnNext = document.getElementById('btn-next');
            btnNext.disabled = userAnswers[currentQIndex] === -1;
            btnNext.innerText = (currentQIndex === 1) ? 'Hantar Jawapan' : 'Seterusnya';

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

            document.getElementById('completion-title').innerText = "TAHNIAH!";
            document.getElementById('completion-msg').innerText = `Kumpulan ${currentTeam} telah berjaya menjawab Checkpoint ${currentCP}!`;
            document.getElementById('cp-score-display').innerText = `${cpScore} / 20`;

            showView('view-completion');
        }

        // Leaderboard
        function showLeaderboard() {
            showView('view-leaderboard');

            let appData = JSON.parse(localStorage.getItem('integrity_walk_data')) || {};
            const tbody = document.getElementById('leaderboard-body');
            tbody.innerHTML = '';
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
                const tr = document.createElement('tr');
                tr.innerHTML = `
                    <td style="font-weight:800; color:#1e3a8a;">K${t.id}</td>
                    <td>${t.cp1}</td>
                    <td>${t.cp2}</td>
                    <td>${t.cp3}</td>
                    <td>${t.cp4}</td>
                    <td>${t.cp5}</td>
                    <td>${t.cp6}</td>
                    <td class="bg-total">${t.total}</td>
                    <td class="bg-time">${t.finishTime}</td>
                    <td>
                        <button onclick="editTeamData(${t.id})" class="btn-gray" style="font-size:0.6rem; padding: 4px 8px; margin-bottom:0;">Ubah</button>
                    </td>
                `;
                tbody.appendChild(tr);
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
    </script>
</body>
</html>
