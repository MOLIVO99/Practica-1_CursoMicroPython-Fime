<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Práctica 1 — MicroPython con ESP32</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;600&family=Sora:wght@400;500;600;700&display=swap');

  :root {
    --primary: #3fb950;
    --primary-glow: rgba(63, 185, 80, 0.15);
    --bg-dark: #0d1117;
    --bg-card: #161b22;
    --border: #30363d;
    --text-main: #e6edf3;
    --text-muted: #8b949e;
    --ai-accent: #d2a8ff;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'Sora', sans-serif;
    background: var(--bg-dark);
    color: var(--text-main);
    line-height: 1.6;
    overflow-x: hidden;
  }

  .container {
    max-width: 900px;
    margin: 0 auto;
    width: 100%;
    padding: 0 1.5rem;
  }

  /* Hero Section */
  .hero {
    background: linear-gradient(135deg, #0d1117 0%, #161b22 60%, #1a2332 100%);
    border-bottom: 1px solid var(--border);
    padding: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .hero::before {
    content: '';
    position: absolute;
    top: -60px; right: -60px;
    width: 300px; height: 300px;
    background: radial-gradient(circle, rgba(63, 185, 80, 0.1) 0%, transparent 70%);
    border-radius: 50%;
  }

  .badge {
    display: inline-block;
    background: rgba(63, 185, 80, 0.1);
    border: 1px solid rgba(63, 185, 80, 0.3);
    color: var(--primary);
    font-size: 11px;
    font-weight: 600;
    text-transform: uppercase;
    padding: 6px 14px;
    border-radius: 20px;
    margin-bottom: 1.5rem;
  }

  .hero h1 {
    font-size: clamp(2rem, 5vw, 2.5rem);
    font-weight: 700;
    line-height: 1.2;
    margin-bottom: 1rem;
  }

  .hero h1 span { color: var(--primary); }
  
  .hero p {
    font-size: 1.05rem;
    color: var(--text-muted);
    max-width: 600px;
  }

  .meta-row {
    display: flex;
    gap: 1rem;
    margin-top: 2rem;
    flex-wrap: wrap;
  }

  .meta-chip {
    display: flex;
    align-items: center;
    gap: 8px;
    font-size: 12px;
    color: var(--text-muted);
    background: var(--bg-card);
    padding: 6px 12px;
    border-radius: 6px;
    border: 1px solid var(--border);
  }

  .meta-chip .dot {
    width: 8px; height: 8px;
    border-radius: 50%;
    background: var(--primary);
  }

  /* Content */
  .content-section { padding: 3rem 0; }

  .section-label {
    font-size: 11px;
    font-weight: 700;
    color: var(--primary);
    text-transform: uppercase;
    letter-spacing: 0.1em;
    margin-bottom: 0.75rem;
    display: block;
  }

  h2 { margin-bottom: 1.5rem; font-size: 1.5rem; color: #f0f6fc; }

  .theory-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 1.75rem;
    margin-bottom: 2.5rem;
    color: #c9d1d9;
    font-size: 1rem;
  }

  .theory-card p { margin-bottom: 1rem; }
  .theory-card p:last-child { margin-bottom: 0; }
  .theory-card strong { color: #f0f6fc; }
  
  code.inline-code {
    background: var(--bg-dark);
    padding: 2px 6px;
    border-radius: 4px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.85em;
    color: #a5d6ff;
  }

  .concept-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1.25rem;
    margin-bottom: 3rem;
  }

  .card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 1.5rem;
    transition: border-color 0.2s;
  }

  .card:hover { border-color: var(--primary); transform: translateY(-2px); }

  .card-icon { font-size: 24px; margin-bottom: 0.8rem; display: block; }
  .card-title { font-family: 'JetBrains Mono', monospace; color: var(--primary); font-weight: 600; font-size: 0.9rem; margin-bottom: 0.4rem; }
  .card-text { font-size: 0.85rem; color: var(--text-muted); line-height: 1.5; }

  /* Code Blocks */
  .code-container {
    background: var(--bg-dark);
    border: 1px solid var(--border);
    border-radius: 12px;
    overflow: hidden;
    margin-bottom: 2.5rem;
  }

  .code-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.75rem 1.25rem;
    background: var(--bg-card);
    border-bottom: 1px solid var(--border);
  }

  .code-filename { font-family: 'JetBrains Mono', monospace; font-size: 0.8rem; color: var(--text-muted); }
  
  .actions { display: flex; gap: 8px; }
  
  .copy-btn {
    background: transparent;
    border: 1px solid var(--border);
    color: var(--text-muted);
    font-size: 11px;
    padding: 5px 12px;
    border-radius: 6px;
    cursor: pointer;
    font-family: 'Sora', sans-serif;
    transition: all 0.2s;
  }
  .copy-btn:hover { border-color: var(--primary); color: var(--primary); background: var(--primary-glow); }

  pre {
    padding: 1.5rem;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.85rem;
    line-height: 1.65;
    overflow-x: auto;
    color: var(--text-main);
  }

  /* Syntax */
  .kw { color: #ff7b72; } .fn { color: #d2a8ff; } .cm { color: #8b949e; font-style: italic; }
  .st { color: #a5d6ff; } .nm { color: #79c0ff; } .op { color: #ff7b72; }

  /* Connections/Wokwi */
  .wokwi-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 1.5rem;
    margin-bottom: 1.5rem;
  }

  .wokwi-card h3 {
    font-size: 0.95rem;
    margin-bottom: 0.8rem;
    display: flex;
    align-items: center;
    gap: 8px;
    color: #f0f6fc;
  }

  .wokwi-card h3::before {
    content: ''; width: 10px; height: 10px; background: var(--primary); border-radius: 50%;
  }

  .conn-list { list-style: none; }
  .conn-list li {
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.85rem;
    color: var(--text-muted);
    margin-bottom: 0.5rem;
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .conn-list li::before { content: '→'; color: var(--primary); font-size: 10px; }

  .pin-tag {
    background: var(--primary-glow);
    border: 1px solid rgba(63, 185, 80, 0.3);
    color: var(--primary);
    padding: 2px 7px;
    border-radius: 4px;
    font-size: 0.75rem;
  }

  /* Links */
  .link-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1rem;
    margin-bottom: 3rem;
  }

  .link-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    padding: 1.25rem;
    border-radius: 10px;
    text-decoration: none;
    transition: border-color 0.2s;
    cursor: pointer;
  }

  .link-card:hover { border-color: var(--primary); }
  .link-card .lc-label { font-size: 10px; color: var(--primary); font-weight: 600; text-transform: uppercase; letter-spacing: 0.1em; margin-bottom: 4px; }
  .link-card .lc-name { font-size: 0.9rem; color: #f0f6fc; font-weight: 600; display: block; }
  .link-card .lc-url { font-size: 0.75rem; color: var(--text-muted); margin-top: 0.2rem; font-family: 'JetBrains Mono', monospace; }

  .divider { height: 1px; background: var(--border); margin: 3rem 0; }

  .challenge-box {
    background: linear-gradient(135deg, rgba(63, 185, 80, 0.08), rgba(63, 185, 80, 0.04));
    border: 1px solid rgba(63, 185, 80, 0.3);
    border-radius: 12px;
    padding: 1.5rem;
    margin-bottom: 2.5rem;
  }

  .challenge-box h3 { color: var(--primary); margin-bottom: 0.75rem; font-size: 0.95rem; display: flex; align-items: center; gap: 8px; }
  .challenge-box p { font-size: 0.88rem; color: #c9d1d9; line-height: 1.65; }

  #toast {
    position: fixed;
    bottom: 2rem;
    left: 50%;
    transform: translateX(-50%);
    background: var(--primary);
    color: var(--bg-dark);
    padding: 0.75rem 1.5rem;
    border-radius: 50px;
    font-weight: 600;
    font-size: 0.9rem;
    box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    opacity: 0;
    transition: opacity 0.3s, transform 0.3s;
    pointer-events: none;
    z-index: 1000;
  }

  #toast.show { opacity: 1; transform: translateX(-50%) translateY(-10px); }

  footer {
    text-align: center;
    padding: 3rem 1.5rem;
    border-top: 1px solid var(--border);
    color: var(--text-muted);
    font-size: 0.78rem;
  }
  
  @media (max-width: 600px) {
    .hero { padding: 3rem 1rem; }
    .content-section { padding: 2rem 1rem; }
  }
</style>
</head>
<body>

<div id="toast">¡Código copiado al portapapeles!</div>

<div class="hero">
  <div class="container">
    <div class="badge">Práctica 1 — MicroPython con ESP32</div>
    <h1>Fundamentos de <span>Hardware</span><br>y Lógica Digital</h1>
    <p>Aprende a controlar pines GPIO del ESP32 con MicroPython. Sin experiencia previa requerida. Usaremos el simulador Wokwi — no se necesita hardware físico.</p>
    
    <div class="meta-row">
      <div class="meta-chip"><div class="dot"></div> Nivel: cero experiencia</div>
      <div class="meta-chip"><div class="dot"></div> Plataforma: Wokwi Simulator</div>
      <div class="meta-chip"><div class="dot"></div> Proyecto: Semáforo secuencial</div>
      <div class="meta-chip"><div class="dot"></div> FIME UANL</div>
    </div>
  </div>
</div>

<div class="container content-section">

  <section>
    <span class="section-label">¿Qué es esto?</span>
    <h2>El ESP32 y MicroPython</h2>
    <div class="theory-card" id="theory1">
      <p>El <strong>ESP32</strong> es una pequeña computadora del tamaño de una tarjeta de presentación. No tiene pantalla ni teclado — su trabajo es <em>controlar cosas</em>: luces, motores, sensores, pantallas. Tiene "patas" físicas llamadas <strong>pines</strong>, y cada pin puede recibir o enviar una señal eléctrica.</p>
      <p><strong>MicroPython</strong> es Python adaptado para correr en microcontroladores como el ESP32. Si alguna vez escribiste una fórmula en Excel, ya tienes el concepto: le dices al programa qué hacer, paso a paso, y él lo ejecuta. La diferencia es que aquí, en vez de calcular celdas, estás encendiendo LEDs o leyendo sensores.</p>
      <p>En este curso no necesitas instalar nada en tu computadora. Usaremos <strong>Wokwi</strong>, un simulador en línea que replica el ESP32 y sus componentes de forma visual e interactiva.</p>
    </div>
  </section>

  <div class="divider"></div>

  <section>
    <span class="section-label">Conceptos clave</span>
    <h2>Vocabulario esencial de esta práctica</h2>
    <div class="concept-grid">
      <div class="card">
        <span class="card-icon">📌</span>
        <div class="card-title">GPIO</div>
        <div class="card-text">General Purpose Input/Output. Son los pines del ESP32 que podemos controlar con código. Cada uno puede actuar como interruptor de entrada o de salida.</div>
      </div>
      <div class="card">
        <span class="card-icon">💡</span>
        <div class="card-title">Pin.OUT</div>
        <div class="card-text">Le decimos al pin que su función es MANDAR señal. Es decir, nosotros controlamos si hay energía o no. Úsalo para controlar LEDs, buzzer, relés.</div>
      </div>
      <div class="card">
        <span class="card-icon">🔁</span>
        <div class="card-title">while True</div>
        <div class="card-text">Bucle infinito. Le dice al programa "repite esto para siempre". El semáforo nunca se detiene por sí solo — eso es exactamente lo que queremos.</div>
      </div>
      <div class="card">
        <span class="card-icon">⏱️</span>
        <div class="card-title">time.sleep()</div>
        <div class="card-text">Pausa el programa N segundos. time.sleep(1) espera 1 segundo. time.sleep(0.5) espera medio segundo. Es el "temporizador" del semáforo.</div>
      </div>
      <div class="card">
        <span class="card-icon">🟢</span>
        <div class="card-title">led.on()</div>
        <div class="card-text">Manda energía al pin — enciende el LED. Equivale a subir el switch de la luz. El pin pasa a nivel ALTO (3.3V).</div>
      </div>
      <div class="card">
        <span class="card-icon">⚫</span>
        <div class="card-title">led.off()</div>
        <div class="card-text">Corta la energía al pin — apaga el LED. El pin pasa a nivel BAJO (0V). Siempre apaga el color anterior antes de prender el siguiente.</div>
      </div>
      <div class="card">
        <span class="card-icon">⚙️</span>
        <div class="card-title">def función()</div>
        <div class="card-text">Una función es un bloque de código al que le pones nombre para reutilizarlo. apagar_todos() agrupa 3 líneas en una sola instrucción.</div>
      </div>
      <div class="card">
        <span class="card-icon">🖨️</span>
        <div class="card-title">print()</div>
        <div class="card-text">Muestra texto en la consola del simulador. No hace nada en el hardware — es una herramienta de diagnóstico para saber qué está haciendo el programa.</div>
      </div>
    </div>
  </section>

  <div class="divider"></div>

  <section>
    <span class="section-label">Código 1 de 2</span>
    <h2>LED parpadeando — el "Hola Mundo" de la electrónica</h2>
    <div class="theory-card" id="theory2">
      <p>Antes de construir el semáforo completo, vamos a dominar lo más básico: <strong>un LED que parpadea en bucle infinito</strong>. Este código introduce los tres elementos que todo programa de MicroPython para hardware va a tener: importar librerías, definir un pin como salida, y controlar el tiempo.</p>
      <p>Experimenta cambiando el valor de <code class="inline-code">time.sleep()</code> — si pones <code class="inline-code">0.1</code> el LED parpadeará muy rápido; si pones <code class="inline-code">2</code> será muy lento. Ese número es tu primer parámetro configurable.</p>
    </div>

    <div class="wokwi-card">
      <h3>Conexiones en Wokwi — Código 1</h3>
      <ul class="conn-list">
        <li>ESP32 <span class="pin-tag">GND</span> → resistencia (220Ω) → cátodo del LED (pata corta)</li>
        <li>ESP32 <span class="pin-tag">Pin 2</span> → ánodo del LED (pata larga)</li>
      </ul>
    </div>

    <div class="code-container">
      <div class="code-nav">
        <span class="code-filename">semaforo_codigo1_led_parpadeante.py</span>
        <button class="copy-btn" onclick="copyCode('code1')">Copiar</button>
      </div>
<pre id="code1"><span class="cm"># ============================================================</span>
<span class="cm"># CÓDIGO 1: Un LED que parpadea para siempre</span>
<span class="cm"># Práctica 1 — MicroPython con ESP32 | FIME UANL</span>
<span class="cm"># ============================================================</span>

<span class="cm"># Importamos las herramientas que necesitamos</span>
<span class="kw">from</span> machine <span class="kw">import</span> Pin   <span class="cm"># "Pin" nos permite hablarle a los pines del ESP32</span>
<span class="kw">import</span> time               <span class="cm"># "time" nos permite hacer pausas en el programa</span>

<span class="cm"># Creamos la variable "led" que representa el pin 2 configurado como SALIDA</span>
<span class="cm"># Pin.OUT = nosotros mandamos la señal (no la recibimos)</span>
<span class="nm">led</span> <span class="op">=</span> <span class="fn">Pin</span>(<span class="nm">2</span>, Pin.OUT)

<span class="cm"># Este bucle se repite PARA SIEMPRE (hasta apagar el ESP32)</span>
<span class="kw">while</span> <span class="nm">True</span>:

    led.<span class="fn">on</span>()            <span class="cm"># Prendemos el LED — mandamos energía al pin 2</span>
    time.<span class="fn">sleep</span>(<span class="nm">0.5</span>)   <span class="cm"># Esperamos medio segundo (puedes cambiar este número)</span>

    led.<span class="fn">off</span>()           <span class="cm"># Apagamos el LED — cortamos la energía del pin 2</span>
    time.<span class="fn">sleep</span>(<span class="nm">0.5</span>)   <span class="cm"># Esperamos otro medio segundo</span>

    <span class="cm"># ... y vuelve a empezar desde led.on()</span></pre>
    </div>
  </section>

  <div class="divider"></div>

  <section>
    <span class="section-label">Código 2 de 2 — Proyecto</span>
    <h2>Semáforo de Control Secuencial</h2>
    <div class="theory-card" id="theory3">
      <p>Ahora escalamos a <strong>3 LEDs trabajando en secuencia</strong>. El principio es el mismo que el código anterior, pero ahora tenemos que coordinar: antes de prender el siguiente color, hay que apagar el anterior. Para esto creamos la función <code class="inline-code">apagar_todos()</code>.</p>
      <p>Una <strong>función</strong> es un bloque de código con nombre propio. En vez de repetir tres líneas de <code class="inline-code">.off()</code> cada vez que cambiamos de color, simplemente llamamos a <code class="inline-code">apagar_todos()</code>. Esto hace el código más limpio, más corto y más fácil de leer.</p>
      <p>También usamos <code class="inline-code">print()</code> para mostrar mensajes en la consola del simulador. Aunque no hace nada en el hardware, es muy útil para saber en qué fase está el semáforo mientras lo desarrollamos.</p>
    </div>

    <div class="wokwi-card">
      <h3>Conexiones en Wokwi — Código 2</h3>
      <ul class="conn-list">
        <li>LED verde → <span class="pin-tag">Pin 18</span> + resistencia 220Ω a GND</li>
        <li>LED amarillo → <span class="pin-tag">Pin 19</span> + resistencia 220Ω a GND</li>
        <li>LED rojo → <span class="pin-tag">Pin 21</span> + resistencia 220Ω a GND</li>
        <li>Todos los cátodos (pata corta) van a cualquier pin <span class="pin-tag">GND</span> del ESP32</li>
      </ul>
    </div>

    <div class="code-container">
      <div class="code-nav">
        <span class="code-filename">semaforo_codigo2_secuencial.py</span>
        <button class="copy-btn" onclick="copyCode('code2')">Copiar</button>
      </div>
<pre id="code2"><span class="cm"># ============================================================</span>
<span class="cm"># CÓDIGO 2: Semáforo de Control Secuencial</span>
<span class="cm"># Práctica 1 — MicroPython con ESP32 | FIME UANL</span>
<span class="cm"># Proyecto: Verde → Amarillo → Rojo → repetir</span>
<span class="cm"># ============================================================</span>

<span class="cm"># Importamos las herramientas necesarias</span>
<span class="kw">from</span> machine <span class="kw">import</span> Pin
<span class="kw">import</span> time

<span class="cm"># ── DEFINIMOS UN PIN PARA CADA COLOR DEL SEMÁFORO ────────────</span>
<span class="nm">led_verde</span>    <span class="op">=</span> <span class="fn">Pin</span>(<span class="nm">18</span>, Pin.OUT)   <span class="cm"># LED verde    → conectado al pin 18</span>
<span class="nm">led_amarillo</span> <span class="op">=</span> <span class="fn">Pin</span>(<span class="nm">19</span>, Pin.OUT)   <span class="cm"># LED amarillo → conectado al pin 19</span>
<span class="nm">led_rojo</span>     <span class="op">=</span> <span class="fn">Pin</span>(<span class="nm">21</span>, Pin.OUT)   <span class="cm"># LED rojo     → conectado al pin 21</span>


<span class="cm"># ── FUNCIÓN: apagar los 3 LEDs de un solo golpe ──────────────</span>
<span class="cm"># La usamos antes de prender cada nuevo color</span>
<span class="cm"># Así nos aseguramos de que nunca queden 2 colores prendidos a la vez</span>
<span class="kw">def</span> <span class="fn">apagar_todos</span>():
    led_verde.<span class="fn">off</span>()
    led_amarillo.<span class="fn">off</span>()
    led_rojo.<span class="fn">off</span>()


<span class="cm"># ── SEMÁFORO EN BUCLE INFINITO ───────────────────────────────</span>
<span class="fn">print</span>(<span class="st">"Semáforo iniciado correctamente..."</span>)

<span class="kw">while</span> <span class="nm">True</span>:

    <span class="cm"># ── FASE 1: VERDE — Puedes pasar ──</span>
    <span class="fn">apagar_todos</span>()          <span class="cm"># Primero apagamos todo</span>
    led_verde.<span class="fn">on</span>()           <span class="cm"># Luego prendemos el verde</span>
    <span class="fn">print</span>(<span class="st">"VERDE  → Puedes pasar"</span>)
    time.<span class="fn">sleep</span>(<span class="nm">5</span>)            <span class="cm"># El verde dura 5 segundos</span>

    <span class="cm"># ── FASE 2: AMARILLO — Prepárate para parar ──</span>
    <span class="fn">apagar_todos</span>()
    led_amarillo.<span class="fn">on</span>()
    <span class="fn">print</span>(<span class="st">"AMARILLO → Prepárate para parar"</span>)
    time.<span class="fn">sleep</span>(<span class="nm">2</span>)            <span class="cm"># El amarillo dura 2 segundos</span>

    <span class="cm"># ── FASE 3: ROJO — Alto total ──</span>
    <span class="fn">apagar_todos</span>()
    led_rojo.<span class="fn">on</span>()
    <span class="fn">print</span>(<span class="st">"ROJO   → Alto total"</span>)
    time.<span class="fn">sleep</span>(<span class="nm">5</span>)            <span class="cm"># El rojo dura 5 segundos</span>

    <span class="cm"># ... y vuelve al verde automáticamente</span></pre>
    </div>
  </section>

  <div class="divider"></div>

  <section>
    <span class="section-label">Reto para casa</span>
    <div class="challenge-box">
      <h3>⚡ Desafío opcional</h3>
      <p>¿Puedes hacer que el LED amarillo <strong>parpadee 3 veces</strong> antes de pasar al rojo, en lugar de quedarse encendido fijo? Tip: necesitarás un bucle <code class="inline-code">for</code> dentro del bucle <code class="inline-code">while</code>. En la próxima clase lo revisamos.</p>
    </div>
  </section>

  <section>
    <span class="section-label">Links</span>
    <h2>Recursos de la práctica</h2>
    <div class="link-grid">
      <div class="link-card" onclick="openLink('https://wokwi.com')">
        <div class="lc-label">Simulador</div>
        <div class="lc-name">Wokwi — ESP32 Online</div>
        <div class="lc-url">wokwi.com</div>
      </div>
      <div class="link-card" onclick="openLink('https://docs.micropython.org/en/latest/library/machine.Pin.html')">
        <div class="lc-label">Documentación</div>
        <div class="lc-name">MicroPython — machine.Pin</div>
        <div class="lc-url">docs.micropython.org</div>
      </div>
      <div class="link-card" onclick="openLink('https://docs.micropython.org/en/latest/library/time.html')">
        <div class="lc-label">Documentación</div>
        <div class="lc-name">MicroPython — time</div>
        <div class="lc-url">docs.micropython.org</div>
      </div>
    </div>
  </section>

</div>

<footer class="footer">
  Curso MicroPython con ESP32 · FIME UANL · Práctica 1
</footer>

<script>
  const apiKey = ""; // La API key se inyecta automáticamente en el entorno
  const MODEL_TEXT = "gemini-2.5-flash-preview-09-2025";
  const MODEL_TTS = "gemini-2.5-flash-preview-tts";

  function openLink(url) {
    window.open(url, '_blank');
  }

  function copyCode(id) {
    const codeElement = document.getElementById(id);
    const text = codeElement.innerText || codeElement.textContent;
    
    const textArea = document.createElement("textarea");
    textArea.value = text;
    textArea.style.position = "fixed";
    textArea.style.left = "-9999px";
    textArea.style.top = "0";
    document.body.appendChild(textArea);
    textArea.focus();
    textArea.select();
    
    try {
      const successful = document.execCommand('copy');
      if (successful) showToast();
    } catch (err) {
      console.error('Error al copiar', err);
    }
    
    document.body.removeChild(textArea);
  }

  function showToast() {
    const toast = document.getElementById('toast');
    toast.classList.add('show');
    setTimeout(() => { toast.classList.remove('show'); }, 2500);
  }
</script>

</body>
</html>
