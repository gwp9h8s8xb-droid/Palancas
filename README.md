<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Inmobiliaria Palancas</title>
  <meta name="description" content="Inmobiliaria Palancas · Venta y alquiler de viviendas, oficinas y locales en Ávila y Comunidad de Madrid. Contacta para visitar una propiedad.">
  <meta property="og:title" content="Inmobiliaria Palancas">
  <meta property="og:description" content="Venta y alquiler de propiedades en Ávila y Madrid.">
  <meta property="og:type" content="website">
  <meta property="og:url" content="https://tudominio.com">
  <meta property="og:image" content="/img/og.jpg">
  <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='0.9em' font-size='90'>🏠</text></svg>">
  <style>
    :root{--bg:#0b0d11;--fg:#e9eef5;--muted:#a7b0bd;--card:#12151b;--brand:#1d4ed8;--accent:#93c5fd;--ok:#22c55e;--warn:#f59e0b;--err:#ef4444}
    *{box-sizing:border-box}html,body{margin:0;height:100%;background:var(--bg);color:var(--fg);font:16px/1.5 system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,'Helvetica Neue',Arial}
    a{color:var(--accent)}img{max-width:100%;display:block;border-radius:12px}
    .wrap{max-width:1100px;margin:0 auto;padding:24px}
    header{display:flex;gap:16px;align-items:center;justify-content:space-between;padding:12px 0}
    .logo{display:flex;gap:12px;align-items:center}
    .logo b{font-size:1.1rem}
    nav a{margin-left:16px;text-decoration:none;color:var(--fg);opacity:.9}
    .hero{display:grid;grid-template-columns:1.2fr .8fr;gap:24px;align-items:center;padding:28px 0}
    .hero h1{font-size:2rem;margin:.2em 0}
    .hero p{color:var(--muted)}
    .badge{display:inline-flex;align-items:center;gap:8px;background:linear-gradient(90deg,var(--brand),var(--accent));color:#0b0d11;padding:6px 10px;border-radius:999px;font-weight:700}
    .panel{background:var(--card);border:1px solid #1f2530;padding:14px;border-radius:16px}
    .filters{display:grid;grid-template-columns:repeat(6,1fr);gap:10px}
    .filters input,.filters select{width:100%;padding:10px 12px;border-radius:10px;border:1px solid #2a3241;background:#0f1319;color:var(--fg)}
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:18px}
    .card{background:var(--card);border:1px solid #1f2530;border-radius:16px;overflow:hidden;display:flex;flex-direction:column}
    .card .body{padding:12px 14px;display:grid;gap:6px}
    .tag{display:inline-block;font-size:.75rem;padding:4px 8px;border-radius:999px;border:1px solid #263041;color:var(--muted)}
    .price{font-weight:800;font-size:1.15rem}
    .meta{color:var(--muted);font-size:.9rem}
    .btn{display:inline-block;text-align:center;padding:10px 12px;border-radius:10px;text-decoration:none;border:1px solid #264353;color:var(--fg);background:#0f1319}
    .btn.brand{border-color:transparent;background:linear-gradient(90deg,var(--brand),var(--accent));color:#0b0d11;font-weight:800}
    footer{margin:40px 0 20px;color:var(--muted);font-size:.9rem}
    .contact{display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-top:18px}
    .contact input,.contact textarea{width:100%;padding:10px 12px;border-radius:10px;border:1px solid #2a3241;background:#0f1319;color:var(--fg)}
    .contact textarea{min-height:120px}
    .schema{display:none}
    @media (max-width:960px){.hero{grid-template-columns:1fr}.filters{grid-template-columns:repeat(2,1fr)}.grid{grid-template-columns:repeat(2,1fr)}}
    @media (max-width:640px){.filters{grid-template-columns:1fr}.grid{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="logo"><span style="font-size:1.5rem">🏠</span><b>Inmobiliaria Palancas</b></div>
      <nav>
        <a href="#listings">Propiedades</a>
        <a href="#contacto">Contacto</a>
      </nav>
    </header>

    <section class="hero">
      <div>
        <span class="badge">Mejor opción económica</span>
        <h1>Web inmobiliaria rápida, barata y efectiva</h1>
        <p>Sin CMS pesado, sin cuotas. Dirección física: Avenida Doctor Rodríguez de Miñón 2, Sotillo de la Adrada (Ávila). Tel: 912 79 49 52 · Email: info@palancas.es Un único archivo HTML que puedes subir gratis a GitHub Pages o Netlify. Edita el listado en el propio código o en un JSON aparte.</p>
        <p>
          <a class="btn brand" href="#contacto">Solicitar visita</a>
          <a class="btn" href="#como">Cómo publicarla gratis</a>
        </p>
      </div>
      <div class="panel">
        <div class="filters" id="filters">
          <input id="q" type="search" placeholder="Buscar barrio o título" />
          <select id="tipo">
            <option value="">Venta o Alquiler</option>
            <option>venta</option>
            <option>alquiler</option>
          </select>
          <select id="ciudad"></select>
          <select id="habitaciones">
            <option value="">Habitaciones</option>
            <option value="1">1+</option>
            <option value="2">2+</option>
            <option value="3">3+</option>
            <option value="4">4+</option>
          </select>
          <input id="precioMax" type="number" min="0" step="100" placeholder="Precio máx (€)" />
          <select id="orden">
            <option value="recientes">Recientes</option>
            <option value="precioAsc">Precio ↑</option>
            <option value="precioDesc">Precio ↓</option>
          </select>
        </div>
      </div>
    </section>

    <section id="listings">
      <div class="grid" id="grid"></div>
    </section>

    <section id="como" style="margin-top:38px">
      <h2>Cómo publicarla gratis</h2>
      <ol>
        <li>Crea una cuenta en <b>GitHub</b>, sube este archivo como <code>index.html</code>.</li>
        <li>Activa <b>GitHub Pages</b> en Settings → Pages → Source: <i>Deploy from a branch</i>.</li>
        <li>Opcional: compra un dominio barato y apúntalo a Pages. Si no, usa el subdominio gratuito <code>tusuario.github.io</code>.</li>
        <li>Para formularios, cambia el atributo <code>action</code> por tu endpoint de <b>Formspree</b> o similar (plan gratuito).</li>
      </ol>
    </section>

    <section id="contacto" class="panel" style="margin-top:28px">
      <h2>Contacto</h2>
      <p class="meta">📍 Avenida Doctor Rodríguez de Miñón 2, Sotillo de la Adrada, Ávila · <a href="https://maps.google.com/?q=Avenida%20Doctor%20Rodr%C3%ADguez%20de%20Mi%C3%B1%C3%B3n%202%20Sotillo%20de%20la%20Adrada%20Avila" target="_blank" rel="noopener">Ver mapa</a></p>
      <p class="meta">☎️ <a href="tel:+34912794952">912 79 49 52</a> · ✉️ <a href="mailto:info@palancas.es">info@palancas.es</a> · WhatsApp: <a href="https://wa.me/34633102934" target="_blank" rel="noopener">633 102 934</a> (secundario)</p>
      <form class="contact" method="POST" action="https://formspree.io/f/xqayvavw" onsubmit="submitted(event)">
        <input type="text" name="nombre" placeholder="Tu nombre" required>
        <input type="email" name="email" placeholder="Tu email" required>
        <input type="tel" name="telefono" placeholder="Teléfono">
        <textarea name="mensaje" placeholder="Quiero información sobre…" required></textarea>
        <button class="btn brand" type="submit">Enviar</button>
      </form>
      <p id="msg" class="meta" aria-live="polite"></p>
    </section>

    <footer>
      © <span id="year"></span> Inmobiliaria Palancas · <a href="#">Aviso legal</a> · <a href="#">Privacidad</a>
    </footer>
  </div>

  <!-- Datos de ejemplo: edítalos o cámbialos por un fetch a /propiedades.json -->
  <script>
    const PROPS = [
      {id:1,titulo:"Piso céntrico reformado",tipo:"venta",precio:235000,habitaciones:2,banos:1,m2:72,ciudad:"Madrid",barrio:"Lavapiés",img:"https://images.unsplash.com/photo-1505693416388-ac5ce068fe85?w=1200",destacado:true,fecha:"2025-10-01"},
      {id:2,titulo:"Ático con terraza",tipo:"alquiler",precio:1200,habitaciones:1,banos:1,m2:56,ciudad:"Madrid",barrio:"Chamberí",img:"https://images.unsplash.com/photo-1494526585095-c41746248156?w=1200",destacado:false,fecha:"2025-09-20"},
      {id:3,titulo:"Chalet adosado familiar",tipo:"venta",precio:365000,habitaciones:4,banos:3,m2:180,ciudad:"Alcalá de Henares",barrio:"Ensanche",img:"https://images.unsplash.com/photo-1568605114967-8130f3a36994?w=1200",destacado:true,fecha:"2025-10-10"},
      {id:4,titulo:"Loft luminoso",tipo:"alquiler",precio:850,habitaciones:1,banos:1,m2:40,ciudad:"Valencia",barrio:"Ruzafa",img:"https://images.unsplash.com/photo-1502005229762-cf1b2da7c54a?w=1200",destacado:false,fecha:"2025-08-28"},
      {id:5,titulo:"Local comercial en esquina",tipo:"alquiler",precio:950,habitaciones:0,banos:1,m2:75,ciudad:"Madrid",barrio:"Tetuán",img:"https://images.unsplash.com/photo-1501183638710-841dd1904471?w=1200",destacado:false,fecha:"2025-10-05"}
    ];

    // --- utilidades ---
    const $ = s=>document.querySelector(s);
    const grid = $('#grid');
    const ciudadSel = $('#ciudad');
    const q = $('#q');
    const tipo = $('#tipo');
    const hab = $('#habitaciones');
    const precioMax = $('#precioMax');
    const orden = $('#orden');

    // Rellenar ciudades únicas
    const ciudades = Array.from(new Set(PROPS.map(p=>p.ciudad))).sort();
    ciudadSel.innerHTML = '<option value="">Ciudad</option>' + ciudades.map(c=>`<option>${c}</option>`).join('');

    function fmtEUR(v){return new Intl.NumberFormat('es-ES',{style:'currency',currency:'EUR',maximumFractionDigits:0}).format(v)}

    function render(list){
      grid.innerHTML = '';
      list.forEach(p=>{
        const el = document.createElement('article');
        el.className = 'card';
        el.innerHTML = `
          <img src="${p.img}" alt="${p.titulo}">
          <div class="body">
            <div style="display:flex;justify-content:space-between;align-items:center;gap:8px">
              <strong>${p.titulo}</strong>
              <span class="tag">${p.ciudad} · ${p.barrio || ''}</span>
            </div>
            <div class="price">${fmtEUR(p.precio)} ${p.tipo==='alquiler'?'/ mes':''}</div>
            <div class="meta">${p.habitaciones||0} hab · ${p.banos||1} baño · ${p.m2||0} m²</div>
            <div style="display:flex;gap:8px;margin-top:6px">
              <a class="btn brand" href="#contacto" onclick="preRellenar(${p.id})">Me interesa</a>
              <a class="btn" href="#" onclick="share(${p.id})">Compartir</a>
            </div>
          </div>`;
        grid.appendChild(el);
      });
      if(!list.length){ grid.innerHTML = '<p class="meta">No hay propiedades con esos filtros.</p>'; }
    }

    function filtrar(){
      const term = q.value.trim().toLowerCase();
      const t = tipo.value;
      const c = ciudadSel.value;
      const h = Number(hab.value||0);
      const pm = Number(precioMax.value||0);
      let out = PROPS.filter(p=>{
        const txt = `${p.titulo} ${p.ciudad} ${p.barrio}`.toLowerCase();
        if(term && !txt.includes(term)) return false;
        if(t && p.tipo!==t) return false;
        if(c && p.ciudad!==c) return false;
        if(h && (p.habitaciones||0) < h) return false;
        if(pm && p.precio > pm) return false;
        return true;
      });
      if(orden.value==='precioAsc') out.sort((a,b)=>a.precio-b.precio);
      else if(orden.value==='precioDesc') out.sort((a,b)=>b.precio-a.precio);
      else out.sort((a,b)=> new Date(b.fecha)-new Date(a.fecha));
      render(out);
    }

    q.oninput = tipo.onchange = ciudadSel.onchange = hab.onchange = precioMax.oninput = orden.onchange = filtrar;

    function preRellenar(id){
      const p = PROPS.find(x=>x.id===id);
      const ta = document.querySelector('textarea[name="mensaje"]');
      ta.value = `Hola, me interesa la propiedad: ${p.titulo} (${p.ciudad}${p.barrio? ', '+p.barrio:''}). ¿Podemos agendar visita?`;
      document.getElementById('contacto').scrollIntoView({behavior:'smooth'});
    }

    async function share(id){
      const p = PROPS.find(x=>x.id===id);
      const url = location.href.split('#')[0] + `#prop-${id}`;
      try{ await navigator.share({title:p.titulo,text:`${p.titulo} – ${fmtEUR(p.precio)}`,url}); }
      catch(e){ navigator.clipboard.writeText(url); alert('Enlace copiado'); }
    }

    function submitted(e){
      e.preventDefault();
      const form = e.target;
      const data = new FormData(form);
      fetch(form.action,{method:'POST',body:data,headers:{'Accept':'application/json'}})
        .then(r=> r.ok ? r.json(): Promise.reject(r))
        .then(()=>{ document.getElementById('msg').textContent='¡Gracias! Te contactaremos pronto.'; form.reset(); })
        .catch(()=>{ document.getElementById('msg').textContent='No se pudo enviar. Escríbenos por WhatsApp o email.'; });
    }

    // Schema.org (SEO básico)
    const org = {
      '@context':'https://schema.org',
      '@type':'RealEstateAgent',
      name:'Inmobiliaria Palancas',
      url:location.origin,
      areaServed:'España',
      sameAs:['https://wa.me/34633102934']
    };
    const json = document.createElement('script');
    json.type='application/ld+json';
    json.textContent = JSON.stringify(org);
    document.body.appendChild(json);

    document.getElementById('year').textContent = new Date().getFullYear();
    filtrar();
  </script>
  <div class="schema" aria-hidden="true"></div>
  
  <!-- Chat interno (envía aviso al email vía Formspree) -->
  <style>
    .chat-fab{position:fixed;right:18px;bottom:18px;background:linear-gradient(90deg,var(--brand),var(--accent));color:#0b0d11;border:none;border-radius:999px;padding:12px 16px;font-weight:800;cursor:pointer;box-shadow:0 8px 24px rgba(0,0,0,.35)}
    .chat-panel{position:fixed;right:18px;bottom:74px;width:320px;max-height:70vh;background:var(--card);border:1px solid #1f2530;border-radius:16px;display:none;flex-direction:column;overflow:hidden}
    .chat-head{padding:10px 12px;border-bottom:1px solid #1f2530;font-weight:700}
    .chat-log{padding:12px;display:flex;flex-direction:column;gap:8px;overflow:auto}
    .chat-msg{background:#0f1319;border:1px solid #2a3241;padding:8px 10px;border-radius:12px;max-width:85%}
    .chat-me{align-self:flex-end;background:rgba(147,197,253,.1)}
    .chat-form{display:flex;gap:8px;padding:10px;border-top:1px solid #1f2530}
    .chat-form input{flex:1;padding:10px 12px;border-radius:10px;border:1px solid #2a3241;background:#0f1319;color:var(--fg)}
    .chat-form button{padding:10px 12px;border-radius:10px;border:1px solid #264353;background:#0f1319;color:var(--fg)}
    .chat-meta{padding:8px 12px;color:var(--muted);font-size:.85rem}
  </style>
  <div class="chat-panel" id="chat">
    <div class="chat-head">Chat Palancas</div>
    <div class="chat-meta">Te respondemos por email. No usamos WhatsApp para este chat.</div>
    <div class="chat-log" id="chatLog"></div>
    <form class="chat-form" onsubmit="sendChat(event)">
      <input type="text" id="chatName" placeholder="Tu nombre" required>
      <input type="email" id="chatEmail" placeholder="Tu email" required>
      <input type="text" id="chatInput" placeholder="Escribe tu mensaje" required>
      <button>Enviar</button>
    </form>
  </div>
  <button class="chat-fab" onclick="toggleChat()">Chat</button>
  <script>
    function toggleChat(){
      const el = document.getElementById('chat');
      el.style.display = el.style.display==='flex' ? 'none' : 'flex';
      if(el.style.display==='flex'){ setTimeout(()=> el.querySelector('#chatInput').focus(), 50); }
    }
    function addMsg(txt,me=false){
      const log = document.getElementById('chatLog');
      const div = document.createElement('div');
      div.className = 'chat-msg' + (me?' chat-me':'');
      div.textContent = txt;
      log.appendChild(div);
      log.scrollTop = log.scrollHeight;
    }
    function sendChat(e){
      e.preventDefault();
      const name = document.getElementById('chatName').value.trim();
      const email = document.getElementById('chatEmail').value.trim();
      const msg = document.getElementById('chatInput').value.trim();
      if(!name||!email||!msg) return;
      addMsg(msg,true);
      document.getElementById('chatInput').value='';
      // Enviar a Formspree como si fuera el formulario principal
      const data = new FormData();
      data.append('nombre', name);
      data.append('email', email);
      data.append('mensaje', msg);
      data.append('origen', 'chat');
      fetch('https://formspree.io/f/xqayvavw',{method:'POST',body:data,headers:{'Accept':'application/json'}})
        .then(r=>r.ok?r.json():Promise.reject(r))
        .then(()=> addMsg('Gracias, te responderemos por email en breve.'))
        .catch(()=> addMsg('No pudimos enviar el mensaje. Prueba el formulario o escríbenos a info@palancas.es'));
    }
  </script>
</body>
</html>
