<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>COGBRIDGE – Sistem Interaksi Kognitif-AI</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
<script src="https://cdn.tailwindcss.com"></script>
<style>
  *{font-family:'Poppins',sans-serif!important;box-sizing:border-box}
  body{background:radial-gradient(ellipse at 30% 20%,#0d0d2b 0%,#060614 60%);min-height:100vh;display:flex;align-items:center;justify-content:center;margin:0;padding:20px}
  .screen{display:none;flex-direction:column;animation:fadeUp .35s ease both}
  .screen.active{display:flex}
  @keyframes fadeUp{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:translateY(0)}}
  @keyframes spin{from{transform:rotate(0)}to{transform:rotate(360deg)}}
  @keyframes pulse{0%,100%{box-shadow:0 0 0 0 rgba(99,102,241,.35)}50%{box-shadow:0 0 0 14px rgba(99,102,241,0)}}
  @keyframes scanLine{0%{top:0;opacity:1}100%{top:96px;opacity:0}}
  @keyframes bounceIn{0%{transform:scale(0);opacity:0}60%{transform:scale(1.2)}100%{transform:scale(1);opacity:1}}
  @keyframes ripple{0%{transform:scale(1);opacity:.5}100%{transform:scale(1.8);opacity:0}}
  @keyframes chatSlide{from{opacity:0;transform:translateX(-14px)}to{opacity:1;transform:translateX(0)}}
  @keyframes dot{0%,80%,100%{opacity:.25}40%{opacity:1}}
  .spin{animation:spin 1s linear infinite}
  .pulse-btn{animation:pulse 2.5s ease infinite}
  .bounce-in{animation:bounceIn .55s cubic-bezier(.34,1.56,.64,1) forwards}
  .chat-in{animation:chatSlide .45s ease both}
  .dot1{animation:dot 1.2s 0s infinite}
  .dot2{animation:dot 1.2s .2s infinite}
  .dot3{animation:dot 1.2s .4s infinite}
  textarea{resize:none;outline:none}
  textarea:focus{border-color:#6366F1!important;box-shadow:0 0 0 2px rgba(99,102,241,.2)!important}
  ::-webkit-scrollbar{width:3px}
  ::-webkit-scrollbar-thumb{background:#2a2a4a;border-radius:2px}
  .btn-primary{width:100%;padding:15px;background:linear-gradient(135deg,#6366F1,#4F46E5);border:none;border-radius:16px;color:white;font-size:13.5px;font-weight:700;cursor:pointer;letter-spacing:.3px;display:flex;align-items:center;justify-content:center;gap:8px;font-family:Poppins,sans-serif;transition:opacity .2s}
  .btn-primary:hover{opacity:.88}
  .btn-secondary{width:100%;padding:14px;background:linear-gradient(135deg,#4F46E5,#3B82F6);border:none;border-radius:14px;color:white;font-size:12.5px;font-weight:700;cursor:pointer;font-family:Poppins,sans-serif;transition:opacity .2s}
  .btn-secondary:hover{opacity:.88}
  .btn-green{width:100%;padding:15px;background:linear-gradient(135deg,#059669,#10B981);border:none;border-radius:16px;color:white;font-size:13.5px;font-weight:700;cursor:pointer;font-family:Poppins,sans-serif;transition:opacity .2s}
  .btn-green:hover{opacity:.88}
  .tag{display:inline-flex;align-items:center;gap:6px;border-radius:20px;padding:4px 12px}
  .send-btn{width:38px;height:38px;flex-shrink:0;align-self:flex-end;background:#6366F1;border:none;border-radius:11px;color:white;font-size:18px;cursor:pointer;display:flex;align-items:center;justify-content:center;font-family:Poppins;transition:opacity .2s}
  .send-btn:hover{opacity:.8}
</style>
</head>
<body>

<!-- Ambient glows -->
<div style="position:fixed;top:15%;left:20%;width:350px;height:350px;border-radius:50%;background:rgba(99,102,241,.05);filter:blur(70px);pointer-events:none;z-index:0"></div>
<div style="position:fixed;bottom:15%;right:20%;width:250px;height:250px;border-radius:50%;background:rgba(59,130,246,.05);filter:blur(60px);pointer-events:none;z-index:0"></div>

<!-- Phone Frame -->
<div style="width:390px;background:#08081a;border-radius:52px;border:1.5px solid rgba(99,102,241,.22);box-shadow:0 0 0 5px #0b0b1f,0 0 0 7px rgba(99,102,241,.12),0 50px 90px rgba(0,0,0,.7);overflow:hidden;display:flex;flex-direction:column;position:relative;z-index:1;max-height:96vh">

  <!-- Status Bar -->
  <div style="padding:14px 22px 8px;display:flex;align-items:flex-start;justify-content:space-between;flex-shrink:0">
    <span style="font-size:11px;font-weight:600;color:#e2e8f0">9:41</span>
    <div style="width:110px;height:26px;background:#000;border-radius:16px;margin-top:-6px"></div>
    <div style="display:flex;gap:5px;align-items:center;margin-top:2px">
      <svg width="14" height="10" fill="none"><rect x="0" y="3" width="3" height="7" rx="1" fill="rgba(255,255,255,.5)"/><rect x="4" y="2" width="3" height="8" rx="1" fill="rgba(255,255,255,.5)"/><rect x="8" y="0" width="3" height="10" rx="1" fill="rgba(255,255,255,.7)"/></svg>
      <svg width="16" height="10" viewBox="0 0 22 12" fill="none"><rect x="1" y="1" width="17" height="10" rx="2" stroke="rgba(255,255,255,.5)" stroke-width="1.5"/><rect x="18" y="4" width="2.5" height="4" rx="1" fill="rgba(255,255,255,.4)"/><rect x="2.5" y="2.5" width="12" height="7" rx="1.2" fill="rgba(255,255,255,.55)"/></svg>
    </div>
  </div>

  <!-- App Header -->
  <div style="padding:5px 20px 10px;display:flex;align-items:center;gap:9px;border-bottom:1px solid rgba(99,102,241,.1);flex-shrink:0">
    <div style="width:27px;height:27px;background:linear-gradient(135deg,#6366F1,#3B82F6);border-radius:8px;display:flex;align-items:center;justify-content:center;flex-shrink:0">
      <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>
    </div>
    <span style="font-size:14px;font-weight:900;color:#f1f5f9;letter-spacing:.8px">COGBRIDGE</span>
    <div id="app-status" style="margin-left:auto;display:flex;align-items:center;gap:4px;background:rgba(16,185,129,.1);border:1px solid rgba(16,185,129,.25);border-radius:20px;padding:3px 9px">
      <div style="width:5px;height:5px;border-radius:50%;background:#10B981"></div>
      <span style="color:#34D399;font-size:9px;font-weight:700;letter-spacing:.5px">AKTIF</span>
    </div>
  </div>

  <!-- Screens Container -->
  <div style="flex:1;overflow:hidden;position:relative;min-height:580px">

    <!-- ==================== SCREEN 1: DASHBOARD ==================== -->
    <div id="s0" class="screen active" style="height:100%;overflow-y:auto;padding:18px 20px;gap:14px">
      
      <!-- Greeting -->
      <div style="display:flex;align-items:center;gap:12px">
        <div style="width:48px;height:48px;border-radius:14px;background:linear-gradient(135deg,#6366F1,#3B82F6);display:flex;align-items:center;justify-content:center;font-size:20px;font-weight:800;color:white;flex-shrink:0">F</div>
        <div>
          <p style="color:#64748b;font-size:11px;font-weight:500;margin:0">Selamat datang kembali 👋</p>
          <h2 style="color:#f1f5f9;font-size:20px;font-weight:800;margin:0;line-height:1.1">Fatih!</h2>
        </div>
        <div style="margin-left:auto;background:rgba(99,102,241,.12);border:1px solid rgba(99,102,241,.25);border-radius:20px;padding:4px 10px;font-size:9px;color:#818CF8;font-weight:700;letter-spacing:.5px">SESI BARU</div>
      </div>

      <!-- Section Label -->
      <p style="color:#475569;font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:1.2px;margin-top:2px;margin-bottom:0">Metrik Kognitif Anda</p>
      
      <!-- Metric Cards -->
      <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px">
        <div style="background:linear-gradient(135deg,rgba(99,102,241,.14),rgba(99,102,241,.04));border:1px solid rgba(99,102,241,.22);border-radius:16px;padding:14px">
          <p style="color:#818CF8;font-size:9px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;margin:0 0 8px">Skor Metakognisi</p>
          <div style="display:flex;align-items:baseline;gap:3px;margin-bottom:8px">
            <span style="font-size:30px;font-weight:900;color:#f1f5f9">72</span>
            <span style="font-size:11px;color:#6366F1">/100</span>
          </div>
          <div style="height:4px;background:rgba(99,102,241,.15);border-radius:2px;overflow:hidden">
            <div style="width:72%;height:100%;background:linear-gradient(90deg,#6366F1,#818CF8);border-radius:2px"></div>
          </div>
          <p style="color:#34D399;font-size:10px;margin:6px 0 0;font-weight:600">↑ +5% minggu ini</p>
        </div>
        <div style="background:linear-gradient(135deg,rgba(59,130,246,.14),rgba(59,130,246,.04));border:1px solid rgba(59,130,246,.22);border-radius:16px;padding:14px">
          <p style="color:#60A5FA;font-size:9px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;margin:0 0 8px">Efikasi Diri</p>
          <div style="display:flex;align-items:baseline;gap:3px;margin-bottom:8px">
            <span id="ef-score" style="font-size:30px;font-weight:900;color:#f1f5f9">65</span>
            <span style="font-size:11px;color:#3B82F6">/100</span>
          </div>
          <div style="height:4px;background:rgba(59,130,246,.15);border-radius:2px;overflow:hidden">
            <div id="ef-bar" style="width:65%;height:100%;background:linear-gradient(90deg,#3B82F6,#60A5FA);border-radius:2px;transition:width .6s ease"></div>
          </div>
          <p id="ef-trend" style="color:#94A3B8;font-size:10px;margin:6px 0 0;font-weight:500">→ Stabil</p>
        </div>
      </div>

      <!-- Decision Fatigue -->
      <div style="background:rgba(16,185,129,.07);border:1px solid rgba(16,185,129,.18);border-radius:14px;padding:13px;display:flex;align-items:center;gap:11px">
        <div style="width:38px;height:38px;border-radius:11px;background:rgba(16,185,129,.12);display:flex;align-items:center;justify-content:center;font-size:18px;flex-shrink:0">🧠</div>
        <div style="flex:1">
          <p style="color:#64748b;font-size:10px;font-weight:500;margin:0 0 2px">Level Decision Fatigue</p>
          <p style="color:#34D399;font-size:15px;font-weight:700;margin:0">Rendah ✓</p>
        </div>
        <div style="display:flex;gap:3px;align-items:flex-end">
          <div style="width:5px;border-radius:2px;background:#10B981;height:18px"></div>
          <div style="width:5px;border-radius:2px;background:rgba(255,255,255,.1);height:24px"></div>
          <div style="width:5px;border-radius:2px;background:rgba(255,255,255,.1);height:20px"></div>
          <div style="width:5px;border-radius:2px;background:rgba(255,255,255,.1);height:28px"></div>
          <div style="width:5px;border-radius:2px;background:rgba(255,255,255,.1);height:22px"></div>
        </div>
      </div>

      <!-- PFC Status -->
      <div style="background:rgba(255,255,255,.025);border:1px solid rgba(255,255,255,.06);border-radius:14px;padding:14px">
        <p style="color:#475569;font-size:9px;font-weight:700;text-transform:uppercase;letter-spacing:1px;margin:0 0 10px">Status PFC Hari Ini</p>
        <div style="display:flex;flex-direction:column;gap:9px">
          <div>
            <div style="display:flex;justify-content:space-between;margin-bottom:3px">
              <span style="color:#94A3B8;font-size:10px">Penalaran Kritis</span>
              <span style="color:#818CF8;font-size:10px;font-weight:600">78%</span>
            </div>
            <div style="height:3px;background:rgba(255,255,255,.07);border-radius:2px">
              <div style="width:78%;height:100%;background:linear-gradient(90deg,#6366F1,#60A5FA);border-radius:2px"></div>
            </div>
          </div>
          <div>
            <div style="display:flex;justify-content:space-between;margin-bottom:3px">
              <span style="color:#94A3B8;font-size:10px">Pengambilan Keputusan</span>
              <span style="color:#60A5FA;font-size:10px;font-weight:600">65%</span>
            </div>
            <div style="height:3px;background:rgba(255,255,255,.07);border-radius:2px">
              <div style="width:65%;height:100%;background:linear-gradient(90deg,#3B82F6,#60A5FA);border-radius:2px"></div>
            </div>
          </div>
          <div>
            <div style="display:flex;justify-content:space-between;margin-bottom:3px">
              <span style="color:#94A3B8;font-size:10px">Regulasi Emosi</span>
              <span style="color:#34D399;font-size:10px;font-weight:600">81%</span>
            </div>
            <div style="height:3px;background:rgba(255,255,255,.07);border-radius:2px">
              <div style="width:81%;height:100%;background:linear-gradient(90deg,#059669,#34D399);border-radius:2px"></div>
            </div>
          </div>
        </div>
      </div>

      <!-- CTA Button -->
      <button class="btn-primary pulse-btn" onclick="goTo(1)" style="margin-top:4px">
        <span>⚡</span> Mulai Sesi Kognitif Baru <span>→</span>
      </button>
    </div><!-- /s0 -->


    <!-- ==================== SCREEN 2: THINKING CANVAS ==================== -->
    <div id="s1" class="screen" style="height:100%;overflow-y:auto;padding:16px 20px;gap:13px">
      
      <!-- Progress -->
      <div style="display:flex;gap:5px">
        <div style="flex:1;height:3px;border-radius:2px;background:#6366F1"></div>
        <div style="flex:1;height:3px;border-radius:2px;background:rgba(255,255,255,.1)"></div>
        <div style="flex:1;height:3px;border-radius:2px;background:rgba(255,255,255,.1)"></div>
        <div style="flex:1;height:3px;border-radius:2px;background:rgba(255,255,255,.1)"></div>
      </div>

      <div>
        <div class="tag" style="background:rgba(99,102,241,.13);border:1px solid rgba(99,102,241,.28);margin-bottom:8px">
          <div style="width:5px;height:5px;border-radius:50%;background:#6366F1"></div>
          <span style="color:#818CF8;font-size:9px;font-weight:700;text-transform:uppercase;letter-spacing:1px">Fase 1 · Input Mandiri</span>
        </div>
        <h2 style="color:#f1f5f9;font-size:20px;font-weight:800;margin:0 0 5px">The Thinking Canvas</h2>
        <p style="color:#64748b;font-size:11px;line-height:1.65;margin:0">Jabarkan pemikiranmu secara <span style="color:#818CF8;font-weight:600">mandiri</span> sebelum AI dilibatkan. Tidak ada jalan pintas — kognisimu harus bekerja duluan.</p>
      </div>

      <div>
        <label style="display:block;color:#94A3B8;font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;margin-bottom:7px">📋 Konteks Masalah</label>
        <textarea id="t-konteks" placeholder="Deskripsikan masalah atau topik yang sedang kamu hadapi secara detail..." rows="4" style="width:100%;background:rgba(255,255,255,.03);border:1px solid rgba(99,102,241,.18);border-radius:13px;padding:11px 13px;color:#e2e8f0;font-size:12px;line-height:1.65;transition:border .2s,box-shadow .2s"></textarea>
      </div>

      <div>
        <label style="display:block;color:#94A3B8;font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;margin-bottom:7px">💡 Asumsi Awal</label>
        <textarea id="t-asumsi" placeholder="Apa asumsi atau hipotesis awal yang kamu miliki? Tulis dengan jujur..." rows="4" style="width:100%;background:rgba(255,255,255,.03);border:1px solid rgba(59,130,246,.18);border-radius:13px;padding:11px 13px;color:#e2e8f0;font-size:12px;line-height:1.65;transition:border .2s,box-shadow .2s"></textarea>
      </div>

      <div style="background:rgba(245,158,11,.07);border:1px solid rgba(245,158,11,.2);border-radius:11px;padding:10px 12px;display:flex;gap:8px;align-items:flex-start">
        <span style="font-size:13px;flex-shrink:0">⚠️</span>
        <p style="color:#FCD34D;font-size:10.5px;line-height:1.55;margin:0">Semakin kamu jujur dan detail di sini, semakin tajam pertanyaan Sokratik yang akan mengujimu.</p>
      </div>

      <button class="btn-secondary" onclick="goTo(2)">
        🔍 Kirim untuk Pengujian AI (Scrutiny) →
      </button>
    </div><!-- /s1 -->


    <!-- ==================== SCREEN 3: SOCRATIC LAB ==================== -->
    <div id="s2" class="screen" style="height:100%;flex-direction:column">
      
      <div style="padding:14px 20px 10px;flex-shrink:0">
        <div style="display:flex;gap:5px;margin-bottom:10px">
          <div style="flex:1;height:3px;border-radius:2px;background:#6366F1"></div>
          <div style="flex:1;height:3px;border-radius:2px;background:#6366F1"></div>
          <div style="flex:1;height:3px;border-radius:2px;background:#6366F1"></div>
          <div style="flex:1;height:3px;border-radius:2px;background:rgba(255,255,255,.1)"></div>
        </div>
        <div class="tag" style="background:rgba(59,130,246,.12);border:1px solid rgba(59,130,246,.25)">
          <div style="width:5px;height:5px;border-radius:50%;background:#3B82F6"></div>
          <span style="color:#60A5FA;font-size:9px;font-weight:700;text-transform:uppercase;letter-spacing:1px">Fase 2 & 3 · Socratic Lab</span>
        </div>
      </div>

      <!-- Loading State -->
      <div id="loading-state" style="flex:1;display:flex;flex-direction:column;align-items:center;justify-content:center;padding:30px;gap:22px">
        <div style="position:relative;width:96px;height:96px">
          <div style="position:absolute;inset:0;border-radius:50%;border:2px solid rgba(99,102,241,.2)"></div>
          <div class="spin" style="position:absolute;inset:4px;border-radius:50%;border:2.5px solid transparent;border-top-color:#6366F1;border-right-color:#3B82F6"></div>
          <div style="position:absolute;inset:0;display:flex;align-items:center;justify-content:center;font-size:30px">🧠</div>
          <div style="position:absolute;left:0;right:0;height:2px;background:linear-gradient(90deg,transparent,#6366F1,transparent);top:0;animation:scanLine 1.8s ease-in-out infinite"></div>
        </div>
        <div style="text-align:center">
          <p style="color:#818CF8;font-size:14px;font-weight:700;margin:0 0 5px">Memindai celah logika</p>
          <p style="color:#475569;font-size:11px;line-height:1.6;margin:0">dan asumsi Anda sedang dianalisis...</p>
        </div>
        <div style="display:flex;gap:8px">
          <div class="dot1" style="width:9px;height:9px;border-radius:50%;background:#6366F1"></div>
          <div class="dot2" style="width:9px;height:9px;border-radius:50%;background:#6366F1"></div>
          <div class="dot3" style="width:9px;height:9px;border-radius:50%;background:#6366F1"></div>
        </div>
      </div>

      <!-- Chat State -->
      <div id="chat-state" style="display:none;flex:1;flex-direction:column;overflow:hidden">
        <div id="chat-messages" style="flex:1;overflow-y:auto;padding:14px 20px;display:flex;flex-direction:column;gap:12px">
          
          <!-- AI Message -->
          <div class="chat-in" style="display:flex;gap:9px">
            <div style="width:28px;height:28px;border-radius:9px;background:linear-gradient(135deg,#6366F1,#3B82F6);display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:2px">
              <svg width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>
            </div>
            <div>
              <p style="color:#475569;font-size:9px;font-weight:600;margin:0 0 4px;text-transform:uppercase;letter-spacing:.5px">COGBRIDGE AI · Fase 2: Scrutiny</p>
              <div style="background:rgba(99,102,241,.1);border:1px solid rgba(99,102,241,.18);border-radius:4px 14px 14px 14px;padding:13px;max-width:290px">
                <p style="color:#818CF8;font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:.5px;margin:0 0 7px">🔍 Celah Logika Terdeteksi</p>
                <p style="color:#cbd5e1;font-size:11.5px;line-height:1.65;margin:0 0 10px">Argumenmu menunjukkan potensi <span style="color:#F87171;font-weight:600">asumsi kausalitas tanpa bukti empiris</span> dan kecenderungan <span style="color:#FBBF24;font-weight:600">confirmation bias</span> dalam pemilihan data pendukung.</p>
                <div style="height:1px;background:rgba(99,102,241,.18);margin:0 0 10px"></div>
                <p style="color:#818CF8;font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:.5px;margin:0 0 7px">💡 Pertanyaan Sokratik</p>
                <p style="color:#e2e8f0;font-size:11.5px;line-height:1.65;margin:0;font-style:italic">"Jika asumsimu benar, bukti kontradiktif seperti apa yang akan mengubah pendirianmu? Dan sudahkah kamu mempertimbangkan bahwa premis awalmu sendiri yang mungkin keliru?"</p>
              </div>
            </div>
          </div>

          <!-- User reply placeholder -->
          <div id="user-reply-bubble" style="display:none;justify-content:flex-end">
            <div style="background:rgba(59,130,246,.12);border:1px solid rgba(59,130,246,.22);border-radius:14px 4px 14px 14px;padding:11px 14px;max-width:250px">
              <p id="user-reply-text" style="color:#e2e8f0;font-size:11.5px;line-height:1.6;margin:0"></p>
            </div>
          </div>

        </div>

        <div style="padding:12px 20px;border-top:1px solid rgba(99,102,241,.1);flex-shrink:0">
          <div style="display:flex;gap:8px;margin-bottom:9px">
            <textarea id="t-chat" placeholder="Pertahankan argumenmu atau revisi asumsimu..." rows="2" style="flex:1;background:rgba(255,255,255,.03);border:1px solid rgba(99,102,241,.18);border-radius:12px;padding:9px 12px;color:#e2e8f0;font-size:11.5px;line-height:1.5;transition:border .2s,box-shadow .2s"></textarea>
            <button class="send-btn" onclick="sendChat()">→</button>
          </div>
          <button onclick="goTo(3)" style="width:100%;padding:12px;background:rgba(239,68,68,.1);border:1px solid rgba(239,68,68,.25);border-radius:12px;color:#FCA5A5;font-size:12px;font-weight:700;cursor:pointer;font-family:Poppins;transition:background .2s" onmouseover="this.style.background='rgba(239,68,68,.18)'" onmouseout="this.style.background='rgba(239,68,68,.1)'">
            ⚔️ Akhiri Debat &amp; Putuskan →
          </button>
        </div>
      </div>

    </div><!-- /s2 -->


    <!-- ==================== SCREEN 4: SOVEREIGN OUTCOME ==================== -->
    <div id="s3" class="screen" style="height:100%;overflow-y:auto;padding:16px 20px;gap:13px">
      
      <div style="display:flex;gap:5px">
        <div style="flex:1;height:3px;border-radius:2px;background:#6366F1"></div>
        <div style="flex:1;height:3px;border-radius:2px;background:#6366F1"></div>
        <div style="flex:1;height:3px;border-radius:2px;background:#6366F1"></div>
        <div style="flex:1;height:3px;border-radius:2px;background:#6366F1"></div>
      </div>

      <!-- Warning Banner -->
      <div style="background:rgba(245,158,11,.09);border:1px solid rgba(245,158,11,.28);border-radius:14px;padding:14px;display:flex;gap:11px;align-items:flex-start">
        <span style="font-size:22px;flex-shrink:0">🔓</span>
        <div>
          <p style="color:#FCD34D;font-size:13.5px;font-weight:800;margin:0 0 4px">AI Scaffolding Dilepas.</p>
          <p style="color:#D97706;font-size:11px;line-height:1.55;margin:0">Anda memegang kendali penuh. Tidak ada lagi bantuan eksternal — hanya nalar murnimu yang tersisa.</p>
        </div>
      </div>

      <div>
        <div class="tag" style="background:rgba(16,185,129,.12);border:1px solid rgba(16,185,129,.25);margin-bottom:8px">
          <div style="width:5px;height:5px;border-radius:50%;background:#10B981"></div>
          <span style="color:#34D399;font-size:9px;font-weight:700;text-transform:uppercase;letter-spacing:1px">Fase 4 · Sovereign Outcome</span>
        </div>
        <h2 style="color:#f1f5f9;font-size:20px;font-weight:800;margin:0 0 5px">Keputusanmu</h2>
        <p style="color:#64748b;font-size:11px;line-height:1.65;margin:0">Tuliskan kesimpulan final dari hasil nalar <span style="color:#34D399;font-weight:600">murnimu sendiri</span>. Ini adalah output kognitifmu yang sesungguhnya.</p>
      </div>

      <textarea id="t-kesimpulan" placeholder="Tuliskan kesimpulan, keputusan, atau insight yang kamu capai setelah melewati seluruh proses dialektika ini..." rows="8" style="width:100%;background:rgba(16,185,129,.04);border:1px solid rgba(16,185,129,.18);border-radius:15px;padding:14px;color:#e2e8f0;font-size:12px;line-height:1.7;min-height:180px;transition:border .2s,box-shadow .2s"></textarea>

      <div style="background:rgba(255,255,255,.025);border:1px solid rgba(255,255,255,.06);border-radius:11px;padding:10px 13px;display:flex;align-items:center;gap:9px">
        <span style="font-size:16px">💎</span>
        <p style="color:#64748b;font-size:11px;line-height:1.5;margin:0">Setiap kata di sini adalah <span style="color:#818CF8">bukti aktivasi PFC</span> yang sesungguhnya.</p>
      </div>

      <button class="btn-green" onclick="goTo(4)">
        💾 Simpan Keputusan
      </button>
    </div><!-- /s3 -->


    <!-- ==================== SCREEN 5: SUCCESS ==================== -->
    <div id="s4" class="screen" style="height:100%;overflow-y:auto;align-items:center;justify-content:center;padding:24px 20px;gap:18px;text-align:center">

      <!-- Success Icon -->
      <div style="position:relative;margin-bottom:6px">
        <div id="success-icon" style="width:96px;height:96px;border-radius:50%;background:rgba(16,185,129,.13);border:2px solid rgba(16,185,129,.4);display:flex;align-items:center;justify-content:center;font-size:44px;color:#34D399;font-weight:900;opacity:0">✓</div>
        <div style="position:absolute;inset:-14px;border-radius:50%;border:1.5px solid rgba(16,185,129,.2);animation:ripple 2.2s ease-out infinite"></div>
        <div style="position:absolute;inset:-28px;border-radius:50%;border:1px solid rgba(16,185,129,.1);animation:ripple 2.2s ease-out .55s infinite"></div>
      </div>

      <!-- Text -->
      <div>
        <h2 style="color:#34D399;font-size:17px;font-weight:800;line-height:1.45;margin:0 0 10px">Prefrontal Cortex (PFC)<br>Anda Berhasil Diaktifkan!</h2>
        <p style="color:#94A3B8;font-size:11.5px;line-height:1.7;max-width:270px;margin:0 auto">melalui <span style="color:#818CF8;font-weight:600">dialektika mandiri</span> yang Anda jalani. Anda telah membuktikan bahwa nalar Anda mampu bekerja tanpa bergantung pada AI.</p>
      </div>

      <!-- Score Badge -->
      <div style="background:linear-gradient(135deg,rgba(99,102,241,.15),rgba(59,130,246,.15));border:1px solid rgba(99,102,241,.28);border-radius:20px;padding:15px 22px;display:flex;align-items:center;gap:16px">
        <div style="text-align:center">
          <p style="color:#64748b;font-size:9px;font-weight:700;text-transform:uppercase;letter-spacing:1px;margin:0 0 4px">Efikasi Diri</p>
          <div style="display:flex;align-items:baseline;gap:3px;justify-content:center">
            <span style="color:#34D399;font-size:26px;font-weight:900">+2</span>
            <span style="color:#64748b;font-size:12px">Poin</span>
          </div>
        </div>
        <div style="width:1px;height:38px;background:rgba(99,102,241,.2)"></div>
        <div style="text-align:center">
          <p style="color:#64748b;font-size:9px;font-weight:700;text-transform:uppercase;letter-spacing:1px;margin:0 0 4px">Skor Baru</p>
          <span id="new-score" style="color:#f1f5f9;font-size:26px;font-weight:900">67</span>
        </div>
        <div style="width:1px;height:38px;background:rgba(99,102,241,.2)"></div>
        <div style="text-align:center">
          <p style="color:#64748b;font-size:9px;font-weight:700;text-transform:uppercase;letter-spacing:1px;margin:0 0 4px">Sesi</p>
          <span style="font-size:22px">🎯</span>
        </div>
      </div>

      <!-- Achievement badges -->
      <div style="display:flex;gap:7px;flex-wrap:wrap;justify-content:center">
        <div style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.08);border-radius:20px;padding:5px 11px;display:flex;align-items:center;gap:5px">
          <span style="font-size:13px">🧠</span><span style="color:#94A3B8;font-size:10px;font-weight:500">Pemikir Mandiri</span>
        </div>
        <div style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.08);border-radius:20px;padding:5px 11px;display:flex;align-items:center;gap:5px">
          <span style="font-size:13px">⚡</span><span style="color:#94A3B8;font-size:10px;font-weight:500">PFC Aktif</span>
        </div>
        <div style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.08);border-radius:20px;padding:5px 11px;display:flex;align-items:center;gap:5px">
          <span style="font-size:13px">💎</span><span style="color:#94A3B8;font-size:10px;font-weight:500">Dialectician</span>
        </div>
      </div>

      <button class="btn-primary" onclick="goTo(0)" style="margin-top:4px">
        ← Kembali ke Dashboard
      </button>
    </div><!-- /s4 -->

  </div><!-- /screens container -->

  <!-- Home indicator -->
  <div style="height:30px;display:flex;align-items:center;justify-content:center;flex-shrink:0">
    <div style="width:110px;height:4px;background:rgba(241,245,249,.2);border-radius:3px"></div>
  </div>

</div><!-- /phone -->

<script>
var efikasi = 65;
var loadTimer = null;
var totalSessions = 0;

function goTo(n) {
  var screens = document.querySelectorAll('.screen');
  screens.forEach(function(s) { s.classList.remove('active'); });
  var next = document.getElementById('s' + n);
  if (!next) return;
  setTimeout(function() {
    next.classList.add('active');
    if (n === 2) { startLoading(); }
    if (n === 4) { animateSuccess(); }
  }, 30);
}

function startLoading() {
  var ls = document.getElementById('loading-state');
  var cs = document.getElementById('chat-state');
  if (ls) ls.style.display = 'flex';
  if (cs) cs.style.display = 'none';
  clearTimeout(loadTimer);
  loadTimer = setTimeout(function() {
    if (ls) ls.style.display = 'none';
    if (cs) { cs.style.display = 'flex'; }
  }, 2200);
}

function sendChat() {
  var inp = document.getElementById('t-chat');
  var bubble = document.getElementById('user-reply-bubble');
  var txt = document.getElementById('user-reply-text');
  if (inp && inp.value.trim() && bubble && txt) {
    txt.textContent = inp.value.trim();
    bubble.style.display = 'flex';
    inp.value = '';
    var msgs = document.getElementById('chat-messages');
    if (msgs) msgs.scrollTop = msgs.scrollHeight;
  }
}

function animateSuccess() {
  totalSessions++;
  efikasi = Math.min(100, efikasi + 2);
  var icon = document.getElementById('success-icon');
  var ns = document.getElementById('new-score');
  var ef = document.getElementById('ef-score');
  var efb = document.getElementById('ef-bar');
  var eft = document.getElementById('ef-trend');
  if (ns) ns.textContent = efikasi;
  if (ef) ef.textContent = efikasi;
  if (efb) efb.style.width = efikasi + '%';
  if (eft) { eft.textContent = '↑ Meningkat +2'; eft.style.color = '#34D399'; }
  if (icon) {
    icon.style.opacity = '0';
    icon.style.transform = 'scale(0)';
    setTimeout(function() {
      icon.classList.add('bounce-in');
      icon.style.opacity = '1';
      icon.style.transform = '';
    }, 100);
  }
}

// Allow Enter key to send in chat (Shift+Enter for newline)
document.addEventListener('keydown', function(e) {
  if (e.target && e.target.id === 't-chat' && e.key === 'Enter' && !e.shiftKey) {
    e.preventDefault();
    sendChat();
  }
});
</script>

</body>
</html>
