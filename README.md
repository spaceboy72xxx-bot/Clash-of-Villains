# MOBA ni Joy

Laro sa browser na JavaScript ang code (Three.js). Pumili ng hero, tapos sirain ang mga tower at ang Nexus ng Pula.

## Mga hero
- **Joy** (Mage): Kidlat at Starfall
- **Skeleton** (Tank): Slam at Rage
- **Behemoth** (Bruiser): Charge at Roar
- **Minotaur** (Assassin): Dive at Gale

## Mga file
- `index.html`: ang mismong laro. May loading screen, pagpili ng hero, at walang editor.
- `editor.html`: ang Mini Game Editor (opsyonal), para makita at mabago ang script ng laro.

## Laruin
- Hintaying matapos ang loading, pindutin ang **Maglaro**, at pumili ng hero.
- Joystick (kaliwa-baba) o tap sa lupa para maglakad.
- Kanan-baba: malaking button ang atake, at sa paligid nito ang mga skill. Sa ilalim, **Recall** at **Heal**.
- May banggaan ang mga puno, tower, Nexus, at mga unit.
- Pindutin ang **Ulit** (kanan-taas) para bumalik sa pagpili ng hero.
- Pinch (o scroll) para mag-zoom ng camera.

## I-deploy sa GitHub Pages
1. Gumawa ng bagong repository sa GitHub.
2. Add file > Upload files. I-upload ang `index.html`, `editor.html`, at `README.md`. Commit changes.
3. Settings > Pages > Source: **Deploy from a branch** > Branch: `main`, folder `/ (root)` > Save.
4. Maghintay ng ilang minuto. Ang laro ay nasa link ng Pages mo, at ang editor ay sa dulo ng link na `/editor.html`.

## Para i-upload ang sarili mong laro
1. Buksan ang editor at gawin ang laro. Ilagay ang pangalan ng laro sa kahon sa taas.
2. Pindutin ang **I-export ang Laro**. Makukuha mo ang `laro.html`: may loading screen at walang editor.
3. Palitan ang pangalan nito ng `index.html` at i-upload sa GitHub.
4. Hindi kasama sa export ang mga na-import na GLB. Pero pwede mong gamitin sa script ang `Spawn("joy")`, `Spawn("skeleton")`, `Spawn("beast")`, at `Spawn("minotaur")`, na naka-embed na.

## Paalala
- Kailangan ng internet dahil kinukuha ang Three.js mula sa CDN.
- Mabigat ang file (mga 3 MB) dahil naka-embed ang mga 3D model at texture.
- Auto-rig ang galaw ng mga character (hula batay sa hugis), kaya hindi ito kasing-ayos ng totoong animation.
- Wala pang physics na kumpleto, gold, items, at multiplayer. AI lang ang kalaban.
