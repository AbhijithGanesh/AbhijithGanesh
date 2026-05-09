<!-- markdownlint-disable MD033 MD041 -->

```aura width=1200 height=520
<div style={{
  width: '100%', height: '100%', display: 'flex', flexDirection: 'column',
  background: 'linear-gradient(135deg, #050505 0%, #0d0d0f 60%, #1a0f05 100%)',
  fontFamily: 'Inter', color: '#f5efe6', padding: '52px 56px',
  position: 'relative',
}}>
  <style>{`
    @keyframes pulseDot { 0%,100% { opacity: 1; transform: scale(1); } 50% { opacity: 0.35; transform: scale(0.7); } }
    @keyframes sweep { 0% { transform: translateX(-120%); } 100% { transform: translateX(120%); } }
    @keyframes flickerCorner { 0%,100% { opacity: 1; } 50% { opacity: 0.4; } }
    @keyframes nameSlide { 0% { opacity: 0; transform: translateX(-24px); } 100% { opacity: 1; transform: translateX(0); } }
    @keyframes nameSlideR { 0% { opacity: 0; transform: translateX(24px); } 100% { opacity: 1; transform: translateX(0); } }
    #hero-name { animation: nameSlide 1.2s ease-out both; }
    #hero-name-2 { animation: nameSlideR 1.2s ease-out 0.2s both; }
    #hero-dot { animation: pulseDot 1.4s ease-in-out infinite; transform-origin: center; }
    #hero-c1, #hero-c2, #hero-c3, #hero-c4 { animation: flickerCorner 3s ease-in-out infinite; }
    #hero-c2 { animation-delay: 0.4s; }
    #hero-c3 { animation-delay: 0.8s; }
    #hero-c4 { animation-delay: 1.2s; }
    #hero-sweep { animation: sweep 4s ease-in-out infinite; }
  `}</style>
  {/* corner ticks */}
  <div id="hero-c1" style={{ position: 'absolute', top: 24, left: 24, width: 28, height: 28, borderTop: '2px solid #ffb547', borderLeft: '2px solid #ffb547', display: 'flex' }} />
  <div id="hero-c2" style={{ position: 'absolute', top: 24, right: 24, width: 28, height: 28, borderTop: '2px solid #ffb547', borderRight: '2px solid #ffb547', display: 'flex' }} />
  <div id="hero-c3" style={{ position: 'absolute', bottom: 24, left: 24, width: 28, height: 28, borderBottom: '2px solid #ffb547', borderLeft: '2px solid #ffb547', display: 'flex' }} />
  <div id="hero-c4" style={{ position: 'absolute', bottom: 24, right: 24, width: 28, height: 28, borderBottom: '2px solid #ffb547', borderRight: '2px solid #ffb547', display: 'flex' }} />
  {/* sweep light */}
  <div id="hero-sweep" style={{ position: 'absolute', top: 0, left: 0, width: '40%', height: '100%', display: 'flex', background: 'linear-gradient(90deg, transparent 0%, rgba(255,181,71,0.06) 50%, transparent 100%)' }} />

  {/* meta strip */}
  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center', fontSize: 13, letterSpacing: 4, color: '#888', textTransform: 'uppercase' }}>
    <div style={{ display: 'flex' }}>VOL. 01 · DOSSIER</div>
    <div style={{ display: 'flex' }}>CHENNAI · 13.0827° N</div>
    <div style={{ display: 'flex', color: '#ffb547', alignItems: 'center', gap: 8 }}>
      <div id="hero-dot" style={{ display: 'flex', width: 10, height: 10, borderRadius: 10, background: '#ffb547' }} />
      <div style={{ display: 'flex' }}>ONLINE</div>
    </div>
  </div>

  <div style={{ display: 'flex', flex: 1, alignItems: 'center', marginTop: 18 }}>
    <div style={{ display: 'flex', flexDirection: 'column' }}>
      <div style={{ display: 'flex', fontSize: 22, color: '#1af4ff', letterSpacing: 8, fontWeight: 300, textTransform: 'uppercase' }}>
        Founding AI Engineer
      </div>
      <div id="hero-name" style={{ display: 'flex', fontSize: 132, fontWeight: 900, lineHeight: 1, marginTop: 14, letterSpacing: -6 }}>
        ABHIJITH
      </div>
      <div id="hero-name-2" style={{ display: 'flex', fontSize: 132, fontWeight: 200, lineHeight: 1, letterSpacing: -6, color: '#ffb547', fontStyle: 'italic' }}>
        Ganesh.
      </div>
      <div style={{ display: 'flex', marginTop: 22, fontSize: 18, color: '#aaa', maxWidth: 760, lineHeight: 1.4 }}>
        Production LLM systems, end-to-end. Retrieval pipelines, document forensics, agentic automation — wired to cloud-native infrastructure that doesn't fall over.
      </div>
    </div>
  </div>

  <div style={{ display: 'flex', justifyContent: 'space-between', fontSize: 12, letterSpacing: 3, color: '#555', textTransform: 'uppercase', borderTop: '1px solid #2a2a2a', paddingTop: 14 }}>
    <div style={{ display: 'flex' }}>// CKA · CERTIFIED</div>
    <div style={{ display: 'flex' }}>// AZ-900 · AI-900 · AWS · GCP</div>
    <div style={{ display: 'flex' }}>// SHIP → MEASURE → REPEAT</div>
  </div>
</div>
```

```aura width=160 height=44 link="mailto:work@abhijithganesh.com" inline align=center
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
    { offset: '100%', color: '#1af4ff' },
  ]}
/>
```
```aura width=170 height=44 link="https://abhijithganesh.com" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/safari/1af4ff"
  text="abhijithganesh.com"
  backgroundColor="#0a0a0a"
  textColor="#f5efe6"
  fontSize={11}
  width={170}
  height={44}
  iconSize="18"
  gradientStops={[
    { offset: '0%', color: '#1af4ff' },
    { offset: '100%', color: '#0a0a0a' },
  ]}
/>
```
```aura width=120 height=44 link="https://linkedin.com/in/AbhijithGanesh14" inline align=center
<SocialMediaButton
  icon="https://cdn.jsdelivr.net/npm/simple-icons@v11/icons/linkedin.svg"
  text="LinkedIn"
  backgroundColor="#0a0a0a"
  textColor="#f5efe6"
  fontSize={12}
  width={120}
  height={44}
  iconSize="18"
/>
```
```aura width=140 height=44 link="https://github.com/AbhijithGanesh" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/github/ffffff"
  text="AbhijithGanesh"
  backgroundColor="#0a0a0a"
  textColor="#f5efe6"
  fontSize={12}
  width={150}
  height={44}
  iconSize="18"
/>
```
```aura width=180 height=44 link="https://www.credly.com/badges/1eb04f2a-d051-4db8-b3ab-f0df8c08de6d/linked_in_profile" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/kubernetes/326CE5"
  text="CKA Certified"
  backgroundColor="#0a0a0a"
  textColor="#f5efe6"
  fontSize={12}
  width={160}
  height={44}
  iconSize="18"
  gradientStops={[
    { offset: '0%', color: '#326CE5' },
    { offset: '100%', color: '#1af4ff' },
  ]}
/>
```

```aura width=1200 height=360
<div style={{
  width: '100%', height: '100%', display: 'flex',
  background: '#0a0a0a', fontFamily: 'Inter', color: '#f5efe6', padding: '48px 56px',
  borderTop: '1px solid #1a1a1a', borderBottom: '1px solid #1a1a1a',
}}>
  <div style={{ display: 'flex', flexDirection: 'column', width: 280, paddingRight: 32, borderRight: '1px solid #222' }}>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#666', textTransform: 'uppercase' }}>§ 01</div>
    <div style={{ display: 'flex', fontSize: 36, fontWeight: 900, marginTop: 12, lineHeight: 1, letterSpacing: -1 }}>About</div>
    <div style={{ display: 'flex', fontSize: 36, fontWeight: 200, fontStyle: 'italic', color: '#ffb547', lineHeight: 1, letterSpacing: -1 }}>the engineer.</div>
    <div style={{ display: 'flex', marginTop: 24, width: 60, height: 2, background: '#ffb547' }} />
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', flex: 1, paddingLeft: 40, justifyContent: 'center' }}>
    <div style={{ display: 'flex', fontSize: 240, fontWeight: 900, color: '#141414', position: 'absolute', top: -40, right: 40, lineHeight: 1 }}>"</div>
    <div style={{ display: 'flex', fontSize: 22, lineHeight: 1.55, color: '#e8e2d6', fontWeight: 300 }}>
      Founding AI engineer shipping production LLM systems end-to-end — retrieval pipelines, document forensics, and agentic automation — on cloud-native infrastructure.
    </div>
    <div style={{ display: 'flex', marginTop: 22, fontSize: 16, color: '#888', fontWeight: 400 }}>
      CKA-certified. Track record of measurable wins in latency, build speed, and reliability.
    </div>
    <div style={{ display: 'flex', marginTop: 28, fontSize: 12, letterSpacing: 4, color: '#1af4ff', textTransform: 'uppercase' }}>
      → BASED IN CHENNAI, INDIA
    </div>
  </div>
</div>
```

```aura width=1200 height=460
<div style={{
  width: '100%', height: '100%', display: 'flex', flexDirection: 'column',
  background: 'linear-gradient(180deg, #0a0a0a 0%, #0f0a05 100%)', fontFamily: 'Inter', color: '#f5efe6', padding: '44px 56px',
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
  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'flex-end' }}>
    <div style={{ display: 'flex', flexDirection: 'column' }}>
      <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#666', textTransform: 'uppercase' }}>§ 02 · IN PROGRESS</div>
      <div style={{ display: 'flex', fontSize: 56, fontWeight: 900, lineHeight: 1, marginTop: 8, letterSpacing: -2 }}>
        Currently <span style={{ color: '#ffb547', fontStyle: 'italic', fontWeight: 200 }}>shipping</span>
      </div>
    </div>
    <div style={{ display: 'flex', fontSize: 14, color: '#1af4ff', letterSpacing: 3, textTransform: 'uppercase', alignItems: 'center', gap: 8 }}>
      <div id="live-dot" style={{ display: 'flex', width: 10, height: 10, borderRadius: 10, background: '#1af4ff' }} />
      <div style={{ display: 'flex' }}>LIVE</div>
    </div>
  </div>

  <div style={{ display: 'flex', flex: 1, marginTop: 36, gap: 18 }}>
    {[
      { n: '01', t: 'Retrieval Platform', d: 'LLM-backed retrieval over private corpora with grounded citations.', a: '#ffb547' },
      { n: '02', t: 'Agent Runtime', d: 'LLM-driven agent automating machine-level tasks with remote multi-language code execution.', a: '#1af4ff' },
      { n: '03', t: 'CI/CD at Scale', d: 'Standardising CI/CD across 90+ repos. -60–80% failures. -50–70% build time.', a: '#ff5e5b' },
    ].map((c, i) => (
      <div key={i} id={`card-${i}`} style={{
        display: 'flex', flexDirection: 'column', flex: 1,
        background: '#111', border: '1px solid #1f1f1f', padding: 28,
        position: 'relative',
      }}>
        <div id={`bar-${i}`} style={{ display: 'flex', position: 'absolute', top: 0, left: 0, width: 60, height: 4, background: c.a }} />
        <div style={{ display: 'flex', fontSize: 12, letterSpacing: 3, color: c.a }}>{c.n}</div>
        <div style={{ display: 'flex', fontSize: 26, fontWeight: 800, marginTop: 18, lineHeight: 1.1 }}>{c.t}</div>
        <div style={{ display: 'flex', marginTop: 14, fontSize: 15, color: '#999', lineHeight: 1.5, fontWeight: 300 }}>{c.d}</div>
        <div style={{ display: 'flex', marginTop: 'auto', fontSize: 11, letterSpacing: 3, color: '#444', textTransform: 'uppercase' }}>STATUS: ACTIVE →</div>
      </div>
    ))}
  </div>
</div>
```

```aura width=1200 height=620
<div style={{
  width: '100%', height: '100%', display: 'flex', flexDirection: 'column',
  background: '#f5efe6', fontFamily: 'Inter', color: '#0a0a0a', padding: '52px 56px',
}}>
  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'flex-end', borderBottom: '2px solid #0a0a0a', paddingBottom: 18 }}>
    <div style={{ display: 'flex', flexDirection: 'column' }}>
      <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#888', textTransform: 'uppercase' }}>§ 03 · SERVICES</div>
      <div style={{ display: 'flex', fontSize: 64, fontWeight: 900, lineHeight: 1, marginTop: 8, letterSpacing: -3 }}>
        What I do for <span style={{ fontStyle: 'italic', fontWeight: 200, color: '#c2410c' }}>your business.</span>
      </div>
    </div>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: 3, color: '#888' }}>SIX DISCIPLINES →</div>
  </div>

  <div style={{ display: 'flex', flex: 1, marginTop: 28, flexWrap: 'wrap', gap: 0 }}>
    {[
      { n: '01', t: 'Idea → Production', d: 'Whiteboard to deployed system. End-to-end ownership.' },
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
          <div style={{ display: 'flex', fontSize: 11, letterSpacing: 3, color: '#c2410c', fontWeight: 700 }}>{s.n}</div>
          <div style={{ display: 'flex', flex: 1, height: 1, background: '#0a0a0a' }} />
        </div>
        <div style={{ display: 'flex', fontSize: 24, fontWeight: 800, marginTop: 14, lineHeight: 1.1, letterSpacing: -0.5 }}>{s.t}</div>
        <div style={{ display: 'flex', marginTop: 10, fontSize: 14, color: '#555', lineHeight: 1.5, fontWeight: 400 }}>{s.d}</div>
      </div>
    ))}
  </div>
</div>
```

```aura width=1200 height=340
<div style={{
  width: '100%', height: '100%', display: 'flex', flexDirection: 'column',
  background: '#0a0a0a', fontFamily: 'Inter', color: '#f5efe6', padding: '44px 56px',
}}>
  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'baseline' }}>
    <div style={{ display: 'flex', fontSize: 56, fontWeight: 900, letterSpacing: -2, lineHeight: 1 }}>
      Credentials.
    </div>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#666', textTransform: 'uppercase' }}>§ 04 · VERIFIED</div>
  </div>
  <div style={{ display: 'flex', flex: 1, marginTop: 28, gap: 14 }}>
    {[
      { i: 'CNCF', t: 'Certified Kubernetes Administrator', s: 'CKA', c: '#326CE5' },
      { i: 'MS', t: 'Azure AI Fundamentals', s: 'AI-900', c: '#0078D4' },
      { i: 'MS', t: 'Azure Fundamentals', s: 'AZ-900', c: '#0078D4' },
      { i: 'AWS', t: 'Cloud Practitioner', s: 'CCP', c: '#FF9900' },
      { i: 'GCP', t: 'Cloud Digital Leader', s: 'CDL', c: '#4285F4' },
    ].map((c, i) => (
      <div key={i} style={{
        display: 'flex', flexDirection: 'column', flex: 1, padding: 20,
        background: '#111', borderTop: `3px solid ${c.c}`,
      }}>
        <div style={{ display: 'flex', fontSize: 11, letterSpacing: 3, color: c.c, fontWeight: 700 }}>{c.i}</div>
        <div style={{ display: 'flex', fontSize: 32, fontWeight: 900, marginTop: 10, color: c.c, letterSpacing: -1 }}>{c.s}</div>
        <div style={{ display: 'flex', marginTop: 10, fontSize: 13, color: '#aaa', lineHeight: 1.3, fontWeight: 300 }}>{c.t}</div>
      </div>
    ))}
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
  background: 'linear-gradient(90deg, #ffb547 0%, #ff5e5b 50%, #1af4ff 100%)',
  fontFamily: 'Inter', padding: '44px 56px', alignItems: 'center', justifyContent: 'space-between',
  position: 'relative', overflow: 'hidden',
}}>
  <style>{`
    @keyframes ctaShimmer { 0% { transform: translateX(-100%); } 100% { transform: translateX(200%); } }
    @keyframes ctaPulse { 0%,100% { transform: scale(1); } 50% { transform: scale(1.04); } }
    #cta-shimmer { animation: ctaShimmer 3.5s ease-in-out infinite; }
    #cta-badge { animation: ctaPulse 1.8s ease-in-out infinite; transform-origin: center; }
  `}</style>
  <div id="cta-shimmer" style={{ position: 'absolute', top: 0, left: 0, width: '40%', height: '100%', display: 'flex', background: 'linear-gradient(90deg, transparent 0%, rgba(255,255,255,0.35) 50%, transparent 100%)' }} />
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
    <div id="cta-badge" style={{ display: 'flex', marginTop: 14, padding: '10px 20px', background: '#0a0a0a', color: '#f5efe6', fontSize: 13, letterSpacing: 3, fontWeight: 700 }}>
      OPEN FOR COLLABORATIONS
    </div>
  </div>
</div>
```
