<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <title>Aplikasi Sistem Genitourinaria – MEDSURIA</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta
    name="description"
    content="Aplikasi ringkas dan komprehensif untuk belajar sistem genitourinaria bagi mahasiswa kedokteran."
  />


  <style>
    :root {
      --bg: #050816;
      --bg-soft: #0b1020;
      --accent: #22c55e;
      --accent-soft: rgba(34, 197, 94, 0.12);
      --accent-strong: #16a34a;
      --text: #f9fafb;
      --muted: #9ca3af;
      --border: #1f2933;
      --danger: #f97373;
      --radius-lg: 18px;
      --radius-xl: 26px;
      --shadow-soft: 0 18px 45px rgba(0, 0, 0, 0.45);
      --transition-fast: 0.18s ease-out;
      --transition-med: 0.25s ease-out;
    }


    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }


    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI",
        sans-serif;
      background: radial-gradient(circle at top, #111827 0, #020617 46%, #020617 100%);
      color: var(--text);
      min-height: 100vh;
      padding: 20px 12px 32px;
    }


    .app-shell {
      max-width: 1200px;
      margin: 0 auto;
    }


    .app-header {
      display: flex;
      flex-wrap: wrap;
      gap: 16px;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 18px;
    }


    .brand {
      display: flex;
      align-items: center;
      gap: 12px;
    }


    .brand-logo {
      width: 44px;
      height: 44px;
      border-radius: 999px;
      background: conic-gradient(
        from 180deg,
        #22c55e,
        #0ea5e9,
        #a855f7,
        #22c55e
      );
      padding: 2px;
      box-shadow: 0 0 28px rgba(34, 197, 94, 0.55);
    }


    .brand-logo-inner {
      width: 100%;
      height: 100%;
      border-radius: inherit;
      background: radial-gradient(circle at 20% 20%, #22c55e 0, #020617 45%);
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 800;
      font-size: 1.1rem;
    }


    .brand-text h1 {
      font-size: 1.4rem;
      letter-spacing: 0.03em;
      font-weight: 700;
    }


    .brand-text p {
      font-size: 0.82rem;
      color: var(--muted);
    }


    .install-btn {
      padding: 10px 18px;
      border-radius: 999px;
      border: none;
      cursor: pointer;
      font-size: 0.9rem;
      font-weight: 600;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: linear-gradient(135deg, var(--accent), var(--accent-strong));
      color: #022c22;
      box-shadow: 0 15px 35px rgba(34, 197, 94, 0.45);
      text-decoration: none;
      transition: transform var(--transition-fast), box-shadow var(--transition-fast),
        filter var(--transition-fast);
    }


    .install-btn span.icon {
      font-size: 1.1rem;
    }


    .install-btn:hover {
      transform: translateY(-1px) scale(1.01);
      filter: brightness(1.05);
      box-shadow: 0 20px 45px rgba(34, 197, 94, 0.6);
    }


    .install-btn:active {
      transform: translateY(1px) scale(0.99);
      box-shadow: 0 8px 20px rgba(34, 197, 94, 0.4);
    }


    .grid-main {
      display: grid;
      grid-template-columns: minmax(0, 2.1fr) minmax(0, 2.3fr);
      gap: 18px;
    }


    @media (max-width: 900px) {
      .grid-main {
        grid-template-columns: minmax(0, 1fr);
      }
      body {
        padding-inline: 12px;
      }
      .app-header {
        gap: 10px;
      }
    }


    /* Card umum */
    .card {
      background: radial-gradient(circle at top left, #111827 0, #020617 45%);
      border-radius: var(--radius-xl);
      border: 1px solid var(--border);
      box-shadow: var(--shadow-soft);
      padding: 16px 16px 18px;
      position: relative;
      overflow: hidden;
    }


    .card::before {
      content: "";
      position: absolute;
      inset: 0;
      background: radial-gradient(
          circle at top right,
          rgba(56, 189, 248, 0.14),
          transparent 55%
        ),
        radial-gradient(
          circle at bottom left,
          rgba(34, 197, 94, 0.16),
          transparent 52%
        );
      opacity: 0.7;
      pointer-events: none;
    }


    .card-inner {
      position: relative;
      z-index: 1;
    }


    .card-header {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      margin-bottom: 10px;
      gap: 8px;
    }


    .card-header h2 {
      font-size: 1.05rem;
      letter-spacing: 0.04em;
      text-transform: uppercase;
      color: #e5e7eb;
    }


    .badge {
      padding: 3px 8px;
      border-radius: 999px;
      font-size: 0.7rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      border: 1px solid rgba(148, 163, 184, 0.4);
      color: #cbd5f5;
      background: rgba(15, 23, 42, 0.7);
      backdrop-filter: blur(6px);
    }


    .card p,
    .card li {
      font-size: 0.86rem;
      line-height: 1.6;
      color: #e5e7eb;
    }


    .muted {
      color: var(--muted);
      font-size: 0.82rem;
    }


    .developer-box {
      display: grid;
      grid-template-columns: minmax(0, 1.8fr) minmax(0, 1.5fr);
      gap: 12px;
      margin-top: 10px;
    }


    @media (max-width: 720px) {
      .developer-box {
        grid-template-columns: minmax(0, 1fr);
      }
    }


    .chip-list {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-top: 6px;
    }


    .chip {
      border-radius: 999px;
      border: 1px solid rgba(148, 163, 184, 0.45);
      padding: 2px 9px;
      font-size: 0.76rem;
      color: #cbd5f5;
      background: rgba(15, 23, 42, 0.7);
      backdrop-filter: blur(4px);
      white-space: nowrap;
    }


    .highlight {
      background: linear-gradient(
        120deg,
        rgba(34, 197, 94, 0.12),
        rgba(56, 189, 248, 0.12)
      );
      border-radius: 999px;
      padding: 2px 7px;
      font-weight: 500;
    }


    .definition-block {
      margin-top: 6px;
      padding: 10px 11px;
      border-radius: 16px;
      background: rgba(15, 23, 42, 0.92);
      border: 1px solid rgba(148, 163, 184, 0.45);
    }


    .definition-block h3 {
      font-size: 0.9rem;
      margin-bottom: 4px;
    }


    .definition-block ul {
      margin-left: 18px;
      margin-top: 4px;
    }


    .definition-block li {
      margin-bottom: 2px;
    }


    /* Sidebar / menu */
    .main-layout {
      display: grid;
      grid-template-columns: minmax(0, 1.2fr) minmax(0, 1.8fr);
      gap: 16px;
      margin-top: 8px;
    }


    @media (max-width: 900px) {
      .main-layout {
        grid-template-columns: minmax(0, 1fr);
      }
    }


    .menu {
      border-radius: 20px;
      background: radial-gradient(
        circle at top left,
        rgba(34, 197, 94, 0.12),
        rgba(15, 23, 42, 0.95)
      );
      border: 1px solid rgba(30, 64, 175, 0.7);
      padding: 10px 10px 11px;
      box-shadow: 0 20px 40px rgba(15, 23, 42, 0.85);
    }


    .menu h3 {
      font-size: 0.92rem;
      margin-bottom: 8px;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: #e5e7eb;
    }


    .menu-note {
      font-size: 0.78rem;
      color: var(--muted);
      margin-bottom: 8px;
    }


    .menu-list {
      display: flex;
      flex-direction: column;
      gap: 6px;
    }


    .menu-item {
      border-radius: 999px;
      border: 1px solid rgba(148, 163, 184, 0.55);
      padding: 8px 10px;
      font-size: 0.86rem;
      display: flex;
      align-items: center;
      gap: 8px;
      background: rgba(15, 23, 42, 0.9);
      cursor: pointer;
      transition: background var(--transition-med), transform var(--transition-fast),
        border-color var(--transition-fast), box-shadow var(--transition-fast);
      position: relative;
      overflow: hidden;
    }


    .menu-item::before {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(
        135deg,
        rgba(34, 197, 94, 0.18),
        rgba(59, 130, 246, 0.16)
      );
      opacity: 0;
      pointer-events: none;
      transition: opacity var(--transition-med);
    }


    .menu-item span.icon {
      font-size: 1.05rem;
      flex-shrink: 0;
    }


    .menu-item span.text {
      flex: 1;
      z-index: 1;
    }


    .menu-item span.tag {
      font-size: 0.7rem;
      border-radius: 999px;
      padding: 2px 6px;
      border: 1px solid rgba(148, 163, 184, 0.6);
      color: #cbd5f5;
      z-index: 1;
      white-space: nowrap;
    }


    .menu-item.active {
      border-color: rgba(34, 197, 94, 0.9);
      box-shadow: 0 0 0 1px rgba(34, 197, 94, 0.9),
        0 16px 35px rgba(22, 163, 74, 0.55);
      transform: translateY(-1px);
    }


    .menu-item.active::before {
      opacity: 1;
    }


    .menu-item:hover:not(.active) {
      transform: translateY(-1px);
      background: rgba(17, 24, 39, 0.96);
    }


    .menu-item:active {
      transform: translateY(1px);
      box-shadow: 0 10px 22px rgba(15, 23, 42, 0.85);
    }


    /* Content */
    .content {
      border-radius: 20px;
      background: radial-gradient(
        circle at top,
        rgba(59, 130, 246, 0.22),
        rgba(15, 23, 42, 0.98)
      );
      border: 1px solid rgba(37, 99, 235, 0.85);
      padding: 12px 14px 14px;
      box-shadow: 0 20px 50px rgba(15, 23, 42, 0.9);
      max-height: 72vh;
      overflow: hidden;
      display: flex;
      flex-direction: column;
    }


    .content-header {
      display: flex;
      justify-content: space-between;
      gap: 10px;
      align-items: flex-start;
      margin-bottom: 10px;
    }


    .content-title-group h2 {
      font-size: 1.02rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      margin-bottom: 4px;
      color: #e5e7eb;
    }


    .content-title-group p {
      font-size: 0.8rem;
      color: var(--muted);
    }


    .content-header-right {
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      gap: 6px;
    }


    .content-pill {
      border-radius: 999px;
      padding: 3px 9px;
      font-size: 0.78rem;
      border: 1px solid rgba(59, 130, 246, 0.7);
      color: #bfdbfe;
      background: rgba(15, 23, 42, 0.9);
      max-width: 180px;
      text-align: right;
    }


    .mode-toggle {
      display: inline-flex;
      border-radius: 999px;
      padding: 2px;
      background: rgba(15, 23, 42, 0.95);
      border: 1px solid rgba(148, 163, 184, 0.7);
    }


    .mode-btn {
      border: none;
      background: transparent;
      color: #e5e7eb;
      font-size: 0.78rem;
      padding: 4px 9px;
      border-radius: 999px;
      cursor: pointer;
      transition: background var(--transition-fast), color var(--transition-fast),
        transform var(--transition-fast), box-shadow var(--transition-fast);
      white-space: nowrap;
    }


    .mode-btn.active {
      background: linear-gradient(135deg, var(--accent), var(--accent-strong));
      color: #022c22;
      box-shadow: 0 0 0 1px rgba(22, 163, 74, 0.7),
        0 10px 25px rgba(34, 197, 94, 0.55);
      transform: translateY(-1px);
    }


    .mode-btn:not(.active):hover {
      background: rgba(31, 41, 55, 0.9);
    }


    @media (max-width: 640px) {
      .content-header {
        flex-direction: column;
        align-items: flex-start;
      }
      .content-header-right {
        align-items: flex-start;
      }
      .content-pill {
        text-align: left;
      }
    }


    .content-scroll {
      margin-top: 6px;
      padding-right: 6px;
      overflow-y: auto;
      scrollbar-width: thin;
      scrollbar-color: rgba(148, 163, 184, 0.8) rgba(15, 23, 42, 0.5);
    }


    .content-scroll::-webkit-scrollbar {
      width: 8px;
    }


    .content-scroll::-webkit-scrollbar-track {
      background: rgba(15, 23, 42, 0.5);
    }


    .content-scroll::-webkit-scrollbar-thumb {
      background: rgba(148, 163, 184, 0.9);
      border-radius: 999px;
    }


    .section-block {
      margin-bottom: 14px;
      padding: 10px 11px;
      border-radius: 16px;
      background: rgba(15, 23, 42, 0.96);
      border: 1px solid rgba(55, 65, 81, 0.9);
    }


    .section-block h3 {
      font-size: 0.96rem;
      margin-bottom: 4px;
      color: #e5e7eb;
    }


    .section-block h4 {
      font-size: 0.9rem;
      margin-top: 4px;
      margin-bottom: 3px;
    }


    .section-block p {
      font-size: 0.86rem;
      margin-bottom: 4px;
    }


    .section-block ul {
      margin-left: 18px;
      margin-top: 2px;
      margin-bottom: 4px;
    }


    .section-block li {
      margin-bottom: 2px;
    }


    .section-label {
      font-size: 0.78rem;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      color: var(--muted);
      margin-bottom: 4px;
    }


    .note {
      font-size: 0.8rem;
      color: #facc15;
    }


    .danger-text {
      color: var(--danger);
    }


    .illus-placeholder {
      margin-top: 4px;
      padding: 8px 9px;
      border-radius: 14px;
      border: 1px dashed rgba(148, 163, 184, 0.75);
      background: rgba(15, 23, 42, 0.9);
      font-size: 0.8rem;
      color: var(--muted);
    }


    .illus-placeholder strong {
      color: #e5e7eb;
    }


    /* QUIZ STYLES */
    .quiz-intro {
      margin-bottom: 10px;
      padding: 9px 10px;
      border-radius: 14px;
      background: rgba(15, 23, 42, 0.92);
      border: 1px solid rgba(148, 163, 184, 0.7);
      font-size: 0.82rem;
    }


    .quiz-intro ul {
      margin-left: 18px;
      margin-top: 4px;
    }


    .quiz-main {
      padding: 10px 10px 8px;
      border-radius: 16px;
      background: rgba(15, 23, 42, 0.96);
      border: 1px solid rgba(55, 65, 81, 0.9);
    }


    .quiz-top {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 10px;
      margin-bottom: 8px;
      font-size: 0.8rem;
      color: var(--muted);
    }


    #quiz-progress {
      font-weight: 500;
      color: #e5e7eb;
    }


    .quiz-question {
      font-size: 0.9rem;
      margin-bottom: 8px;
      line-height: 1.5;
    }


    .quiz-topic-tag {
      display: inline-block;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      padding: 2px 6px;
      border-radius: 999px;
      border: 1px solid rgba(148, 163, 184, 0.7);
      background: rgba(15, 23, 42, 0.9);
      color: #bfdbfe;
      margin-right: 6px;
      margin-bottom: 3px;
    }


    .quiz-options {
      display: flex;
      flex-direction: column;
      gap: 6px;
      margin-bottom: 8px;
    }


    .quiz-option {
      border-radius: 12px;
      border: 1px solid rgba(148, 163, 184, 0.7);
      background: rgba(15, 23, 42, 0.96);
      padding: 7px 9px;
      font-size: 0.85rem;
      text-align: left;
      cursor: pointer;
      transition: background var(--transition-fast), border-color var(--transition-fast),
        transform var(--transition-fast), box-shadow var(--transition-fast);
    }


    .quiz-option:hover:not(:disabled) {
      background: rgba(31, 41, 55, 0.95);
      transform: translateY(-1px);
      box-shadow: 0 10px 22px rgba(15, 23, 42, 0.9);
    }


    .quiz-option:disabled {
      cursor: default;
      opacity: 0.95;
    }


    .quiz-option.correct {
      border-color: rgba(34, 197, 94, 0.9);
      background: rgba(22, 163, 74, 0.14);
      box-shadow: 0 0 0 1px rgba(34, 197, 94, 0.8);
    }


    .quiz-option.incorrect {
      border-color: rgba(248, 113, 113, 0.9);
      background: rgba(239, 68, 68, 0.08);
    }


    .quiz-feedback {
      font-size: 0.82rem;
      min-height: 28px;
      margin-bottom: 8px;
    }


    .quiz-feedback-correct {
      color: #4ade80;
      font-weight: 600;
      margin-right: 4px;
    }


    .quiz-feedback-incorrect {
      color: #f97373;
      font-weight: 600;
      margin-right: 4px;
    }


    .quiz-bottom {
      display: flex;
      justify-content: flex-end;
      margin-bottom: 6px;
    }


    .quiz-primary-btn,
    .quiz-secondary-btn {
      border-radius: 999px;
      border: 1px solid rgba(148, 163, 184, 0.8);
      padding: 6px 12px;
      font-size: 0.8rem;
      font-weight: 500;
      cursor: pointer;
      background: rgba(15, 23, 42, 0.95);
      color: #e5e7eb;
      transition: background var(--transition-fast), border-color var(--transition-fast),
        transform var(--transition-fast), box-shadow var(--transition-fast);
    }


    .quiz-primary-btn {
      border-color: rgba(34, 197, 94, 0.85);
      background: linear-gradient(135deg, rgba(34, 197, 94, 0.2), rgba(22, 163, 74, 0.2));
    }


    .quiz-primary-btn:disabled {
      opacity: 0.5;
      cursor: default;
      transform: none;
      box-shadow: none;
    }


    .quiz-primary-btn:not(:disabled):hover {
      background: linear-gradient(135deg, rgba(34, 197, 94, 0.3), rgba(22, 163, 74, 0.3));
      box-shadow: 0 12px 26px rgba(22, 163, 74, 0.5);
      transform: translateY(-1px);
    }


    .quiz-secondary-btn:hover {
      background: rgba(31, 41, 55, 0.98);
      box-shadow: 0 8px 20px rgba(15, 23, 42, 0.9);
      transform: translateY(-1px);
    }


    .quiz-summary {
      font-size: 0.82rem;
      border-top: 1px solid rgba(55, 65, 81, 0.9);
      padding-top: 6px;
      margin-top: 4px;
    }


    .quiz-summary h3 {
      font-size: 0.9rem;
      margin-bottom: 4px;
    }


    .quiz-summary h4 {
      font-size: 0.86rem;
      margin-top: 6px;
      margin-bottom: 3px;
    }


    .quiz-summary ul {
      margin-left: 18px;
      margin-top: 3px;
    }


    .quiz-summary li {
      margin-bottom: 3px;
    }


    /* Footer kecil */
    .footer-note {
      margin-top: 10px;
      font-size: 0.75rem;
      text-align: right;
      color: var(--muted);
    }


    .footer-note span {
      opacity: 0.9;
    }
  </style>
</head>
<body>
  <div class="app-shell">
    <header class="app-header">
      <div class="brand">
        <div class="brand-logo">
          <div class="brand-logo-inner">GU</div>
        </div>
        <div class="brand-text">
          <h1>Sistem Genitourinaria</h1>
          <p>Aplikasi ringkas dan terstruktur untuk mahasiswa kedokteran</p>
        </div>
      </div>


      <!-- Ganti href dengan link deploy / Play Store milikmu -->
      <a
        href="https://medsuria-app.vercel.app"
        class="install-btn"
        target="_blank"
        rel="noopener noreferrer"
      >
        <span class="icon">⬇️</span>
        <span>Install / Buka Versi Web</span>
      </a>
    </header>


    <main class="grid-main">
      <!-- KARTU KIRI: Perkenalan & Definisi -->
      <section class="card">
        <div class="card-inner">
          <div class="card-header">
            <div>
              <h2>Perkenalan Developer</h2>
              <p class="muted">
                Profil singkat pembuat aplikasi & gambaran tujuan pembelajaran.
              </p>
            </div>
            <span class="badge">About</span>
          </div>


          <div class="developer-box">
            <div>
              <p>
                Aplikasi ini dikembangkan oleh
                <span class="highlight">[Nama Developer / Tim]</span>,
                dengan latar belakang minat pada pendidikan kedokteran dan
                pengembangan media belajar interaktif untuk
                <strong>mahasiswa profesi & preklinik</strong>.
              </p>
              <p class="muted" style="margin-top: 6px">
                Tujuan aplikasi ini adalah membantu mahasiswa memahami konsep
                dasar hingga pemeriksaan fisik dan penunjang sistem
                genitourinaria secara sistematis, singkat, dan mudah diakses
                melalui perangkat apa pun.
              </p>
              <div class="chip-list">
                <span class="chip">FOCUS: Sistem Genitourinaria</span>
                <span class="chip">Target: Mahasiswa Kedokteran</span>
                <span class="chip">Konten: Anatomi & Pemeriksaan</span>
              </div>
            </div>
            <div>
              <div class="definition-block">
                <h3>Definisi Sistem Genitourinaria</h3>
                <p>
                  Sistem genitourinaria adalah gabungan sistem
                  <strong>urinaria</strong> (ginjal & saluran kemih) dan sistem
                  <strong>reproduksi</strong> (pria & wanita) yang memiliki
                  fungsi:
                </p>
                <ul>
                  <li>Filtrasi darah & pembentukan urin</li>
                  <li>Regulasi cairan, elektrolit, dan asam-basa</li>
                  <li>Ekskresi produk sisa metabolisme</li>
                  <li>Fungsi endokrin (misalnya renin, eritropoietin)</li>
                  <li>Fungsi reproduksi, fertilitas, dan seksual</li>
                </ul>
              </div>
            </div>
          </div>


          <p class="muted" style="margin-top: 8px">
            Catatan: Materi di sini bersifat <strong>referensi edukatif</strong>,
            bukan pengganti penilaian klinis maupun pedoman resmi rumah sakit /
            fakultas.
          </p>
        </div>
      </section>


      <!-- KARTU KANAN: Menu + konten -->
      <section class="card">
        <div class="card-inner">
          <div class="card-header">
            <div>
              <h2>Navigator Materi</h2>
              <p class="muted">
                Pilih topik di samping untuk menampilkan penjelasan detail atau masuk ke mode ujian.
              </p>
            </div>
            <span class="badge">Study & Exam</span>
          </div>


          <div class="main-layout">
            <!-- Menu -->
            <aside class="menu">
              <h3>Daftar Topik</h3>
              <p class="menu-note">
                Klik salah satu judul untuk membuka materi:
                <strong>anatomi, pemeriksaan fisik, dan penunjang</strong>.
              </p>


              <div class="menu-list">
                <button
                  class="menu-item active"
                  data-section="anatomi"
                  type="button"
                >
                  <span class="icon">🧬</span>
                  <span class="text">Anatomi Sistem Genitourinaria</span>
                  <span class="tag">Dasar</span>
                </button>


                <button
                  class="menu-item"
                  data-section="ginjal-abdomen"
                  type="button"
                >
                  <span class="icon">🩺</span>
                  <span class="text">Pemeriksaan Ginjal & Abdomen</span>
                  <span class="tag">Fisik</span>
                </button>


                <button
                  class="menu-item"
                  data-section="genital-pria"
                  type="button"
                >
                  <span class="icon">♂️</span>
                  <span class="text">Pemeriksaan Genitalia Pria</span>
                  <span class="tag">Fisik</span>
                </button>


                <button
                  class="menu-item"
                  data-section="prostat"
                  type="button"
                >
                  <span class="icon">📏</span>
                  <span class="text">Pemeriksaan Prostat (DRE)</span>
                  <span class="tag">Fisik</span>
                </button>


                <button
                  class="menu-item"
                  data-section="genital-wanita"
                  type="button"
                >
                  <span class="icon">♀️</span>
                  <span class="text">Pemeriksaan Genitalia Wanita Dasar</span>
                  <span class="tag">Fisik</span>
                </button>


                <button
                  class="menu-item"
                  data-section="penunjang"
                  type="button"
                >
                  <span class="icon">🧪</span>
                  <span class="text">Pemeriksaan Penunjang</span>
                  <span class="tag">Lab & Imaging</span>
                </button>
              </div>
            </aside>


            <!-- Konten -->
            <section class="content">
              <div class="content-header">
                <div class="content-title-group">
                  <h2 id="content-title">Anatomi Sistem Genitourinaria</h2>
                  <p id="content-subtitle">
                    Gambaran struktur utama ginjal, saluran kemih, dan organ
                    reproduksi pria &amp; wanita.
                  </p>
                </div>
                <div class="content-header-right">
                  <div class="content-pill" id="content-pill">
                    Fokus: Anatomi &amp; Orientasi
                  </div>
                  <div class="mode-toggle">
                    <button
                      type="button"
                      class="mode-btn active"
                      data-mode="materi"
                    >
                      Materi
                    </button>
                    <button
                      type="button"
                      class="mode-btn"
                      data-mode="quiz"
                    >
                      Mode Ujian (MCQ)
                    </button>
                  </div>
                </div>
              </div>


              <div class="content-scroll" id="content-body">
                <!-- konten akan diisi lewat JavaScript -->
              </div>
            </section>
          </div>


          <div class="footer-note">
            <span>v1.0 • Sistem Genitourinaria • Edukasi Mahasiswa</span>
          </div>
        </div>
      </section>
    </main>
  </div>


  <script>
    // ===========================
    // DATA KONTEN MATERI
    // ===========================
    const sections = {
      anatomi: {
        title: "Anatomi Sistem Genitourinaria",
        subtitle:
          "Ringkasan struktur anatomi utama ginjal, saluran kemih, dan organ reproduksi.",
        pill: "Fokus: Anatomi & Orientasi",
        html: `
          <div class="section-block">
            <div class="section-label">Ringkasan</div>
            <h3>Komponen Utama Sistem Genitourinaria</h3>
            <p>
              Sistem genitourinaria terdiri atas:
            </p>
            <ul>
              <li><strong>Sistem urinaria</strong>: ginjal, ureter, vesika urinaria, uretra</li>
              <li><strong>Sistem reproduksi pria</strong>: testis, epididimis, vas deferens, vesikula seminalis, kelenjar prostat, penis</li>
              <li><strong>Sistem reproduksi wanita</strong>: ovarium, tuba uterina, uterus, serviks, vagina, vulva</li>
            </ul>
            <div class="illus-placeholder">
              <strong>Ilustrasi anatomi (disarankan):</strong><br />
              Tambahkan gambar skematik:
              <ul>
                <li>Anatomi ginjal &amp; saluran kemih (depan &amp; potongan frontal)</li>
                <li>Organ reproduksi pria (melintang panggul)</li>
                <li>Organ reproduksi wanita (sagital pelvis)</li>
              </ul>
              Ganti kotak ini dengan tag <code>&lt;img src="..." /&gt;</code> sesuai kebutuhan.
            </div>
          </div>


          <div class="section-block">
            <h3>Ginjal (Ren)</h3>
            <p>
              <strong>Lokasi:</strong> Retroperitoneal, setinggi vertebra T12–L3, ginjal kanan biasanya sedikit lebih rendah karena hepar.
            </p>
            <p><strong>Bagian utama:</strong></p>
            <ul>
              <li><strong>Kortex</strong>: tempat korpuskulus renalis &amp; tubulus kontortus</li>
              <li><strong>Medula</strong>: piramid medularis, berakhir di papila renalis</li>
              <li><strong>Kaliks minor &amp; mayor</strong>: menampung urin dari papila</li>
              <li><strong>Pelvis renalis</strong>: pelebaran ureter di hilus renalis</li>
              <li><strong>Hilus renalis</strong>: keluar masuknya a. renalis, v. renalis, ureter, limfatik, dan saraf</li>
            </ul>
            <p><strong>Nefron:</strong></p>
            <ul>
              <li>Glomerulus + kapsula Bowman</li>
              <li>Tubulus kontortus proksimal (TKP)</li>
              <li>Lengkung Henle (descendens &amp; ascendens)</li>
              <li>Tubulus kontortus distal (TKD)</li>
              <li>Duktus koligentes</li>
            </ul>
            <p>
              <strong>Fungsi utama:</strong> filtrasi, reabsorpsi, sekresi, konsentrasi urin, dan fungsi endokrin (renin, eritropoietin, aktivasi vitamin D).
            </p>
          </div>


          <div class="section-block">
            <h3>Saluran Kemih: Ureter, Vesika Urinaria, Uretra</h3>
            <h4>Ureter</h4>
            <ul>
              <li>Panjang ± 25–30 cm, retroperitoneal</li>
              <li>Berjalan dari pelvis renalis ke vesika urinaria, melewati garis panggul</li>
              <li>Memiliki beberapa tempat penyempitan fisiologis:
                <ul>
                  <li>Peralihan pelvis renalis–ureter</li>
                  <li>Tempat ureter melintasi panggul/arteri iliaka</li>
                  <li>Masuk ke dinding vesika urinaria</li>
                </ul>
              </li>
            </ul>
            <h4>Vesika Urinaria (Kandung Kemih)</h4>
            <ul>
              <li>Organ berongga dengan dinding otot detrusor</li>
              <li>Bagian penting: apex, corpus, fundus, dan collum</li>
              <li><strong>Trigonum vesikae</strong>: segitiga di dasar kandung kemih (dua orifisium ureter &amp; orifisium uretra internal)</li>
            </ul>
            <h4>Uretra</h4>
            <p><strong>Pria:</strong> panjang ± 18–22 cm, terbagi menjadi:</p>
            <ul>
              <li>Pars prostatika</li>
              <li>Pars membranasea</li>
              <li>Pars spongiosa (penile)</li>
            </ul>
            <p><strong>Wanita:</strong> panjang ± 4 cm, lebih pendek &amp; lurus → predisposisi infeksi saluran kemih.</p>
          </div>


          <div class="section-block">
            <h3>Organ Reproduksi Pria</h3>
            <h4>Testis &amp; Skrotum</h4>
            <ul>
              <li>Testis: produksi spermatozoa &amp; testosteron</li>
              <li>Lapisan skrotum: kulit, dartos, fasia, tunika vaginalis, tunika albuginea</li>
            </ul>
            <h4>Epididimis &amp; Vas Deferens</h4>
            <ul>
              <li>Epididimis: pematangan, penyimpanan awal sperma</li>
              <li>Vas deferens: menyalurkan sperma dari epididimis ke duktus ejakulatorius</li>
            </ul>
            <h4>Vesikula Seminalis &amp; Prostat</h4>
            <ul>
              <li>Vesikula seminalis: menghasilkan cairan kaya fruktosa (nutrisi sperma)</li>
              <li>Prostat: menghasilkan cairan prostat yang bersifat sedikit asam, mengandung PSA</li>
            </ul>
            <h4>Penis</h4>
            <ul>
              <li>Terdiri dari <strong>corpus cavernosum</strong> (2) dan <strong>corpus spongiosum</strong> yang mengelilingi uretra</li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Organ Reproduksi Wanita</h3>
            <h4>Ovarium</h4>
            <ul>
              <li>Tempat maturasi folikel dan ovulasi</li>
              <li>Produksi estrogen &amp; progesteron</li>
            </ul>
            <h4>Tuba Uterina</h4>
            <ul>
              <li>Fimbriated end menangkap oosit</li>
              <li>Lokasi fertilisasi biasanya di ampula</li>
            </ul>
            <h4>Uterus</h4>
            <ul>
              <li>Bagian: fundus, korpus, isthmus, serviks</li>
              <li>Lapisan: endometrium, miometrium, perimetrium</li>
            </ul>
            <h4>Vagina &amp; Vulva</h4>
            <ul>
              <li>Vagina: kanalis fibromuskular dari serviks ke introitus</li>
              <li>Vulva: labia majora, labia minora, klitoris, vestibulum, meatus uretra eksternum</li>
            </ul>
          </div>
        `,
      },


      "ginjal-abdomen": {
        title: "Pemeriksaan Ginjal & Abdomen",
        subtitle:
          "Langkah sistematis pemeriksaan fisik ginjal dan abdomen yang berkaitan dengan sistem urinaria.",
        pill: "Fokus: Inspeksi, Palpasi, Perkusi, Auskultasi",
        html: `
          <div class="section-block">
            <div class="section-label">Prinsip Umum</div>
            <h3>Persiapan Pemeriksaan</h3>
            <ul>
              <li>Perkenalkan diri &amp; jelaskan tujuan pemeriksaan</li>
              <li>Dapatkan <strong>informed consent</strong></li>
              <li>Pastikan privasi &amp; kenyamanan pasien (tirai, selimut)</li>
              <li>Pasien posisi supin di tempat tidur datar, perut terekspos secukupnya</li>
              <li>Tangan hangat, gunakan sarung tangan bila perlu</li>
            </ul>
            <p class="note">
              Urutan pemeriksaan abdomen: <strong>Inspeksi → Auskultasi → Perkusi → Palpasi</strong>.
            </p>
          </div>


          <div class="section-block">
            <h3>Inspeksi Abdomen & Daerah Lumbal</h3>
            <ul>
              <li>Perhatikan bentuk &amp; kontur abdomen (distensi, asimetri)</li>
              <li>Cari bekas luka operasi, fistula, massa yang tampak</li>
              <li>Amati pergerakan pernapasan dan pulsasi abnormal</li>
              <li>Inspeksi area lumbal:
                <ul>
                  <li>Asimetri (pembesaran ginjal, massa)</li>
                  <li>Perubahan warna kulit, bekas pembedahan</li>
                </ul>
              </li>
            </ul>
          </div>


          <div class="section-block">
            <h3>AusKultasi</h3>
            <p>
              Dilakukan sebelum perkusi &amp; palpasi untuk menilai:
            </p>
            <ul>
              <li><strong>Bising usus</strong>: hiperaktif, hipoaktif, atau tidak terdengar</li>
              <li><strong>Bruit arteri renalis</strong>:
                <ul>
                  <li>Tempatkan stetoskop di garis midklavikula ± 2–3 cm di atas umbilikus</li>
                  <li>Dengarkan kemungkinan bruit (mengi) → dapat mengarah ke stenosis arteri renalis</li>
                </ul>
              </li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Perkusi</h3>
            <h4>1. Perkusi Abdomen Umum</h4>
            <ul>
              <li>Menilai timpani vs pekak:
                <ul>
                  <li>Timpani: gas usus</li>
                  <li>Pekak: organ padat, massa, feses, atau cairan</li>
                </ul>
              </li>
            </ul>
            <h4>2. Perkusi Di Atas Ginjal</h4>
            <ul>
              <li>Perkusi lembut di area lumbal untuk menilai nyeri</li>
            </ul>
            <h4>3. <em>Costovertebral Angle (CVA) Tenderness</em> – Tes Ketok Ginjal</h4>
            <ul>
              <li>Pasien duduk atau berdiri, atau miring</li>
              <li>Letakkan telapak tangan non-dominan di CVA (sudut antara iga terakhir dan kolumna vertebralis)</li>
              <li>Dengan tangan dominan, kepalkan dan ketuk punggung tangan non-dominan</li>
              <li>Nyeri tumpul yang signifikan → kemungkinan infeksi/ inflamasi ginjal (misalnya pielonefritis)</li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Palpasi Ginjal</h3>
            <p>
              Ginjal normal sering <strong>tidak teraba</strong>, kecuali pada individu kurus atau anak.
            </p>
            <h4>Teknik Bimanual (Ginjal Kanan)</h4>
            <ul>
              <li>Pasien supin, lutut sedikit fleksi untuk relaksasi abdomen</li>
              <li>Tangan kiri ditempatkan di daerah lumbal kanan (mengangkat ginjal ke anterior)</li>
              <li>Tangan kanan di kuadran kanan atas abdomen, di bawah arkus kosta</li>
              <li>Minta pasien inspirasi dalam → dorong tangan kiri ke depan, tangan kanan ke posterior-inferior</li>
              <li>Rasakan apakah ada massa yang “terjepit” di antara kedua tangan (ginjal membesar)</li>
            </ul>
            <h4>Hal yang Dinilai</h4>
            <ul>
              <li>Ukuran &amp; batas (reguler vs tidak)</li>
              <li>Konsistensi (lunak, kistik, padat)</li>
              <li>Permukaan (rata vs noduler)</li>
              <li>Mobilitas dengan pernapasan</li>
              <li>Nyeri tekan</li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Penilaian Edema & Tanda Sistemik</h3>
            <ul>
              <li><strong>Edema perifer</strong>:
                <ul>
                  <li>Tekan tungkai bawah/dorsum pedis selama 5 detik</li>
                  <li>Nilai derajat pitting (1+ sampai 4+)</li>
                </ul>
              </li>
              <li><strong>Edema anasarka</strong> pada sindrom nefrotik / gagal ginjal berat</li>
              <li><strong>Tanda uremia</strong>:
                <ul>
                  <li>Halitosis uremik, kulit kering, pruritus</li>
                  <li>Perubahan status mental (akumulasi toksin uremik)</li>
                </ul>
              </li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Pengukuran Output Urin</h3>
            <ul>
              <li>Catat volume urin/24 jam:
                <ul>
                  <li>Oliguria: &lt; 400 mL/24 jam</li>
                  <li>Anuria: &lt; 100 mL/24 jam</li>
                  <li>Poliuria: &gt; 3 L/24 jam</li>
                </ul>
              </li>
              <li>Perhatikan warna, kejernihan, dan bau urin</li>
              <li>Catat frekuensi dan keluhan (disuria, nokturia, urgensi, hematuria)</li>
            </ul>
            <p class="note">
              Data ini sangat penting untuk mengorelasikan temuan fisik dengan gangguan fungsi ginjal.
            </p>
          </div>
        `,
      },


      "genital-pria": {
        title: "Pemeriksaan Genitalia Pria",
        subtitle:
          "Pemeriksaan sistematis genitalia pria, termasuk penis, skrotum, testis, epididimis, dan hernia inguinal.",
        pill: "Fokus: Inspeksi & Palpasi Terarah",
        html: `
          <div class="section-block">
            <div class="section-label">Prinsip Umum</div>
            <h3>Persiapan & Komunikasi</h3>
            <ul>
              <li>Jelaskan tujuan pemeriksaan dengan bahasa yang jelas dan sensitif</li>
              <li>Pastikan privasi optimal (ruangan tertutup, tirai, minimal petugas)</li>
              <li>Tawarkan keberadaan pendamping (chaperone) bila sesuai kebijakan</li>
              <li>Gunakan sarung tangan, dan jelaskan setiap langkah sebelum dilakukan</li>
            </ul>
            <p class="danger-text">
              Hindari komentar yang tidak profesional. Jaga ekspresi wajah dan bahasa tubuh.
            </p>
          </div>


          <div class="section-block">
            <h3>Pemeriksaan Penis</h3>
            <h4>Inspeksi</h4>
            <ul>
              <li>Perhatikan ukuran, bentuk, dan posisi penis</li>
              <li>Amati kulit: lesi, ulkus, papul, plak, hiperpigmentasi, jaringan parut</li>
              <li>Perhatikan glans: erosi, balanitis, lesi mencurigakan</li>
              <li>Periksa meatus uretra eksternum:
                <ul>
                  <li>Posisi (hipospadia, epispadia)</li>
                  <li>Adanya discharge (uretritis, infeksi menular seksual)</li>
                </ul>
              </li>
            </ul>
            <h4>Palpasi</h4>
            <ul>
              <li>Raba korpus penis:
                <ul>
                  <li>Konsistensi (plak pada penyakit Peyronie)</li>
                  <li>Nyeri tekan atau massa</li>
                </ul>
              </li>
              <li>Bila ada discharge, dapat diambil untuk pemeriksaan mikrobiologi sesuai indikasi</li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Pemeriksaan Skrotum & Testis</h3>
            <h4>Inspeksi Skrotum</h4>
            <ul>
              <li>Simetri skrotum kanan-kiri</li>
              <li>Perubahan kulit (eritem, ulkus, varises, edema)</li>
              <li>Pembesaran skrotum (hidrokel, varikokel, hernia inguinal, tumor testis)</li>
            </ul>
            <h4>Palpasi Testis & Epididimis</h4>
            <ul>
              <li>Posisi pasien berdiri atau supin</li>
              <li>Gunakan kedua tangan:
                <ul>
                  <li>Testis normal: bentuk oval, konsistensi kenyal, permukaan halus</li>
                  <li>Perhatikan:
                    <ul>
                      <li>Nyeri tekan → epididimitis, orkitis, torsi testis</li>
                      <li>Massa keras/ tidak nyeri → curiga tumor testis</li>
                    </ul>
                  </li>
                </ul>
              </li>
              <li>Palpasi epididimis di posterior testis:
                <ul>
                  <li>Nilai pembesaran, nyeri, nodul</li>
                </ul>
              </li>
              <li>Transiluminasi:
                <ul>
                  <li>Sinar senter ke skrotum dalam ruangan gelap</li>
                  <li>Cairan (hidrokel) → transiluminasi positif</li>
                  <li>Massa padat → transiluminasi negatif</li>
                </ul>
              </li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Pemeriksaan Hernia Inguinal</h3>
            <ul>
              <li>Pasien berdiri, minta batuk atau mengejan (manuver Valsalva)</li>
              <li>Inspeksi lipat paha:
                <ul>
                  <li>Adanya benjolan yang muncul saat batuk/mengejan</li>
                </ul>
              </li>
              <li>Palpasi:
                <ul>
                  <li>Masukkan jari ke dalam skrotum dan arahkan ke kanal inguinal</li>
                  <li>Rasakan impulse saat pasien batuk:
                    <ul>
                      <li>Hernia inguinal indirek vs direk (berdasarkan posisi impulse)</li>
                    </ul>
                  </li>
                </ul>
              </li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Pertanyaan Anamnesis Penting</h3>
            <ul>
              <li>Nyeri testis atau skrotum (onset mendadak → curiga torsi testis)</li>
              <li>Keluhan bengkak skrotum (durasi, progresi, nyeri)</li>
              <li>Keluhan buang air kecil (disuria, hematuria, stranguria, aliran lemah)</li>
              <li>Riwayat infeksi menular seksual, trauma, atau pembedahan</li>
              <li>Status fertilitas (lama menikah, anak, riwayat infertilitas)</li>
            </ul>
            <p class="note">
              Temuan ini nantinya dikorelasikan dengan pemeriksaan penunjang (USG skrotum, analisis sperma, dll).
            </p>
          </div>
        `,
      },


      prostat: {
        title: "Pemeriksaan Prostat (DRE)",
        subtitle:
          "Digital rectal examination (DRE) untuk menilai ukuran, konsistensi, dan kelainan prostat.",
        pill: "Fokus: Teknik DRE & Interpretasi Dasar",
        html: `
          <div class="section-block">
            <div class="section-label">Prinsip & Etika</div>
            <h3>Persiapan Pemeriksaan DRE</h3>
            <ul>
              <li>Jelaskan tujuan pemeriksaan dengan bahasa yang jelas &amp; profesional</li>
              <li>Dapatkan <strong>informed consent</strong> tertulis/lisan sesuai kebijakan</li>
              <li>Pastikan privasi maksimal dan gunakan tirai</li>
              <li>Gunakan sarung tangan &amp; pelumas (lubrikan) yang cukup</li>
              <li>Tawarkan pendamping (chaperone) bila sesuai</li>
            </ul>
            <p class="danger-text">
              Pemeriksaan DRE harus dilakukan dengan penuh penghormatan terhadap martabat pasien.
            </p>
          </div>


          <div class="section-block">
            <h3>Posisi Pasien</h3>
            <ul>
              <li><strong>Left lateral (Sim's position)</strong>:
                <ul>
                  <li>Pasien berbaring miring kiri, pinggul fleksi, lutut ditekuk</li>
                </ul>
              </li>
              <li><strong>Litotomi</strong> (sering di ruang operasi/ruang khusus)</li>
              <li><strong>Knee-chest position</strong> (tergantung kebiasaan setempat)</li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Teknik Pemeriksaan</h3>
            <ul>
              <li>Inspeksi regio perianal:
                <ul>
                  <li>Fisura, hemoroid, fistula, massa, eritem</li>
                </ul>
              </li>
              <li>Oleskan pelumas pada jari telunjuk pemeriksa</li>
              <li>Sentuh anus dengan lembut, minta pasien relaks dan bernapas pelan</li>
              <li>Masukkan jari perlahan mengikuti kurva kanal anal</li>
              <li>Nilai <strong>tonus sfingter ani</strong> saat pasien mengontraksikan anus</li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Penilaian Prostat</h3>
            <ul>
              <li>Prostat teraba melalui dinding anterior rektum</li>
              <li><strong>Normal:</strong>
                <ul>
                  <li>Ukuran ± seukuran buah kenari besar</li>
                  <li>Konsistensi padat kenyal</li>
                  <li>Permukaan halus</li>
                  <li>Terdapat sulkus medianus</li>
                </ul>
              </li>
              <li><strong>Benign Prostatic Hyperplasia (BPH):</strong>
                <ul>
                  <li>Prostat membesar, padat kenyal, permukaan halus</li>
                  <li>Sulkus medianus dapat menghilang</li>
                </ul>
              </li>
              <li><strong>Kecurigaan Keganasan:</strong>
                <ul>
                  <li>Konsistensi sangat keras</li>
                  <li>Permukaan noduler / tidak teratur</li>
                  <li>Asimetri lobus</li>
                  <li>Fiksasi ke jaringan sekitar (mobilitas berkurang)</li>
                </ul>
              </li>
              <li><strong>Prostatitis:</strong>
                <ul>
                  <li>Prostat terasa nyeri tekan</li>
                  <li>Konsistensi bisa lebih lunak atau bengkak</li>
                </ul>
              </li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Penilaian Tambahan Saat DRE</h3>
            <ul>
              <li>Feses di rektum (melena, darah segar, massa)</li>
              <li>Lesi lain di rektum (massa, polip, nyeri lokal)</li>
            </ul>
            <p class="note">
              Hasil DRE harus dikorelasikan dengan gejala (LUTS, hematuria, nyeri) dan pemeriksaan penunjang (PSA, USG transrektal, biopsi).
            </p>
          </div>
        `,
      },


      "genital-wanita": {
        title: "Pemeriksaan Genitalia Wanita Dasar",
        subtitle:
          "Langkah pokok pemeriksaan eksternal dan internal genitalia wanita secara edukatif dan sensitif.",
        pill: "Fokus: Privasi, Inspeksi, & Pemeriksaan Bimanual",
        html: `
          <div class="section-block">
            <div class="section-label">Etika & Komunikasi</div>
            <h3>Persiapan Pemeriksaan</h3>
            <ul>
              <li>Jelaskan tujuan pemeriksaan dengan bahasa yang jelas dan empatik</li>
              <li>Dapatkan <strong>informed consent</strong></li>
              <li>Pastikan adanya pendamping (chaperone) sesuai kebijakan</li>
              <li>Gunakan tirai, selimut, dan jaga privasi maksimal</li>
              <li>Gunakan sarung tangan dan pelumas seperlunya</li>
            </ul>
            <p class="danger-text">
              Selalu hormati kenyamanan pasien. Berikan kesempatan pasien bertanya dan menolak.
            </p>
          </div>


          <div class="section-block">
            <h3>Posisi Pasien</h3>
            <ul>
              <li><strong>Litotomi:</strong> pasien terlentang, kaki difleksikan dan ditopang pada leg support/stirrup</li>
              <li>Pastikan hanya area yang diperiksa yang terekspos</li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Inspeksi Eksternal (Vulva)</h3>
            <ul>
              <li>Amati distribusi rambut pubis</li>
              <li>Periksa labia majora &amp; minora:
                <ul>
                  <li>Lesi, ulkus, papul, vesikel (curiga infeksi menular seksual)</li>
                  <li>Status kebersihan, inflamasi, edema</li>
                </ul>
              </li>
              <li>Periksa klitoris dan uretra eksternum:
                <ul>
                  <li>Adanya discharge uretra</li>
                </ul>
              </li>
              <li>Inspeksi introitus vagina:
                <ul>
                  <li>Stenosis, prolaps, lesi, discharge (warna, bau, konsistensi)</li>
                </ul>
              </li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Pemeriksaan dengan Spekulum (Gambaran Dasar)</h3>
            <ul>
              <li>Pilih ukuran spekulum yang sesuai (Cusco/Graves)</li>
              <li>Olesi spekulum dengan pelumas bila diizinkan</li>
              <li>Masukkan spekulum dengan arah miring mengikuti kurva vagina, lalu buka perlahan</li>
              <li>Identifikasi serviks:
                <ul>
                  <li>Bentuk, warna, eversi, erosi</li>
                  <li>Adanya lesi, perdarahan kontak, polip</li>
                  <li>Karakter <strong>discharge serviks</strong></li>
                </ul>
              </li>
            </ul>
            <p class="note">
              Pada prosedur Pap smear, ambil sampel dari ektoserviks dan endoserviks dengan alat yang sesuai.
            </p>
          </div>


          <div class="section-block">
            <h3>Pemeriksaan Bimanual</h3>
            <ul>
              <li>Gunakan 2 jari (telunjuk &amp; tengah) tangan dominan, dengan pelumas</li>
              <li>Jari lain menekan dari suprapubik (tangan non-dominan)</li>
              <li>Nilai:
                <ul>
                  <li><strong>Serviks</strong>: konsistensi, mobilitas, nyeri gerak</li>
                  <li><strong>Uterus</strong>: ukuran, posisi (anteversi/retroversi), mobilitas, nyeri</li>
                  <li><strong>Adneksa (ovarium &amp; tuba)</strong>: pembesaran, massa, nyeri</li>
                </ul>
              </li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Pemeriksaan Rektovaginal (Bila Indikasi)</h3>
            <ul>
              <li>Menilai dinding posterior uterus dan ligamentum uterosakral</li>
              <li>Mendeteksi massa di cul-de-sac (Douglas) dan rektum</li>
            </ul>
            <p class="note">
              Seluruh temuan harus dikorelasikan dengan anamnesis (nyeri panggul, perdarahan abnormal, keputihan) dan pemeriksaan penunjang (USG, Pap smear, kultur).
            </p>
          </div>
        `,
      },


      penunjang: {
        title: "Pemeriksaan Penunjang Sistem Genitourinaria",
        subtitle:
          "Ringkasan pemeriksaan laboratorium dan imaging yang umum digunakan untuk evaluasi sistem urinaria dan reproduksi.",
        pill: "Fokus: Lab, Urinalisis, Imaging",
        html: `
          <div class="section-block">
            <div class="section-label">Lab & Urinalisis</div>
            <h3>Urinalisis Rutin</h3>
            <ul>
              <li><strong>Makroskopik:</strong> warna, kejernihan, bau, volume</li>
              <li><strong>Kimia:</strong>
                <ul>
                  <li>pH, berat jenis</li>
                  <li>Protein, glukosa, keton</li>
                  <li>Bilirubin, urobilinogen</li>
                  <li>Darah/hemoglobin</li>
                  <li>Nitrit &amp; leukocyte esterase (infeksi)</li>
                </ul>
              </li>
              <li><strong>Mikroskopik:</strong>
                <ul>
                  <li>Sel darah merah &amp; sel darah putih</li>
                  <li>Silinder (hialin, granular, eritrosit, leukosit)</li>
                  <li>Kristal (asam urat, oksalat, struvit, dll.)</li>
                  <li>Bakteri, jamur</li>
                </ul>
              </li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Fungsi Ginjal & Elektrolit</h3>
            <ul>
              <li><strong>Serum kreatinin &amp; ureum (BUN):</strong> menggambarkan fungsi filtrasi ginjal</li>
              <li><strong>eGFR:</strong> estimasi laju filtrasi glomerulus</li>
              <li><strong>Elektrolit:</strong> Na, K, Cl, HCO₃⁻ → gangguan pada gagal ginjal akut/kronis</li>
              <li><strong>Gas Darah:</strong> menilai status asam-basa (asidosis metabolik, dll.)</li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Pemeriksaan Imaging</h3>
            <h4>USG Ginjal & Traktus Urinarius</h4>
            <ul>
              <li>Ukuran &amp; kontur ginjal</li>
              <li>Dilatasi sistem pelvikokaliks (hidronefrosis)</li>
              <li>Batu ginjal/ureter (terlihat sebagai echo hiperekoik dengan bayangan)</li>
              <li>Massa ginjal/kandung kemih</li>
            </ul>
            <h4>CT Urografi / CT Abdomen</h4>
            <ul>
              <li>Deteksi batu, massa, trauma ginjal</li>
              <li>Evaluasi tumor traktus urinarius</li>
            </ul>
            <h4>Foto BNO/IVP (Intravenous Pyelography)</h4>
            <ul>
              <li>Menilai fungsi ekskretor ginjal dan anatomi saluran kemih dengan kontras</li>
            </ul>
            <h4>MCU (Micturating Cystourethrography)</h4>
            <ul>
              <li>Evaluasi refluks vesikoureteral</li>
              <li>Kelainan uretra (striktur, divertikel)</li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Pemeriksaan Khusus Sistem Reproduksi Pria</h3>
            <ul>
              <li><strong>Analisis Sperma:</strong>
                <ul>
                  <li>Volume, konsentrasi, motilitas, morfologi</li>
                </ul>
              </li>
              <li><strong>Hormon:</strong> testosteron total/free, LH, FSH, prolaktin</li>
              <li><strong>PSA (Prostate-Specific Antigen):</strong>
                <ul>
                  <li>Meningkat pada BPH, prostatitis, kanker prostat</li>
                  <li>Interpretasi harus hati-hati, lihat pedoman dan usia</li>
                </ul>
              </li>
              <li><strong>USG Transrektal:</strong> menilai prostat, vesikula seminalis</li>
            </ul>
          </div>


          <div class="section-block">
            <h3>Pemeriksaan Khusus Sistem Reproduksi Wanita</h3>
            <ul>
              <li><strong>USG Transvaginal:</strong>
                <ul>
                  <li>Menilai uterus (mioma, adenomyosis), endometrium</li>
                  <li>Ovarium (kista, tumor, PCOS)</li>
                </ul>
              </li>
              <li><strong>USG Transabdominal:</strong> digunakan bila transvaginal tidak mungkin</li>
              <li><strong>Pap Smear / Sitologi Serviks:</strong> skrining lesi prakanker serviks</li>
              <li><strong>Hormon:</strong> FSH, LH, estradiol, progesteron, prolaktin, AMH (sesuai indikasi)</li>
            </ul>
            <p class="note">
              Pilihan pemeriksaan penunjang harus disesuaikan dengan gejala klinis, usia, dan faktor risiko setiap pasien.
            </p>
          </div>
        `,
      },
    };


    // ===========================
    // DATA SOAL UJIAN (FULL EXAM)
    // ===========================
    const examQuestions = [
      {
        topic: "Anatomi",
        question: "Secara anatomis, ginjal biasanya terletak pada level vertebra:",
        options: [
          "T6–T9",
          "T9–T12",
          "T12–L3",
          "L3–L5"
        ],
        answerIndex: 2,
        explanation:
          "Ginjal terletak retroperitoneal setinggi T12–L3. Ginjal kanan sedikit lebih rendah karena tekanan dari hepar."
      },
      {
        topic: "Anatomi",
        question: "Komponen utama korpuskulus renalis tersusun atas:",
        options: [
          "Lengkung Henle dan duktus koligentes",
          "Glomerulus dan kapsula Bowman",
          "Tubulus kontortus proksimal dan distal",
          "Kaliks minor dan pelvis renalis"
        ],
        answerIndex: 1,
        explanation:
          "Korpuskulus renalis terdiri dari glomerulus yang dikelilingi oleh kapsula Bowman dan menjadi tempat awal filtrasi."
      },
      {
        topic: "Anatomi",
        question: "Trigonum vesikae pada kandung kemih dibentuk oleh:",
        options: [
          "Dua ostium uretra dan satu ostium ureter",
          "Dua ostium ureter dan satu ostium uretra internal",
          "Satu ostium ureter dan satu ostium uretra eksternum",
          "Dua ostium uretra eksternum"
        ],
        answerIndex: 1,
        explanation:
          "Trigonum vesikae adalah area segitiga yang dibentuk oleh dua orifisium ureter di atas dan satu orifisium uretra internal di bawah."
      },
      {
        topic: "Anatomi",
        question: "Penyempitan fisiologis ureter secara klasik dijumpai pada lokasi berikut, KECUALI:",
        options: [
          "Peralihan pelvis renalis ke ureter",
          "Saat melintasi panggul/arteri iliaka",
          "Masuk ke dinding vesika urinaria",
          "Saat melintasi diafragma torakalis"
        ],
        answerIndex: 3,
        explanation:
          "Ureter menyempit secara fisiologis di tiga lokasi: pelvi-ureteric junction, crossing pelvic brim/arteri iliaka, dan vesico-ureteric junction."
      },
      {
        topic: "Anatomi",
        question: "Perbedaan utama anatomi uretra pria dan wanita yang relevan secara klinis adalah:",
        options: [
          "Uretra pria lebih pendek sehingga lebih mudah infeksi",
          "Uretra wanita lebih panjang sehingga lebih mudah sumbatan",
          "Uretra pria lebih panjang dan juga berfungsi sebagai saluran reproduksi",
          "Uretra wanita berfungsi ganda sebagai saluran reproduksi"
        ],
        answerIndex: 2,
        explanation:
          "Uretra pria panjang (±18–22 cm) dan berfungsi untuk aliran urin serta ejakulasi. Uretra wanita lebih pendek (±4 cm) dan hanya sebagai saluran urin."
      },
      {
        topic: "Anatomi",
        question: "Fungsi utama aparatus jukstaglomerulus adalah:",
        options: [
          "Memproduksi eritrosit secara langsung",
          "Mengatur tekanan darah dan laju filtrasi glomerulus",
          "Meningkatkan reabsorpsi glukosa di ginjal",
          "Mensekresikan hormon insulin"
        ],
        answerIndex: 1,
        explanation:
          "Aparatus jukstaglomerulus berperan dalam regulasi tekanan darah dan GFR melalui sekresi renin dan mekanisme feedback tubuloglomerular."
      },
      {
        topic: "Pemeriksaan Ginjal & Abdomen",
        question: "Urutan pemeriksaan fisik abdomen yang benar adalah:",
        options: [
          "Inspeksi – Perkusi – Palpasi – Auskultasi",
          "Auskultasi – Inspeksi – Palpasi – Perkusi",
          "Inspeksi – Auskultasi – Perkusi – Palpasi",
          "Palpasi – Inspeksi – Perkusi – Auskultasi"
        ],
        answerIndex: 2,
        explanation:
          "Urutan yang dianjurkan adalah inspeksi terlebih dahulu, diikuti auskultasi, kemudian perkusi, dan terakhir palpasi."
      },
      {
        topic: "Pemeriksaan Ginjal & Abdomen",
        question: "Nyeri tekan pada tes ketok ginjal di costovertebral angle (CVA tenderness) paling sering mengarah pada:",
        options: [
          "Gastritis",
          "Pielonefritis",
          "Apendisitis akut",
          "Pankreatitis"
        ],
        answerIndex: 1,
        explanation:
          "Nyeri pada CVA tenderness biasanya menunjukkan proses inflamasi pada ginjal, seperti pielonefritis."
      },
      {
        topic: "Pemeriksaan Ginjal & Abdomen",
        question: "Definisi oliguria yang sering dipakai dalam praktik klinis adalah produksi urin:",
        options: [
          "Kurang dari 3 liter per hari",
          "Kurang dari 1 liter per hari",
          "Kurang dari 400 mL per hari",
          "Kurang dari 100 mL per hari"
        ],
        answerIndex: 2,
        explanation:
          "Oliguria adalah produksi urin kurang dari 400 mL per hari. Di bawah 100 mL per hari biasanya didefinisikan sebagai anuria."
      },
      {
        topic: "Pemeriksaan Ginjal & Abdomen",
        question: "Posisi yang paling tepat untuk palpasi ginjal kanan secara bimanual adalah:",
        options: [
          "Pasien duduk, tungkai menjuntai",
          "Pasien supin dengan lutut sedikit fleksi",
          "Pasien berdiri tegak",
          "Pasien dalam posisi litotomi"
        ],
        answerIndex: 1,
        explanation:
          "Palpasi ginjal dilakukan saat pasien berbaring supin dengan lutut sedikit fleksi agar otot dinding perut lebih relaks."
      },
      {
        topic: "Pemeriksaan Ginjal & Abdomen",
        question: "Edema pitting pada tungkai bawah yang disertai hipoalbuminemia dan proteinuria berat paling khas ditemukan pada:",
        options: [
          "Sindrom nefrotik",
          "Apendisitis akut",
          "Penyakit refluks vesikoureteral",
          "Pielonefritis akut tanpa komplikasi"
        ],
        answerIndex: 0,
        explanation:
          "Sindrom nefrotik ditandai proteinuria masif, hipoalbuminemia, hiperkoagulabilitas, dan edema generalisata dengan pitting."
      },
      {
        topic: "Genitalia Pria",
        question: "Massa skrotum yang membesar dan memberikan transiluminasi positif paling mungkin merupakan:",
        options: [
          "Hernia inguinalis strangulata",
          "Tumor testis",
          "Hidrokel",
          "Varikokel"
        ],
        answerIndex: 2,
        explanation:
          "Hidrokel berisi cairan di sekitar testis sehingga sering memberikan transiluminasi positif saat disinari."
      },
      {
        topic: "Genitalia Pria",
        question: "Temuan klasik tumor testis pada pemeriksaan fisik adalah:",
        options: [
          "Massa lunak nyeri tekan hebat",
          "Massa keras tidak nyeri pada testis",
          "Skrotum merah dan hangat dengan fluktuasi",
          "Skrotum cekung dan atrofi"
        ],
        answerIndex: 1,
        explanation:
          "Tumor testis umumnya berupa massa keras yang tidak nyeri pada testis. Nyeri hebat lebih sering pada torsi testis atau infeksi akut."
      },
      {
        topic: "Genitalia Pria",
        question: "Epididimis secara anatomi terletak terutama di bagian:",
        options: [
          "Anterior testis",
          "Posterior testis",
          "Superior uretra",
          "Medial penis"
        ],
        answerIndex: 1,
        explanation:
          "Epididimis terletak di posterior testis dan berperan dalam pematangan dan penyimpanan awal sperma."
      },
      {
        topic: "Genitalia Pria",
        question: "Untuk menilai adanya hernia inguinal, posisi dan manuver yang paling sering digunakan adalah:",
        options: [
          "Pasien supin tanpa manuver",
          "Pasien berdiri lalu diminta batuk atau mengejan",
          "Pasien duduk sambil menahan napas",
          "Pasien terlentang dengan tungkai lurus"
        ],
        answerIndex: 1,
        explanation:
          "Hernia inguinal lebih mudah tampak saat tekanan intraabdomen meningkat, misalnya ketika pasien berdiri dan batuk atau mengejan."
      },
      {
        topic: "Prostat (DRE)",
        question: "Pada pemeriksaan DRE, karakteristik prostat normal adalah:",
        options: [
          "Ukuran sangat besar, konsistensi keras, noduler",
          "Ukuran kecil, konsistensi lunak, permukaan berbenjol",
          "Ukuran sedang, konsistensi padat kenyal, permukaan halus",
          "Tidak teraba sama sekali"
        ],
        answerIndex: 2,
        explanation:
          "Prostat normal berukuran kira-kira sebesar buah kenari besar dengan konsistensi padat kenyal dan permukaan halus."
      },
      {
        topic: "Prostat (DRE)",
        question: "Temuan yang paling mengarah pada kecurigaan keganasan prostat pada DRE adalah:",
        options: [
          "Prostat membesar, permukaan halus, konsistensi padat kenyal",
          "Prostat sangat keras, noduler, dan asimetris",
          "Prostat lunak dan mengecil",
          "Prostat nyeri tekan tanpa nodul"
        ],
        answerIndex: 1,
        explanation:
          "Kanker prostat sering memberikan gambaran prostat yang sangat keras, permukaan noduler, dan mungkin asimetris."
      },
      {
        topic: "Prostat (DRE)",
        question: "Posisi pasien yang paling umum digunakan saat melakukan pemeriksaan DRE adalah:",
        options: [
          "Posisi litotomi",
          "Posisi knee-chest",
          "Posisi miring kiri (left lateral) dengan lutut fleksi",
          "Posisi berdiri tegak"
        ],
        answerIndex: 2,
        explanation:
          "Posisi left lateral (Sim's) dengan lutut fleksi banyak digunakan karena memberikan akses yang baik dan relatif nyaman."
      },
      {
        topic: "Genitalia Wanita",
        question: "Posisi standar pasien untuk pemeriksaan spekulum pada genitalia wanita adalah:",
        options: [
          "Left lateral",
          "Knee-chest",
          "Litotomi",
          "Prone"
        ],
        answerIndex: 2,
        explanation:
          "Pemeriksaan dengan spekulum biasanya dilakukan pada posisi litotomi dengan kaki ditopang pada leg support."
      },
      {
        topic: "Genitalia Wanita",
        question: "Pemeriksaan bimanual pada genitalia wanita UTAMA digunakan untuk menilai:",
        options: [
          "Ukuran dan konsistensi uterus serta adneksa",
          "Derajat skoliosis tulang belakang",
          "Fungsi sfingter ani",
          "Kelainan pada paru-paru"
        ],
        answerIndex: 0,
        explanation:
          "Pemeriksaan bimanual menilai uterus (ukuran, posisi, mobilitas) dan adneksa (ovarium dan tuba) terhadap adanya massa atau nyeri."
      },
      {
        topic: "Genitalia Wanita",
        question: "Pemeriksaan skrining utama untuk lesi prakanker serviks adalah:",
        options: [
          "Foto polos abdomen",
          "Pap smear (sitologi serviks)",
          "USG transabdominal",
          "Pemeriksaan analisis urin"
        ],
        answerIndex: 1,
        explanation:
          "Pap smear digunakan luas sebagai pemeriksaan skrining lesi prakanker dan kanker serviks."
      },
      {
        topic: "Penunjang",
        question: "Kombinasi nitrit positif dan leukocyte esterase positif pada urinalisis paling mengarah pada:",
        options: [
          "Glomerulonefritis akut imunologis",
          "Infeksi saluran kemih bakteri",
          "Nefrolitiasis tanpa infeksi",
          "Diabetes insipidus"
        ],
        answerIndex: 1,
        explanation:
          "Nitrit positif menandakan adanya bakteri pengurai nitrat, sedangkan leukocyte esterase positif menandakan leukosituria, keduanya khas pada infeksi saluran kemih."
      },
      {
        topic: "Penunjang",
        question: "Pemeriksaan imaging non-invasif pertama yang paling sering dipilih untuk menilai hidronefrosis adalah:",
        options: [
          "USG ginjal dan traktus urinarius",
          "CT urografi dengan kontras",
          "MRI seluruh tubuh",
          "Foto polos thoraks"
        ],
        answerIndex: 0,
        explanation:
          "USG ginjal dan traktus urinarius aman, tanpa radiasi, dan sensitif untuk mendeteksi dilatasi sistem pelvikokaliks (hidronefrosis)."
      },
      {
        topic: "Penunjang",
        question: "Pemeriksaan micturating cystourethrography (MCU) secara utama digunakan untuk menilai:",
        options: [
          "Fungsi filtrasi glomerulus",
          "Refluks vesikoureteral dan kelainan uretra",
          "Ukuran dan morfologi ovarium",
          "Varikokel pada skrotum"
        ],
        answerIndex: 1,
        explanation:
          "MCU dilakukan dengan kontras pada kandung kemih dan pencitraan saat miksi untuk menilai refluks vesikoureteral serta kelainan uretra."
      },
      {
        topic: "Penunjang",
        question: "Pemeriksaan laboratorium yang paling langsung menggambarkan fungsi filtrasi glomerulus adalah:",
        options: [
          "Kadar serum kreatinin dan perhitungan eGFR",
          "Hitung darah lengkap",
          "Kadar amilase serum",
          "Kadar kreatin kinase"
        ],
        answerIndex: 0,
        explanation:
          "Serum kreatinin dan estimasi eGFR merupakan parameter utama yang sering digunakan untuk menilai fungsi filtrasi glomerulus."
      }
    ];


    // ===========================
    // LOGIKA UI UMUM
    // ===========================
    const menuItems = document.querySelectorAll(".menu-item");
    const contentTitle = document.getElementById("content-title");
    const contentSubtitle = document.getElementById("content-subtitle");
    const contentPill = document.getElementById("content-pill");
    const contentBody = document.getElementById("content-body");
    const modeButtons = document.querySelectorAll(".mode-btn");


    let currentMode = "materi";
    let lastSectionKey = "anatomi";


    function setActiveSection(key) {
      const data = sections[key];
      if (!data) return;


      contentTitle.textContent = data.title;
      contentSubtitle.textContent = data.subtitle;
      contentPill.textContent = data.pill;
      contentBody.innerHTML = data.html;


      menuItems.forEach((btn) => {
        if (btn.dataset.section === key) {
          btn.classList.add("active");
        } else {
          btn.classList.remove("active");
        }
      });
    }


    function setMode(mode) {
      currentMode = mode;


      modeButtons.forEach((btn) => {
        if (btn.dataset.mode === mode) {
          btn.classList.add("active");
        } else {
          btn.classList.remove("active");
        }
      });


      if (mode === "materi") {
        setActiveSection(lastSectionKey);
      } else if (mode === "quiz") {
        renderQuizUI();
        initExam();
      }
    }


    menuItems.forEach((btn) => {
      btn.addEventListener("click", () => {
        const sectionKey = btn.dataset.section;
        lastSectionKey = sectionKey;
        if (currentMode !== "materi") {
          setMode("materi");
        } else {
          setActiveSection(sectionKey);
        }
      });
    });


    modeButtons.forEach((btn) => {
      btn.addEventListener("click", () => {
        const mode = btn.dataset.mode;
        if (mode !== currentMode) {
          setMode(mode);
        }
      });
    });


    // ===========================
    // LOGIKA QUIZ / UJIAN
    // ===========================
    let shuffledQuestions = [];
    let currentQuestionIndex = 0;
    let correctCount = 0;
    let userAnswers = [];
    let questionAnswered = false;


    let quizProgressEl = null;
    let quizQuestionEl = null;
    let quizOptionsEl = null;
    let quizFeedbackEl = null;
    let quizNextBtn = null;
    let quizRestartBtn = null;
    let quizSummaryEl = null;


    function shuffleArray(arr) {
      const a = arr.slice();
      for (let i = a.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [a[i], a[j]] = [a[j], a[i]];
      }
      return a;
    }


    function renderQuizUI() {
      contentTitle.textContent = "Ujian Sistem Genitourinaria (MCQ)";
      contentSubtitle.textContent =
        "Kumpulan soal pilihan ganda dari seluruh topik: anatomi, pemeriksaan fisik, dan penunjang.";
      contentPill.textContent = "Mode: Ujian Komprehensif";


      contentBody.innerHTML = `
        <div class="quiz-intro">
          <p>Jawab seluruh soal berikut. Setiap soal memiliki satu jawaban yang paling tepat.</p>
          <ul>
            <li>Total soal saat ini: <strong>${examQuestions.length}</strong></li>
            <li>Setiap soal langsung diberikan pembahasan singkat setelah dijawab.</li>
            <li>Di akhir, akan muncul rangkuman skor dan rekap singkat.</li>
          </ul>
        </div>
        <div class="quiz-main">
          <div class="quiz-top">
            <span id="quiz-progress">Soal 1</span>
            <button type="button" id="quiz-restart-btn" class="quiz-secondary-btn">Mulai Ulang Ujian</button>
          </div>
          <div class="quiz-question" id="quiz-question"></div>
          <div class="quiz-options" id="quiz-options"></div>
          <div class="quiz-feedback" id="quiz-feedback"></div>
          <div class="quiz-bottom">
            <button type="button" id="quiz-next-btn" class="quiz-primary-btn" disabled>Soal Berikutnya</button>
          </div>
          <div class="quiz-summary" id="quiz-summary" style="display:none;"></div>
        </div>
      `;


      quizProgressEl = document.getElementById("quiz-progress");
      quizQuestionEl = document.getElementById("quiz-question");
      quizOptionsEl = document.getElementById("quiz-options");
      quizFeedbackEl = document.getElementById("quiz-feedback");
      quizNextBtn = document.getElementById("quiz-next-btn");
      quizRestartBtn = document.getElementById("quiz-restart-btn");
      quizSummaryEl = document.getElementById("quiz-summary");


      quizRestartBtn.addEventListener("click", () => {
        initExam();
      });


      quizNextBtn.addEventListener("click", () => {
        goToNextQuestion();
      });
    }


    function initExam() {
      shuffledQuestions = shuffleArray(examQuestions);
      currentQuestionIndex = 0;
      correctCount = 0;
      userAnswers = [];
      questionAnswered = false;


      if (quizSummaryEl) {
        quizSummaryEl.style.display = "none";
        quizSummaryEl.innerHTML = "";
      }


      showQuestion();
    }


    function showQuestion() {
      const q = shuffledQuestions[currentQuestionIndex];
      if (!q) {
        finishExam();
        return;
      }


      questionAnswered = false;
      quizFeedbackEl.textContent = "";
      quizNextBtn.disabled = true;
      quizNextBtn.textContent =
        currentQuestionIndex === shuffledQuestions.length - 1
          ? "Lihat Hasil Akhir"
          : "Soal Berikutnya";


      quizProgressEl.textContent = `Soal ${currentQuestionIndex + 1} dari ${shuffledQuestions.length}`;


      quizQuestionEl.innerHTML = `
        <span class="quiz-topic-tag">${q.topic}</span>${q.question}
      `;


      quizOptionsEl.innerHTML = "";
      const optionObjects = q.options.map((opt, index) => ({
        text: opt,
        isCorrect: index === q.answerIndex
      }));
      const randomizedOptions = shuffleArray(optionObjects);


      randomizedOptions.forEach((optObj) => {
        const btn = document.createElement("button");
        btn.type = "button";
        btn.className = "quiz-option";
        btn.textContent = optObj.text;
        btn.dataset.correct = optObj.isCorrect ? "true" : "false";
        btn.addEventListener("click", () => handleOptionClick(btn, q));
        quizOptionsEl.appendChild(btn);
      });
    }


    function handleOptionClick(selectedBtn, question) {
      if (questionAnswered) return;
      questionAnswered = true;


      const isCorrect = selectedBtn.dataset.correct === "true";
      const optionButtons = quizOptionsEl.querySelectorAll(".quiz-option");
      optionButtons.forEach((btn) => {
        const correct = btn.dataset.correct === "true";
        if (correct) {
          btn.classList.add("correct");
        }
        if (btn === selectedBtn && !correct) {
          btn.classList.add("incorrect");
        }
        btn.disabled = true;
      });


      if (isCorrect) {
        correctCount += 1;
        quizFeedbackEl.innerHTML =
          '<span class="quiz-feedback-correct">Benar.</span> ' +
          (question.explanation || "");
      } else {
        quizFeedbackEl.innerHTML =
          '<span class="quiz-feedback-incorrect">Salah.</span> ' +
          (question.explanation || "");
      }


      userAnswers[currentQuestionIndex] = {
        question,
        isCorrect
      };


      quizNextBtn.disabled = false;
    }


    function goToNextQuestion() {
      if (currentQuestionIndex < shuffledQuestions.length - 1) {
        currentQuestionIndex += 1;
        showQuestion();
      } else {
        finishExam();
      }
    }


    function finishExam() {
      const total = shuffledQuestions.length;
      const scorePercent = Math.round((correctCount / total) * 100);


      let msg = "";
      if (scorePercent >= 85) {
        msg = "Excellent, penguasaan materi sangat baik.";
      } else if (scorePercent >= 70) {
        msg = "Baik, tetap pertajam area yang masih lemah.";
      } else if (scorePercent >= 50) {
        msg = "Cukup, perlu review ulang beberapa topik.";
      } else {
        msg = "Perlu pengulangan materi. Fokus pada konsep dasar dan pemeriksaan fisik.";
      }


      quizQuestionEl.textContent = "";
      quizOptionsEl.innerHTML = "";
      quizFeedbackEl.textContent = "";
      quizNextBtn.disabled = true;


      quizProgressEl.textContent = `Selesai • Skor: ${correctCount}/${total} (${scorePercent}%)`;


      quizSummaryEl.style.display = "block";
      quizSummaryEl.innerHTML = `
        <h3>Ringkasan Hasil Ujian</h3>
        <p><strong>Skor:</strong> ${correctCount} dari ${total} soal (${scorePercent}%).</p>
        <p>${msg}</p>
        <h4>Rekap Singkat:</h4>
        <ul>
          ${shuffledQuestions
            .map((q, idx) => {
              const ua = userAnswers[idx];
              const status = ua && ua.isCorrect ? "✅" : "❌";
              return `<li>${status} Soal ${idx + 1} – ${q.topic}</li>`;
            })
            .join("")}
        </ul>
      `;
    }


    // Muat default awal
    setActiveSection("anatomi");
  </script>
</body>
</html>

