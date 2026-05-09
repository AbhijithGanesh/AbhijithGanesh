<!-- markdownlint-disable MD033 MD041 MD045 -->

```aura width=1200 height=620
<div style={{
  width: '100%', height: '100%', display: 'flex',
  background: 'linear-gradient(135deg, #050505 0%, #0d0a07 55%, #1a0f05 100%)',
  fontFamily: 'Inter', color: '#f5efe6', padding: '72px 80px',
  position: 'relative',
}}>
  <svg
    width="1200" height="620"
    viewBox="0 0 1200 620"
    style={{ position: 'absolute', top: 0, left: 0, display: 'flex' }}
    xmlns="http://www.w3.org/2000/svg"
  >
    <style>{`
      @keyframes flickerCorner { 0%,100% { opacity: 1; } 50% { opacity: 0.35; } }
      @keyframes sweep { 0% { transform: translateX(-360px); } 100% { transform: translateX(1500px); } }
      #c1 { animation: flickerCorner 3s ease-in-out infinite; }
      #c2 { animation: flickerCorner 3s ease-in-out 0.4s infinite; }
      #c3 { animation: flickerCorner 3s ease-in-out 0.8s infinite; }
      #c4 { animation: flickerCorner 3s ease-in-out 1.2s infinite; }
      #sweep-band { animation: sweep 6s ease-in-out infinite; }
    `}</style>
    <defs>
      <linearGradient id="sweepGrad" x1="0" y1="0" x2="1" y2="0">
        <stop offset="0%" stopColor="#ffb547" stopOpacity="0"/>
        <stop offset="50%" stopColor="#ffb547" stopOpacity="0.14"/>
        <stop offset="100%" stopColor="#ffb547" stopOpacity="0"/>
      </linearGradient>
    </defs>
    <rect id="sweep-band" x="-360" y="0" width="360" height="620" fill="url(#sweepGrad)"/>
    <g id="c1" stroke="#ffb547" strokeWidth="2" fill="none">
      <path d="M 36 72 L 36 36 L 72 36"/>
    </g>
    <g id="c2" stroke="#ffb547" strokeWidth="2" fill="none">
      <path d="M 1128 36 L 1164 36 L 1164 72"/>
    </g>
    <g id="c3" stroke="#ffb547" strokeWidth="2" fill="none">
      <path d="M 36 548 L 36 584 L 72 584"/>
    </g>
    <g id="c4" stroke="#ffb547" strokeWidth="2" fill="none">
      <path d="M 1128 584 L 1164 584 L 1164 548"/>
    </g>
  </svg>

  {/* Single-column identity, full width */}
  <div style={{ display: 'flex', flexDirection: 'column', flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', alignItems: 'center', gap: 18 }}>
      <div style={{ display: 'flex', width: 36, height: 1, background: '#ffb547' }} />
      <div style={{ display: 'flex', fontSize: 13, color: '#ffb547', letterSpacing: 6, fontWeight: 500, textTransform: 'uppercase' }}>
        Founding AI Engineer
      </div>
    </div>

    <div style={{ display: 'flex', flexDirection: 'column', marginTop: 36 }}>
      <div style={{ display: 'flex', fontSize: 152, fontWeight: 900, lineHeight: 0.94, letterSpacing: -7 }}>
        Abhijith
      </div>
      <div style={{ display: 'flex', fontSize: 152, fontWeight: 900, lineHeight: 1, letterSpacing: -7, color: '#ffb547', fontStyle: 'italic', marginTop: 6 }}>
        Ganesh.
      </div>
    </div>

    <div style={{ display: 'flex', marginTop: 44, fontSize: 20, color: '#d8d2c4', maxWidth: 760, lineHeight: 1.55, fontWeight: 300 }}>
      Production LLM systems, end-to-end — retrieval, document forensics, and agentic automation, wired to cloud-native infra that doesn't fall over.
    </div>

    <div style={{ display: 'flex', alignItems: 'center', marginTop: 44, fontSize: 12, letterSpacing: 3, color: '#7a7468', textTransform: 'uppercase' }}>
      <div style={{ display: 'flex' }}>Chennai, IN</div>
      <div style={{ display: 'flex', width: 4, height: 4, borderRadius: 4, background: '#3a3a3a', margin: '0 18px' }} />
      <div style={{ display: 'flex' }}>CKA · AWS · GCP · Azure</div>
      <div style={{ display: 'flex', width: 4, height: 4, borderRadius: 4, background: '#3a3a3a', margin: '0 18px' }} />
      <div style={{ display: 'flex', color: '#ffb547' }}>Open for work</div>
    </div>
  </div>
</div>
```

<div style="background:#0a0a0a;padding:18px 0 6px 0;">

```aura width=220 height=44 link="mailto:work@abhijithganesh.com" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/gmail/EA4335"
  text="work@abhijithganesh.com"
  backgroundColor="#0a0a0a"
  textColor="#f5efe6"
  fontSize={11}
  width={220}
  height={44}
  iconSize="18"
  gradientStops={[
    { offset: '0%', color: '#ffb547' },
    { offset: '50%', color: '#0a0a0a' },
    { offset: '100%', color: '#ff7849' },
  ]}
/>
```

```aura width=170 height=44 link="https://abhijithganesh.com" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/safari/ffb547"
  text="abhijithganesh.com"
  backgroundColor="#0a0a0a"
  textColor="#f5efe6"
  fontSize={11}
  width={170}
  height={44}
  iconSize="18"
  gradientStops={[
    { offset: '0%', color: '#ffb547' },
    { offset: '100%', color: '#0a0a0a' },
  ]}
/>
```

```aura width=140 height=44 link="https://github.com/AbhijithGanesh" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/github/ffffff"
  text="GitHub"
  backgroundColor="#0a0a0a"
  textColor="#f5efe6"
  fontSize={12}
  width={140}
  height={44}
  iconSize="18"
/>
```

```aura width=180 height=44 link="https://www.credly.com/badges/1eb04f2a-d051-4db8-b3ab-f0df8c08de6d/linked_in_profile" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/kubernetes/ffb547"
  text="CKA Certified"
  backgroundColor="#0a0a0a"
  textColor="#f5efe6"
  fontSize={12}
  width={160}
  height={44}
  iconSize="18"
  gradientStops={[
    { offset: '0%', color: '#ffb547' },
    { offset: '100%', color: '#0a0a0a' },
  ]}
/>
```

</div>

```aura width=1200 height=760
<div style={{
  width: '100%', height: '100%', display: 'flex', flexDirection: 'column',
  background: 'linear-gradient(180deg, #0a0a0a 0%, #0f0a05 100%)', fontFamily: 'Inter', color: '#f5efe6', padding: '48px 56px',
  borderTop: '1px solid #1a1a1a', borderBottom: '1px solid #1a1a1a',
}}>
  <style>{`
    @keyframes pulseDot { 0%,100% { opacity: 1; } 50% { opacity: 0.3; } }
    @keyframes barGrow { 0% { transform: scaleX(0); } 100% { transform: scaleX(1); } }
    @keyframes cardRise { 0% { opacity: 0; transform: translateY(20px); } 100% { opacity: 1; transform: translateY(0); } }
    #live-dot { animation: pulseDot 1.2s ease-in-out infinite; }
    #card-0 { animation: cardRise 0.8s ease-out 0.0s both; }
    #card-1 { animation: cardRise 0.8s ease-out 0.15s both; }
    #card-2 { animation: cardRise 0.8s ease-out 0.30s both; }
    #bar-0, #bar-1, #bar-2 { transform-origin: left center; animation: barGrow 1s ease-out 0.5s both; }
  `}</style>

  {/* About */}
  <div style={{ display: 'flex' }}>
    <div style={{ display: 'flex', flexDirection: 'column', width: 280, paddingRight: 32, borderRight: '1px solid #222' }}>
      <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#666', textTransform: 'uppercase' }}>§ 01</div>
      <div style={{ display: 'flex', fontSize: 36, fontWeight: 900, marginTop: 12, lineHeight: 1, letterSpacing: -1 }}>About</div>
      <div style={{ display: 'flex', fontSize: 36, fontWeight: 200, fontStyle: 'italic', color: '#ffb547', lineHeight: 1, letterSpacing: -1 }}>me.</div>
      <div style={{ display: 'flex', marginTop: 24, width: 60, height: 2, background: '#ffb547' }} />
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', flex: 1, paddingLeft: 40, justifyContent: 'center' }}>
      <div style={{ display: 'flex', fontSize: 22, lineHeight: 1.55, color: '#e8e2d6', fontWeight: 300 }}>
        Founding AI engineer shipping production LLM systems end-to-end — retrieval pipelines, document forensics, and agentic automation — on cloud-native infrastructure.
      </div>
      <div style={{ display: 'flex', marginTop: 18, fontSize: 16, color: '#888', fontWeight: 400 }}>
        CKA-certified. Track record of measurable wins in latency, build speed, and reliability.
      </div>
      <div style={{ display: 'flex', marginTop: 22, fontSize: 12, letterSpacing: 4, color: '#ffb547', textTransform: 'uppercase' }}>
        → BASED IN CHENNAI, INDIA
      </div>
    </div>
  </div>

  {/* Divider */}
  <div style={{ display: 'flex', marginTop: 40, marginBottom: 40, height: 1, background: '#1f1f1f' }} />

  {/* Currently shipping */}
  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'flex-end' }}>
    <div style={{ display: 'flex', flexDirection: 'column' }}>
      <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#666', textTransform: 'uppercase' }}>§ 02 · IN PROGRESS</div>
      <div style={{ display: 'flex', flexDirection: 'column', marginTop: 8 }}>
        <div style={{ display: 'flex', fontSize: 56, fontWeight: 900, lineHeight: 1, letterSpacing: -2 }}>Currently</div>
        <div style={{ display: 'flex', fontSize: 56, fontWeight: 200, fontStyle: 'italic', color: '#ffb547', lineHeight: 1, letterSpacing: -2, marginTop: 4 }}>shipping</div>
      </div>
    </div>
    <div style={{ display: 'flex', fontSize: 14, color: '#ffb547', letterSpacing: 3, textTransform: 'uppercase', alignItems: 'center', gap: 8 }}>
      <div id="live-dot" style={{ display: 'flex', width: 10, height: 10, borderRadius: 10, background: '#ffb547' }} />
      <div style={{ display: 'flex' }}>LIVE</div>
    </div>
  </div>

  <div style={{ display: 'flex', marginTop: 28, gap: 18 }}>
    {[
      { n: '01', t: 'Retrieval Platform', d: 'LLM-backed retrieval over private corpora with grounded citations.' },
      { n: '02', t: 'Agent Runtime', d: 'LLM-driven agent automating machine-level tasks with remote multi-language code execution.' },
      { n: '03', t: 'CI/CD at Scale', d: 'Standardising CI/CD across 90+ repos. -60–80% failures. -50–70% build time.' },
    ].map((c, i) => (
      <div key={i} id={`card-${i}`} style={{
        display: 'flex', flexDirection: 'column', flex: 1, height: 220,
        background: '#111', border: '1px solid #1f1f1f', padding: 24,
        position: 'relative',
      }}>
        <div id={`bar-${i}`} style={{ display: 'flex', position: 'absolute', top: 0, left: 0, width: 60, height: 4, background: '#ffb547' }} />
        <div style={{ display: 'flex', fontSize: 12, letterSpacing: 3, color: '#ffb547' }}>{c.n}</div>
        <div style={{ display: 'flex', fontSize: 24, fontWeight: 800, marginTop: 14, lineHeight: 1.1 }}>{c.t}</div>
        <div style={{ display: 'flex', marginTop: 12, fontSize: 14, color: '#999', lineHeight: 1.5, fontWeight: 300 }}>{c.d}</div>
        <div style={{ display: 'flex', marginTop: 'auto', fontSize: 11, letterSpacing: 3, color: '#444', textTransform: 'uppercase' }}>STATUS: ACTIVE →</div>
      </div>
    ))}
  </div>
</div>
```

```aura width=1200 height=900
<div style={{
  width: '100%', height: '100%', display: 'flex', flexDirection: 'column',
  background: '#f5efe6', fontFamily: 'Inter', color: '#0a0a0a', padding: '52px 56px',
}}>
  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'flex-end', borderBottom: '2px solid #0a0a0a', paddingBottom: 18 }}>
    <div style={{ display: 'flex', flexDirection: 'column' }}>
      <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#888', textTransform: 'uppercase' }}>§ 03 · SERVICES</div>
      <div style={{ display: 'flex', flexDirection: 'column', marginTop: 8 }}>
        <div style={{ display: 'flex', fontSize: 64, fontWeight: 900, lineHeight: 1, letterSpacing: -3 }}>What I do for</div>
        <div style={{ display: 'flex', fontSize: 64, fontWeight: 200, fontStyle: 'italic', color: '#b45309', lineHeight: 1, letterSpacing: -3, marginTop: 6 }}>your business.</div>
      </div>
    </div>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: 3, color: '#888' }}>SIX DISCIPLINES →</div>
  </div>

  <div style={{ display: 'flex', marginTop: 28, flexWrap: 'wrap' }}>
    {[
      { n: '01', t: 'Idea to Production', d: 'Whiteboard to deployed system. End-to-end ownership.' },
      { n: '02', t: 'Cut Cloud Bills', d: 'Consolidate workloads, right-size compute, lease idle capacity.' },
      { n: '03', t: 'Ship Faster', d: 'Modernise CI/CD pipelines. Unblock developer velocity.' },
      { n: '04', t: 'AI That Works', d: 'RAG, agents, ML — grounded in your domain, not hype.' },
      { n: '05', t: 'Zero-Downtime Migrations', d: 'Stack modernisation across web, edge, and infra.' },
      { n: '06', t: 'Reliability', d: 'Observability, multi-cloud failover, real incident response.' },
    ].map((s, i) => (
      <div key={i} style={{
        display: 'flex', flexDirection: 'column', width: '33.333%', padding: '24px 24px 24px 0',
        borderRight: i % 3 === 2 ? 'none' : '1px solid #d4cfc4',
        borderBottom: i < 3 ? '1px solid #d4cfc4' : 'none',
        paddingLeft: i % 3 === 0 ? 0 : 24,
      }}>
        <div style={{ display: 'flex', alignItems: 'center', gap: 10 }}>
          <div style={{ display: 'flex', fontSize: 11, letterSpacing: 3, color: '#b45309', fontWeight: 700 }}>{s.n}</div>
          <div style={{ display: 'flex', flex: 1, height: 1, background: '#0a0a0a' }} />
        </div>
        <div style={{ display: 'flex', fontSize: 22, fontWeight: 800, marginTop: 12, lineHeight: 1.1, letterSpacing: -0.5 }}>{s.t}</div>
        <div style={{ display: 'flex', marginTop: 10, fontSize: 13, color: '#555', lineHeight: 1.5, fontWeight: 400 }}>{s.d}</div>
      </div>
    ))}
  </div>

  {/* Credentials */}
  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'baseline', marginTop: 36, borderTop: '2px solid #0a0a0a', paddingTop: 24 }}>
    <div style={{ display: 'flex', fontSize: 44, fontWeight: 900, letterSpacing: -2, lineHeight: 1 }}>
      Credentials.
    </div>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#888', textTransform: 'uppercase' }}>§ 04 · VERIFIED</div>
  </div>
  <div style={{ display: 'flex', marginTop: 22, gap: 12 }}>
    {[
      { i: 'CNCF', t: 'Certified Kubernetes Administrator', s: 'CKA' },
      { i: 'MS', t: 'Azure AI Fundamentals', s: 'AI-900' },
      { i: 'MS', t: 'Azure Fundamentals', s: 'AZ-900' },
      { i: 'AWS', t: 'Cloud Practitioner', s: 'CCP' },
      { i: 'GCP', t: 'Cloud Digital Leader', s: 'CDL' },
    ].map((c, i) => (
      <div key={i} style={{
        display: 'flex', flexDirection: 'column', flex: 1, padding: 18,
        background: '#ece5d8', borderTop: '3px solid #b45309',
      }}>
        <div style={{ display: 'flex', fontSize: 11, letterSpacing: 3, color: '#8a7a5e', fontWeight: 700 }}>{c.i}</div>
        <div style={{ display: 'flex', fontSize: 28, fontWeight: 900, marginTop: 8, color: '#b45309', letterSpacing: -1 }}>{c.s}</div>
        <div style={{ display: 'flex', marginTop: 8, fontSize: 12, color: '#555', lineHeight: 1.3, fontWeight: 400 }}>{c.t}</div>
      </div>
    ))}
  </div>
</div>
```

```aura width=1200 height=300
<div style={{
  width: '100%', height: '100%', display: 'flex', flexDirection: 'column',
  background: '#0a0a0a', fontFamily: 'Inter', color: '#f5efe6', padding: '40px 56px',
}}>
  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'baseline' }}>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#666', textTransform: 'uppercase' }}>§ 05 · STACK</div>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: 3, color: '#666' }}>40+ TOOLS · DAILY DRIVERS BELOW</div>
  </div>
  <div style={{ display: 'flex', marginTop: 14, fontSize: 36, fontWeight: 200, fontStyle: 'italic', color: '#ffb547', letterSpacing: -1 }}>
    Tools of the trade —
  </div>
  <div style={{ display: 'flex', flex: 1, marginTop: 18, flexWrap: 'wrap', alignContent: 'flex-start' }}>
    {[
      'Python','TypeScript','Go','Rust','C++','FastAPI','React','Next.js','Astro','Tailwind',
      'Kubernetes','Docker','Terraform','AWS','GCP','Azure','Cloudflare','Postgres','Redis','Kafka',
      'Prometheus','Grafana','PyTorch','GraphQL','Bun',
    ].map((t, i) => (
      <div key={i} style={{
        display: 'flex', padding: '6px 14px', margin: '0 8px 8px 0',
        border: '1px solid #2a2a2a', fontSize: 13, color: '#ddd',
        background: i % 5 === 0 ? '#1a1208' : '#111',
      }}>{t}</div>
    ))}
  </div>
</div>
```

```aura width=1200 height=240 link="mailto:work@abhijithganesh.com"
<div style={{
  width: '100%', height: '100%', display: 'flex',
  background: 'linear-gradient(90deg, #ffb547 0%, #ff7849 100%)',
  fontFamily: 'Inter', padding: '44px 56px', alignItems: 'center', justifyContent: 'space-between',
  position: 'relative', overflow: 'hidden',
}}>
  <svg width="1200" height="240" viewBox="0 0 1200 240" style={{ position: 'absolute', top: 0, left: 0, display: 'flex' }} xmlns="http://www.w3.org/2000/svg">
    <style>{`
      @keyframes ctaSweep { 0% { transform: translateX(-500px); } 100% { transform: translateX(1700px); } }
      #cta-band { animation: ctaSweep 4s ease-in-out infinite; }
    `}</style>
    <defs>
      <linearGradient id="ctaSweepGrad" x1="0" y1="0" x2="1" y2="0">
        <stop offset="0%" stopColor="#ffffff" stopOpacity="0"/>
        <stop offset="50%" stopColor="#ffffff" stopOpacity="0.4"/>
        <stop offset="100%" stopColor="#ffffff" stopOpacity="0"/>
      </linearGradient>
    </defs>
    <rect id="cta-band" x="-500" y="0" width="500" height="240" fill="url(#ctaSweepGrad)"/>
  </svg>
  <div style={{ display: 'flex', flexDirection: 'column' }}>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#0a0a0a', textTransform: 'uppercase' }}>§ END</div>
    <div style={{ display: 'flex', fontSize: 56, fontWeight: 900, color: '#0a0a0a', lineHeight: 1, marginTop: 8, letterSpacing: -2 }}>
      Let's build something
    </div>
    <div style={{ display: 'flex', fontSize: 56, fontWeight: 200, fontStyle: 'italic', color: '#0a0a0a', lineHeight: 1, letterSpacing: -2 }}>
      worth shipping.
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'flex-end' }}>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: 3, color: '#0a0a0a' }}>WRITE TO →</div>
    <div style={{ display: 'flex', fontSize: 26, fontWeight: 800, color: '#0a0a0a', marginTop: 8 }}>work@abhijithganesh.com</div>
    <div style={{ display: 'flex', marginTop: 14, padding: '10px 20px', background: '#0a0a0a', color: '#f5efe6', fontSize: 13, letterSpacing: 3, fontWeight: 700 }}>
      OPEN FOR COLLABORATIONS
    </div>
  </div>
</div>
```

<p align="center">
  <img src="http://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=AbhijithGanesh&theme=github_dark" width="80%" alt="profile summary"/>
</p>

<p align="center">
  <img src="http://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=AbhijithGanesh&theme=github_dark" height="200" alt="top languages by repo"/>
  <img src="http://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=AbhijithGanesh&theme=github_dark" height="200" alt="top languages by commit"/>
</p>
