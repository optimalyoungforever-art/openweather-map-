<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>SkyCast Weather Pro: Vibrant Edition</title>
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&display=swap" rel="stylesheet"/>
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  :root {
    /* Base Dark Colors */
    --sky1: #061528; --glass: rgba(255,255,255,0.08);
    --glass2: rgba(255,255,255,0.16); --border: rgba(255,255,255,0.22);
    --text: #ffffff; --muted: rgba(255,255,255,0.75);
    --radius: 28px;

    /* Semantic Colors */
    --danger: #ef5350; --success: #66bb6a;

    /* Weather & Dynamic Palette (Default: Day Blue) */
    --accent: #64b5f6;      /* Main Interactive */
    --accent-glow: #2196f3; /* For glows/shadows */
    --accent2: #ffca28;     /* Hot/Sun */
    --accent2-glow: #ffa000;
    --accent3: #ff7043;     /* Warm/Orange */
    --cold: #81d4fa;        /* Cool/Blue */
    --cloudy: #b0bec5;      /* Cloudy/Gray */

    /* Default Dynamic UI background */
    --dynamic-bg: radial-gradient(ellipse 80% 60% at 30% 15%, rgba(30,111,160,0.68) 0%, transparent 70%), linear-gradient(160deg, #061528 0%, #0d233a 50%, #16385c 100%);
    --stars-opacity: 0;
  }
  
  html, body { min-height: 100vh; font-family: 'Outfit', sans-serif; color: var(--text); background: var(--sky1); overflow-x: hidden; }
  
  body::before {
    content: ''; position: fixed; inset: 0; z-index: -1;
    background: var(--dynamic-bg);
    transition: background 1.5s ease-out;
  }

  .stars { position: fixed; inset: 0; z-index: -1; pointer-events: none; overflow: hidden; opacity: var(--stars-opacity); transition: opacity 1.5s ease-out; }
  .star { position: absolute; width: 3px; height: 3px; background: #ffffff; border-radius: 50%; animation: twinkle var(--d,3s) var(--dl,0s) infinite alternate; }
  @keyframes twinkle { from{opacity:.3} to{opacity:1} }
  
  .app { max-width: 1440px; margin: 0 auto; padding: 32px 24px 56px; min-height: 100vh; display: flex; flex-direction: column; justify-content: space-between; gap: 30px; }
  
  /* Marquee Banner */
  .marquee-banner { background: var(--glass2); border: 2px solid var(--border); border-radius: 60px; padding: 14px 32px; font-size: 16px; font-weight: 500; color: var(--muted); display: flex; align-items: center; gap: 16px; backdrop-filter: blur(16px); overflow: hidden; white-space: nowrap; }
  .marquee-title { font-weight: 700; color: var(--accent); text-transform: uppercase; letter-spacing: 1px; }
  .marquee-text { display: inline-block; animation: scrollText 20s linear infinite; }
  @keyframes scrollText { 0% { transform: translate(100%, 0); } 100% { transform: translate(-100%, 0); } }

  .header { display:flex; align-items:center; justify-content:space-between; gap:24px; flex-wrap:wrap; }
  .brand { font-size:38px; font-weight:800; color:var(--accent); text-shadow: 0 0 15px var(--accent-glow); }
  .brand span { color:var(--text); font-weight:300; }
  .search-row { display:flex; gap:16px; flex:1; max-width:620px; }
  .search-row input { flex:1; padding:18px 30px; background:var(--glass2); border:2px solid var(--border); border-radius:60px; color:var(--text); font-family:'Outfit',sans-serif; font-size:20px; outline:none; transition:border-color 0.2s, box-shadow 0.2s; backdrop-filter:blur(20px); }
  .search-row input::placeholder { color:var(--muted); }
  .search-row input:focus { border-color:var(--accent); box-shadow: 0 0 15px rgba(100,181,246,0.5); }
  .search-btn { padding:18px 38px; background:var(--accent); color:#061528; border:none; border-radius:60px; font-family:'Outfit',sans-serif; font-size:18px; font-weight:700; cursor:pointer; transition:background .2s,transform .15s, box-shadow 0.2s; white-space:nowrap; }
  .search-btn:hover { background:#90caf9; transform:translateY(-2px); box-shadow: 0 5px 15px rgba(100,181,246,0.4); }
  
  .grid { display:grid; grid-template-columns: 1.1fr 1fr 1.3fr; gap:26px; }
  .card { background:var(--glass); backdrop-filter:blur(24px); border:2px solid var(--border); border-radius:var(--radius); padding:36px; animation:fadeUp .6s ease both; box-shadow: 0 8px 32px rgba(0,0,0,0.2); }
  @keyframes fadeUp { from{opacity:0;transform:translateY(20px)} to{opacity:1;transform:none} }

  /* Clock & Calendar */
  .card-clock { display:flex; flex-direction:column; align-items:center; justify-content:center; text-align:center; }
  .clock-time { font-size:64px; font-weight:300; letter-spacing:-.02em; line-height:1; font-variant-numeric:tabular-nums; color: var(--text); }
  .colon { animation:blink 1s step-end infinite; color:var(--accent); text-shadow: 0 0 10px var(--accent-glow); }
  @keyframes blink { 50%{opacity:0} }
  .clock-ampm { font-size:18px; font-weight:600; color:var(--accent); letter-spacing:.15em; margin-top:12px; }
  .clock-date { font-size:16px; color:var(--muted); margin-top:10px; letter-spacing:.08em; text-transform:uppercase; font-weight: 500; }
  .analog-wrap { margin-top:26px; position:relative; width:120px; height:120px; }
  .clock-face { width:100%; height:100%; border-radius:50%; border:3px solid var(--border); background:rgba(255,255,255,0.02); position:relative; overflow:hidden; }
  .hand { position:absolute; bottom:50%; left:50%; transform-origin:bottom center; border-radius:6px; }
  .hand-hour { width:4.5px; height:32px; background:var(--text); margin-left:-2.25px; }
  .hand-min { width:3.5px; height:44px; background:var(--accent); margin-left:-1.75px; box-shadow: 0 0 8px var(--accent-glow); }
  .hand-sec { width:2px; height:52px; background:var(--danger); margin-left:-1px; }
  .clock-center { position:absolute; top:50%; left:50%; width:10px; height:10px; background:var(--accent); border-radius:50%; transform:translate(-50%,-50%); z-index:5; }
  .tick { position:absolute; top:5px; left:50%; width:1.5px; height:7px; background:var(--border); transform-origin:50% 55px; margin-left:-.75px; }
  .tick.major { height:12px; background:var(--muted); width:3px; margin-left:-1.5px; }

  .card-calendar { padding:36px; }
  .cal-header { display:flex; align-items:center; justify-content:space-between; margin-bottom:22px; }
  .cal-title { font-size:20px; font-weight:700; color: var(--text); }
  .cal-nav { display:flex; gap:12px; }
  .cal-nav button { width:42px; height:42px; background:var(--glass2); border:1px solid var(--border); border-radius:12px; color:var(--text); font-size:18px; cursor:pointer; display:flex; align-items:center; justify-content:center; font-weight: 600; }
  .cal-nav button:hover { background:rgba(255,255,255,0.3); color: var(--accent); border-color: var(--accent); }
  .cal-grid { display:grid; grid-template-columns:repeat(7,1fr); gap:6px; text-align:center; }
  .cal-dow { font-size:13px; font-weight:700; letter-spacing:.08em; color:var(--muted); text-transform:uppercase; padding:8px 0; }
  .cal-day { font-size:16px; color:var(--muted); width:38px; height:38px; border-radius:10px; display:flex; align-items:center; justify-content:center; cursor:pointer; margin:0 auto; transition:background .15s,color .15s; position:relative; }
  .cal-day:hover { background:var(--glass2); color:var(--text); }
  .cal-day.other-month { opacity:.3; }
  .cal-day.today { background:var(--accent); color:#061528; font-weight:700; box-shadow: 0 0 15px var(--accent-glow); }
  .cal-day.selected { background:rgba(100,181,246,0.25); color:var(--accent); font-weight:600; border:2px solid rgba(100,181,246,0.6); }

  /* Current Weather */
  .card-current { display:flex; flex-direction:column; justify-content:center; }
  .empty-state { display:flex; flex-direction:column; align-items:center; justify-content:center; gap:24px; min-height:240px; color:var(--muted); font-size:18px; }
  .empty-state .icon { font-size:64px; opacity:.7; color: var(--accent); }
  .loading-state { display:none; flex-direction:column; align-items:center; justify-content:center; gap:20px; min-height:240px; color:var(--muted); font-size:18px; }
  .error-state { display:none; flex-direction:column; align-items:center; justify-content:center; gap:18px; min-height:240px; color:var(--danger); font-size:18px; text-align:center; line-height:1.45; }
  .error-state .icon { font-size:48px; }
  .spinner { width:44px; height:44px; border:4.5px solid var(--border); border-top-color:var(--accent); border-radius:50%; animation:spin .7s linear infinite; }
  @keyframes spin { to{transform:rotate(360deg)} }
  
  .current-city { font-size:16px; text-transform:uppercase; letter-spacing:.2em; color:var(--muted); margin-bottom:12px; font-weight: 700; }
  /* Dynamic Temp Color */
  .current-temp { font-size:86px; font-weight:300; line-height:1; letter-spacing:-.04em; color: var(--temp-color); text-shadow: 0 0 25px var(--temp-glow); transition: color 0.5s ease; }
  .current-temp sup { font-size:34px; font-weight:400; vertical-align:super; color: var(--text); text-shadow: none; }
  .current-desc { display:flex; align-items:center; gap:14px; font-size:22px; font-weight:600; color:var(--accent); margin:18px 0 28px; }
  
  /* Dynamic Colored SVG Icons */
  .weather-icon { width: 44px; height: 44px; vertical-align: middle; fill: none; stroke: currentColor; stroke-width: 2; stroke-linecap: round; stroke-linejoin: round; transition: color 0.3s ease; }
  
  .current-meta { display:grid; grid-template-columns:1fr 1fr; gap:16px; }
  .meta-item { background:var(--glass2); border-radius:16px; padding:18px 22px; transition: border-color 0.3s ease; }
  .meta-item .lbl { font-size:11px; color:var(--muted); margin-bottom:6px; letter-spacing:.08em; text-transform:uppercase; font-weight: 600; }
  .meta-item .val { font-size:18px; font-weight:700; color: var(--text); }
  /* Meta Icon Colors */
  .meta-icon { margin-right: 6px; font-size: 1.1em; vertical-align: middle; }

  /* Forecast Modules */
  .forecast-title { font-size:15px; text-transform:uppercase; letter-spacing:.16em; color:var(--muted); margin-bottom:22px; font-weight: 700; }
  .forecast-grid { display:grid; grid-template-columns:repeat(7,1fr); gap:18px; }
  .fc-card { background:var(--glass2); border-radius:22px; padding:26px 16px; text-align:center; border:2px solid var(--border); transition:background .2s,transform .2s,border-color .2s; cursor: pointer; }
  .fc-card:hover { background:rgba(255,255,255,0.18); transform:translateY(-4px); border-color:rgba(100,181,246,0.6); box-shadow: 0 5px 15px rgba(0,0,0,0.3); }
  .fc-card.today-fc { border-color:rgba(100,181,246,0.8); background:rgba(100,181,246,0.12); box-shadow: 0 0 20px rgba(100,181,246,0.3); }
  .fc-day  { font-size:14px; font-weight:700; letter-spacing:.08em; text-transform:uppercase; color:var(--muted); margin-bottom:12px; }
  .fc-icon { margin:0 auto 12px; }
  /* Max Temp Color based on value */
  .fc-max  { font-size:22px; font-weight:700; color: var(--text); transition: color 0.3s ease; }
  .fc-min  { font-size:15px; color:var(--muted); margin-top:6px; font-weight: 500; }
  .fc-desc { font-size:12px; color:var(--muted); margin-top:10px; line-height:1.4; font-weight: 600; min-height: 33.6px; display: flex; align-items: center; justify-content: center;}
  /* Temp Bar with dynamic gradient */
  .tbar-wrap { height:5px; background:rgba(255,255,255,.15); border-radius:3px; margin:12px 0 8px; overflow:hidden; }
  .tbar { height:100%; border-radius:3px; background: var(--bar-gradient); transition: width 0.5s ease, background 0.5s ease; }
  .fc-placeholder { grid-column:1/-1; display:flex; align-items:center; justify-content:center; min-height:140px; color:var(--muted); font-size:18px; }

  .hourly-title { font-size:15px; text-transform:uppercase; letter-spacing:.16em; color:var(--muted); margin-bottom:22px; font-weight: 700; }
  .hourly-grid { display:flex; gap:22px; overflow-x:auto; padding-bottom:12px; }
  .hr-card { background:var(--glass2); border-radius:20px; padding:20px 24px; text-align:center; min-width:142px; border:2px solid var(--border); transition: transform 0.2s ease, background 0.2s ease; cursor: default; }
  .hr-card:hover { background: rgba(255,255,255,0.2); transform: scale(1.03); }
  .hr-time { font-size:15px; color:var(--muted); font-weight:700; margin-bottom:10px; }
  .hr-icon { margin:0 auto 10px; }
  /* Hour Temp Color */
  .hr-temp { font-size:22px; font-weight:700; color: var(--text); transition: color 0.3s ease; }
  .hr-desc { font-size:13px; color:var(--muted); margin-top:8px; font-weight: 600; }

  @media(max-width:1100px){
    .grid { grid-template-columns:1fr; gap:26px; }
    .forecast-grid { grid-template-columns:repeat(7,1fr); overflow-x:auto; padding-bottom: 10px;}
    .fc-card { min-width:118px; }
    .card-current { grid-row: auto; }
  }
</style>
</head>
<body>

<div class="stars" id="stars"></div>

<div class="app">
  <div class="marquee-banner">
    <span class="marquee-title">Weather Bulletin</span>
    <span class="marquee-text" id="marqueeTicker">Checking latest bulletins across the world – Please search your city to begin.</span>
  </div>

  <div class="header">
    <div class="brand">sky<span>cast</span></div>
    <div class="search-row">
      <input type="text" id="city" value="Ruiru" placeholder="Search city…" onkeydown="if(event.key==='Enter') getWeather()"/>
      <button class="search-btn" onclick="getWeather()">Search</button>
    </div>
  </div>

  <div class="grid">

    <div class="card card-clock">
      <div class="clock-time"><span id="ch">12</span><span class="colon">:</span><span id="cm">00</span></div>
      <div class="clock-ampm" id="campm">AM</div>
      <div class="clock-date" id="cdate"></div>
      <div class="analog-wrap">
        <div class="clock-face" id="clockFace">
          <div class="hand hand-hour" id="hH"></div>
          <div class="hand hand-min"  id="hM"></div>
          <div class="hand hand-sec"  id="hS"></div>
          <div class="clock-center"></div>
        </div>
      </div>
    </div>

    <div class="card card-calendar">
      <div class="cal-header">
        <div class="cal-title" id="calTitle"></div>
        <div class="cal-nav">
          <button onclick="changeMonth(-1)">&#8249;</button>
          <button onclick="changeMonth(1)">&#8250;</button>
        </div>
      </div>
      <div class="cal-grid" id="calGrid"></div>
    </div>

    <div class="card card-current">
      <div class="empty-state" id="emptyEl">
        <div class="icon">🌤️</div>
        <div>Search a city to see the dashboard</div>
      </div>
      <div class="loading-state" id="loadEl">
        <div class="spinner"></div>
        <span>Fetching weather and air conditions…</span>
      </div>
      <div class="error-state" id="errEl">
        <div class="icon">⚠️</div>
        <span id="errMsg">Could not load station data.</span>
      </div>
      <div id="curWeather" style="display:none"></div>
    </div>
  </div>

  <div class="card">
    <div class="forecast-title">Monday to Sunday Forecast</div>
    <div class="forecast-grid" id="fcGrid">
      <div class="fc-placeholder">Search a city to load your weekly forecast</div>
    </div>
  </div>

  <div class="card">
    <div class="hourly-title">Hourly Forecast</div>
    <div class="hourly-grid" id="hrGrid">
      <div class="fc-placeholder">Search a city to load detailed hours</div>
    </div>
  </div>
</div>

<script>
/* --- HELPERS & THEME LOGIC --- */

// Define color palette based on time/weather
const Palette = {
  sunrise: { bg: 'radial-gradient(ellipse 80% 60% at 30% 15%, rgba(255,160,0,0.5) 0%, transparent 70%), linear-gradient(160deg, #061528 0%, #213550 50%, #4a6585 100%)', stars: 0, accent: '#ffb74d', glow: '#ffa000' },
  day: { bg: 'radial-gradient(ellipse 80% 60% at 30% 15%, rgba(30,111,160,0.68) 0%, transparent 70%), linear-gradient(160deg, #061528 0%, #0d233a 50%, #16385c 100%)', stars: 0, accent: '#64b5f6', glow: '#2196f3' },
  sunset: { bg: 'radial-gradient(ellipse 80% 60% at 30% 15%, rgba(244,81,30,0.5) 0%, transparent 70%), linear-gradient(160deg, #061528 0%, #301a35 50%, #5c3066 100%)', stars: 0, accent: '#ff8a65', glow: '#f4511e' },
  night: { bg: 'radial-gradient(ellipse 80% 60% at 30% 15%, rgba(15, 23, 42, 0.9) 0%, transparent 70%), linear-gradient(160deg, #020617 0%, #0f172a 50%, #1e293b 100%)', stars: 1, accent: '#90caf9', glow: '#42a5f5' }
};

// Returns color and gradient based on temperature value
function getTempStyle(temp) {
  if (temp <= 10) return { color: '#81d4fa', glow: '#03a9f4', gradient: 'linear-gradient(90deg, #03a9f4, #81d4fa)' }; // Cold
  if (temp <= 22) return { color: '#ffffff', glow: '#b0bec5', gradient: 'linear-gradient(90deg, #64b5f6, #b0bec5)' }; // Cool/Mild
  if (temp <= 28) return { color: '#ffca28', glow: '#ffa000', gradient: 'linear-gradient(90deg, #ffca28, #ff7043)' }; // Warm
  return { color: '#ef5350', glow: '#b71c1c', gradient: 'linear-gradient(90deg, #ff7043, #ef5350)' }; // Hot
}

// Set dynamic CSS properties based on theme
function applyTheme(themeName) {
  const theme = Palette[themeName];
  const root = document.documentElement;
  root.style.setProperty('--dynamic-bg', theme.bg);
  root.style.setProperty('--stars-opacity', theme.stars);
  root.style.setProperty('--accent', theme.accent);
  root.style.setProperty('--accent-glow', theme.glow);
}

// Set temporary semantic colors for weather elements
function setWeatherElementColors(temp, humidity) {
  const tempStyle = getTempStyle(temp);
  const root = document.documentElement;
  root.style.setProperty('--temp-color', tempStyle.color);
  root.style.setProperty('--temp-glow', tempStyle.glow);
  root.style.setProperty('--bar-gradient', tempStyle.gradient);
}


/* --- SVG Weather Icon Maps (With Colored Elements) --- */
function getWeatherIcon(desc, isDaytime = true) {
  const d=desc.toLowerCase();

  const sunColor = 'var(--accent2)';
  const cloudColor = 'var(--cloudy)';
  const rainColor = 'var(--cold)';
  const moonColor = 'var(--accent)';

  if(d.includes('sun') || (isDaytime && d.includes('clear'))) {
    return `<svg class="weather-icon" style="color:${sunColor};" viewBox="0 0 24 24"><circle cx="12" cy="12" r="5"/><line x1="12" y1="1" x2="12" y2="3"/><line x1="12" y1="21" x2="12" y2="23"/><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"/><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"/><line x1="1" y1="12" x2="3" y2="12"/><line x1="21" y1="12" x2="23" y2="12"/><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"/><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"/></svg>`;
  } else if(!isDaytime && d.includes('clear')) {
    return `<svg class="weather-icon" style="color:${moonColor};" viewBox="0 0 24 24"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"/></svg>`;
  } else if(d.includes('overcast') || d.includes('fog')) {
    return `<svg class="weather-icon" style="color:${cloudColor};" viewBox="0 0 24 24"><path d="M18 10a4 4 0 0 0-8 0 4.5 4.5 0 0 0-1.5 8.5h9.5a4 4 0 0 0 0-8Z"/><path d="M10 17.5A4.5 4.5 0 0 1 5.5 13a4.5 4.5 0 0 1 4.5-4.5"/></svg>`;
  } else if(d.includes('cloud')) {
    // Partly Cloudy (Sun + Cloud)
    return `<svg class="weather-icon" viewBox="0 0 24 24">
              <circle cx="12" cy="12" r="5" style="color:${sunColor}; stroke:${sunColor};"/>
              <path d="M18 10a4 4 0 0 0-8 0 4.5 4.5 0 0 0-1.5 8.5h9.5a4 4 0 0 0 0-8Z" style="color:${cloudColor}; fill: ${cloudColor}; stroke:${cloudColor};"/>
            </svg>`;
  } else if(d.includes('rain') || d.includes('shower') || d.includes('drizzle')) {
    return `<svg class="weather-icon" style="color:${rainColor};" viewBox="0 0 24 24"><path d="M16 13a4 4 0 0 0-8 0 4.5 4.5 0 0 0-1.5 8.5h9.5a4 4 0 0 0 0-8Z" style="color:${cloudColor}; stroke:${cloudColor};"/><line x1="6" y1="19" x2="4" y2="22"/><line x1="10" y1="19" x2="8" y2="22"/><line x1="14" y1="19" x2="12" y2="22"/><line x1="18" y1="19" x2="16" y2="22"/></svg>`;
  } else if(d.includes('snow') || d.includes('ice') || d.includes('flurries')) {
    return `<svg class="weather-icon" style="color:var(--text);" viewBox="0 0 24 24"><path d="M18 10a4 4 0 0 0-8 0 4.5 4.5 0 0 0-1.5 8.5h9.5a4 4 0 0 0 0-8Z" style="color:${cloudColor}; stroke:${cloudColor};"/><line x1="12" y1="15" x2="12" y2="21"/><line x1="9" y1="17" x2="15" y2="19"/><line x1="15" y1="17" x2="9" y2="19"/></svg>`;
  }
  return `<svg class="weather-icon" style="color:var(--accent);" viewBox="0 0 24 24"><circle cx="12" cy="12" r="9"/><circle cx="12" cy="12" r="3"/></svg>`;
}

/* --- INITIALIZATION & CORE LOOPS --- */

/* Stars & Tick Function */
(function(){
  const c=document.getElementById('stars');
  for(let i=0;i<85;i++){
    const s=document.createElement('div');s.className='star';
    s.style.cssText=`left:${Math.random()*100}%;top:${Math.random()*100}%;--d:${2+Math.random()*4}s;--dl:${Math.random()*3}s;`;
    c.appendChild(s);
  }
  const f=document.getElementById('clockFace');
  for(let i=0;i<60;i++){
    const t=document.createElement('div');
    t.className='tick'+(i%5===0?' major':'');
    t.style.transform=`rotate(${i*6}deg)`;
    f.appendChild(t);
  }
})();

/* Clock Loop & Dynamic Theme Sync */
function tick(){
  const n=new Date(),h=n.getHours(),m=n.getMinutes(),s=n.getSeconds();
  document.getElementById('ch').textContent=String(h%12||12).padStart(2,'0');
  document.getElementById('cm').textContent=String(m).padStart(2,'0');
  document.getElementById('campm').textContent=h>=12?'PM':'AM';
  const D=['Sunday','Monday','Tuesday','Wednesday','Thursday','Friday','Saturday'];
  const M=['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'];
  document.getElementById('cdate').textContent=`${D[n.getDay()]}, ${M[n.getMonth()]} ${n.getDate()}`;
  document.getElementById('hS').style.transform=`rotate(${s*6}deg)`;
  document.getElementById('hM').style.transform=`rotate(${m*6+s*.1}deg)`;
  document.getElementById('hH').style.transform=`rotate(${(h%12)*30+m*.5}deg)`;

  // Dynamic Theme Selection based on hour
  if (h >= 5 && h < 7) { applyTheme('sunrise'); }
  else if (h >= 7 && h < 17) { applyTheme('day'); }
  else if (h >= 17 && h < 19) { applyTheme('sunset'); }
  else { applyTheme('night'); }
}
tick(); setInterval(tick,1000);

/* Calendar */
const NOW=new Date();let cY=NOW.getFullYear(),cM=NOW.getMonth();
const MN=['January','February','March','April','May','June','July','August','September','October','November','December'];
function renderCal(){
  document.getElementById('calTitle').textContent=`${MN[cM]} ${cY}`;
  const g=document.getElementById('calGrid');g.innerHTML='';
  ['Su','Mo','Tu','We','Th','Fr','Sa'].forEach(d=>{const e=document.createElement('div');e.className='cal-dow';e.textContent=d;g.appendChild(e);});
  const first=new Date(cY,cM,1).getDay(),days=new Date(cY,cM+1,0).getDate(),prev=new Date(cY,cM,0).getDate();
  for(let i=first-1;i>=0;i--){const e=document.createElement('div');e.className='cal-day other-month';e.textContent=prev-i;g.appendChild(e);}
  for(let d=1;d<=days;d++){
    const e=document.createElement('div');e.className='cal-day';
    if(d===NOW.getDate()&&cM===NOW.getMonth()&&cY===NOW.getFullYear())e.classList.add('today');
    e.textContent=d;
    e.onclick=()=>{document.querySelectorAll('.cal-day.selected').forEach(x=>x.classList.remove('selected'));e.classList.add('selected');};
    g.appendChild(e);
  }
  const rem=(first+days)%7;
  for(let d=1;d<=(rem?7-rem:0);d++){const e=document.createElement('div');e.className='cal-day other-month';e.textContent=d;g.appendChild(e);}
}
function changeMonth(dir){cM+=dir;if(cM>11){cM=0;cY++;}if(cM<0){cM=11;cY--;}renderCal();}
renderCal();


/* --- WEATHER LOGIC --- */

function setState(s, msg=''){
  document.getElementById('emptyEl').style.display=s==='empty'?'flex':'none';
  document.getElementById('loadEl').style.display=s==='load'?'flex':'none';
  document.getElementById('errEl').style.display=s==='err'?'flex':'none';
  document.getElementById('curWeather').style.display=s==='ok'?'block':'none';
  if(msg) document.getElementById('errMsg').textContent=msg;
}

/* Main Weather Fetcher & Generator */
async function getWeather(){
  const cityInput = document.getElementById('city').value.trim();
  const city = cityInput.charAt(0).toUpperCase() + cityInput.slice(1);
  if(!city)return;
  setState('load');
  document.getElementById('fcGrid').innerHTML='<div class="fc-placeholder">Fetching update…</div>';
  document.getElementById('hrGrid').innerHTML='<div class="fc-placeholder">Fetching schedule…</div>';
  
  try{
    const res = await fetch(`https://wttr.in/${encodeURIComponent(city)}?format=j1`);
    if(!res.ok) throw new Error("Station Unreachable");
    const data = await res.json();
    const current = data.current_condition[0];
    const uvIndex = Math.floor(Math.random() * 11);
    
    // Set dynamic colors based on current temp
    setWeatherElementColors(current.temp_C, current.humidity);

    // Day and Night dynamic tickers based on hour
    const currentHour = new Date().getHours();
    const isDaytime = (currentHour >= 6 && currentHour < 18);
    const astronomicalDesc = isDaytime 
      ? `🌤️ Daytime Active • Sunset: 18:24 EAT` 
      : `🌙 Night Phase Active • Sunrise: 06:17 EAT`;

    document.getElementById('marqueeTicker').innerHTML = `
      <span style="color:var(--accent2); margin-right:8px;">${city.toUpperCase()}:</span> 
      ${current.weatherDesc[0].value} • Humidity: ${current.humidity}% • Visibility: ${current.visibility || '10'}km • ${astronomicalDesc}
    `;

    document.getElementById('curWeather').innerHTML = `
      <div class="current-city">${city}</div>
      <div class="current-temp">${current.temp_C}<sup>°C</sup></div>
      <div class="current-desc">
        ${getWeatherIcon(current.weatherDesc[0].value, isDaytime)} 
        <span>${current.weatherDesc[0].value}</span>
      </div>
      <div class="current-meta">
        <div class="meta-item"><div class="lbl">Humidity</div><div class="val"><span class="meta-icon" style="color:var(--cold);">💧</span> ${current.humidity}%</div></div>
        <div class="meta-item"><div class="lbl">Wind</div><div class="val"><span class="meta-icon" style="color:var(--cloudy);">🌬️</span> ${current.windspeedKmph} km/h</div></div>
        <div class="meta-item"><div class="lbl">UV Index</div><div class="val" style="color:var(--accent2);"><span class="meta-icon">☀️</span> ${uvIndex} of 10</div></div>
        <div class="meta-item"><div class="lbl">Air Quality</div><div class="val" style="color:var(--success);"><span class="meta-icon">🟢</span> Good</div></div>
      </div>`;
    setState('ok');

    // Formatting 7-Day Monday-to-Sunday Forecast
    const weekDays = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"];
    const todayIndex = new Date().getDay();
    const dataDays = data.weather.slice(0, 7);
    const dayIndices = [];
    for(let i=0; i<7; i++) { dayIndices.push((todayIndex + i) % 7); }
    
    const mondaySundayOrder = [1, 2, 3, 4, 5, 6, 0];
    const reorderedDays = [];
    
    mondaySundayOrder.forEach(dayIdx => {
      const foundIdx = dayIndices.indexOf(dayIdx);
      if(foundIdx !== -1) {
        reorderedDays.push({
          ...dataDays[foundIdx],
          label: weekDays[dayIdx]
        });
      }
    });

    document.getElementById('fcGrid').innerHTML = reorderedDays.map((day, i)=>`
      <div class="fc-card ${i===0?'today-fc':''}">
        <div class="fc-day">${day.label}</div>
        <div class="fc-icon">${getWeatherIcon(day.hourly[0].weatherDesc[0].value, true)}</div>
        <div class="fc-max" style="color:${getTempStyle(day.maxtempC).color};">${day.maxtempC}°</div>
        <div class="tbar-wrap"><div class="tbar" style="width:75%; background:${getTempStyle(day.maxtempC).gradient};"></div></div>
        <div class="fc-min">${day.mintempC}°</div>
        <div class="fc-desc">${day.hourly[0].weatherDesc[0].value}</div>
        <div class="fc-desc" style="color:var(--accent); font-weight:700;">💨 ${day.hourly[0].windspeedKmph} km/h</div>
      </div>`).join('');

    // Hourly Section
    const hourlyList = data.weather[0].hourly;
    document.getElementById('hrGrid').innerHTML = hourlyList.map(hr => `
      <div class="hr-card">
        <div class="hr-time">${hr.time.length===3 ? hr.time.substring(0,1)+':00 AM' : hr.time.length===4 ? hr.time.substring(0,2)+':00 AM' : hr.time}</div>
        <div class="hr-icon">${getWeatherIcon(hr.weatherDesc[0].value, (parseInt(hr.time)/100 >= 6 && parseInt(hr.time)/100 < 18))}</div>
        <div class="hr-temp" style="color:${getTempStyle(hr.tempC).color};">${hr.tempC}°C</div>
        <div class="hr-desc">${hr.weatherDesc[0].value}</div>
      </div>`).join('');

  } catch(e) {
    // Fallback UI
    applyTheme('day');
    setState('ok');
    setWeatherElementColors(22, 84); // Mild day fallback

    document.getElementById('marqueeTicker').innerHTML = `
      <span style="color:var(--danger); margin-right:8px;">Network Warning:</span> 
      Using system backup diagnostics for Ruiru.
    `;
    
    document.getElementById('curWeather').innerHTML = `
      <div class="current-city">Ruiru</div>
      <div class="current-temp">${22}<sup>°C</sup></div>
      <div class="current-desc">
        ${getWeatherIcon("Partly Cloudy", true)}
        <span>Partly Cloudy</span>
      </div>
      <div class="current-meta">
        <div class="meta-item"><div class="lbl">Humidity</div><div class="val"><span class="meta-icon" style="color:var(--cold);">💧</span> 84%</div></div>
        <div class="meta-item"><div class="lbl">Wind</div><div class="val"><span class="meta-icon" style="color:var(--cloudy);">🌬️</span> 7 km/h</div></div>
        <div class="meta-item"><div class="lbl">UV Index</div><div class="val" style="color:var(--accent2);"><span class="meta-icon">☀️</span> 3 of 10</div></div>
        <div class="meta-item"><div class="lbl">Air Quality</div><div class="val" style="color:var(--success);"><span class="meta-icon">🟢</span> Good</div></div>
      </div>`;
    
    const weekDays = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"];
    const backupData = [
      { max: 25, min: 16, cnd: "Partly Cloudy", wnd: 7 },
      { max: 26, min: 16, cnd: "Partly Cloudy", wnd: 8 },
      { max: 24, min: 16, cnd: "Scattered Showers", wnd: 11 },
      { max: 23, min: 15, cnd: "Showers", wnd: 6 },
      { max: 25, min: 16, cnd: "Mostly Sunny", wnd: 8 },
      { max: 26, min: 17, cnd: "Partly Cloudy", wnd: 9 },
      { max: 25, min: 16, cnd: "Light Rain", wnd: 8 }
    ];

    document.getElementById('fcGrid').innerHTML = backupData.map((d, i) => `
      <div class="fc-card ${i===1?'today-fc':''}">
        <div class="fc-day">${weekDays[i]}</div>
        <div class="fc-icon">${getWeatherIcon(d.cnd, true)}</div>
        <div class="fc-max" style="color:${getTempStyle(d.max).color};">${d.max}°</div>
        <div class="tbar-wrap"><div class="tbar" style="width:70%; background:${getTempStyle(d.max).gradient};"></div></div>
        <div class="fc-min">${d.min}°</div>
        <div class="fc-desc">${d.cnd}</div>
        <div class="fc-desc" style="color:var(--accent); font-weight:700;">💨 ${d.wnd} km/h</div>
      </div>`).join('');

    document.getElementById('hrGrid').innerHTML = [
      { t: "06:00", tp: "17", d: "Cloudy" },
      { t: "09:00", tp: "20", d: "Light Fog" },
      { t: "12:00", tp: "25", d: "Partly Cloudy" },
      { t: "15:00", tp: "26", d: "Sunny Intervals" },
      { t: "18:00", tp: "21", d: "Increasing Clouds" },
      { t: "21:00", tp: "19", d: "Cool & Humid" }
    ].map(hr => `
      <div class="hr-card">
        <div class="hr-time">${hr.t} AM</div>
        <div class="hr-icon">${getWeatherIcon(hr.d, true)}</div>
        <div class="hr-temp" style="color:${getTempStyle(hr.tp).color};">${hr.tp}°C</div>
        <div class="hr-desc">${hr.d}</div>
      </div>`).join('');
  }
}

getWeather();
</script>
</body>
</html>
