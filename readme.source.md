<!-- markdownlint-disable MD033 MD041 MD045 -->

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
  <div id="hero-c1" style={{ position: 'absolute', top: 24, left: 24, width: 28, height: 28, borderTop: '2px solid #ffb547', borderLeft: '2px solid #ffb547', display: 'flex' }} />
  <div id="hero-c2" style={{ position: 'absolute', top: 24, right: 24, width: 28, height: 28, borderTop: '2px solid #ffb547', borderRight: '2px solid #ffb547', display: 'flex' }} />
  <div id="hero-c3" style={{ position: 'absolute', bottom: 24, left: 24, width: 28, height: 28, borderBottom: '2px solid #ffb547', borderLeft: '2px solid #ffb547', display: 'flex' }} />
  <div id="hero-c4" style={{ position: 'absolute', bottom: 24, right: 24, width: 28, height: 28, borderBottom: '2px solid #ffb547', borderRight: '2px solid #ffb547', display: 'flex' }} />
  <div id="hero-sweep" style={{ position: 'absolute', top: 0, left: 0, width: '40%', height: '100%', display: 'flex', background: 'linear-gradient(90deg, transparent 0%, rgba(255,181,71,0.06) 50%, transparent 100%)' }} />

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
        Production LLM systems, end-to-end. Retrieval, document forensics, agentic automation — on cloud-native infra that doesn't fall over.
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
```aura width=160 height=44 link="https://linkedin.com/in/AbhijithGanesh14" inline align=center
<SocialMediaButton
  icon="https://cdn.jsdelivr.net/npm/simple-icons@v11/icons/linkedin.svg"
  text="LinkedIn"
  backgroundColor="#0a0a0a"
  textColor="#f5efe6"
  fontSize={12}
  width={160}
  height={44}
  iconSize="18"
/>
```

```aura width=1200 height=480
<div style={{
  width: '100%', height: '100%', display: 'flex', flexDirection: 'column',
  background: '#0a0a0a', fontFamily: 'Inter', color: '#f5efe6', padding: '44px 56px',
}}>
  <style>{`
    @keyframes barGrow { 0% { transform: scaleX(0); } 100% { transform: scaleX(1); } }
    @keyframes cardRise { 0% { opacity: 0; transform: translateY(16px); } 100% { opacity: 1; transform: translateY(0); } }
    #card-0 { animation: cardRise 0.8s ease-out 0.0s both; }
    #card-1 { animation: cardRise 0.8s ease-out 0.15s both; }
    #card-2 { animation: cardRise 0.8s ease-out 0.30s both; }
    #bar-0, #bar-1, #bar-2 { transform-origin: left center; animation: barGrow 1s ease-out 0.5s both; }
  `}</style>

  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'flex-end' }}>
    <div style={{ display: 'flex', fontSize: 56, fontWeight: 900, lineHeight: 1, letterSpacing: -2 }}>
      Currently <span style={{ color: '#ffb547', fontStyle: 'italic', fontWeight: 200 }}>shipping</span>
    </div>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#666', textTransform: 'uppercase' }}>§ WORK</div>
  </div>

  <div style={{ display: 'flex', flex: 1, marginTop: 32, gap: 18 }}>
    {[
      { n: '01', t: 'Retrieval Platform', d: 'LLM-backed retrieval over private corpora with grounded citations.', a: '#ffb547' },
      { n: '02', t: 'Agent Runtime', d: 'LLM-driven agent automating machine-level tasks via remote multi-language code execution.', a: '#1af4ff' },
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
      </div>
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
