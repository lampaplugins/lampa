# /brag: Лампа

## Inspection answers

- **What is it?** Lampa is a free app that turns a TV into a catalog of films and series: browse with the remote, press OK, and you get the full card for the title.
- **Who is it for, and what does it do for them?** People watching on a TV, a set-top box or a phone. They can browse what's new, find any film and open its card without a mouse or keyboard, using only the arrows and OK.
- **What sets it apart?**
  - «Приложение полностью бесплатное» (README).
  - Runs on LG webOS, Samsung Tizen, MSX, Android, macOS and Windows (README).
  - 12 interface languages (`lang/`).
  - The interface is built for a remote.
- **Most impressive claim:** it's free and works on almost any screen.
- **Visual hook:** Lampa means "lamp". The logo's arcs light up like a lamp, and the light reveals a wall of posters.
- **Real UI to show:**
  - The main screen, with the focus jumping between posters and the background tint following the poster.
  - OK opens the card for «Хитрый Койот».
  - The on-screen keyboard types «дюна», and every Dune appears.
  - The side menu.
- **Tone:** `default`: playful, clean, quick. Russian, like the app.
- **Share caption:** «Лампа — бесплатный каталог фильмов и сериалов для телевизора.»

## Angle

"Включи Лампу": the lamp switches on and lights up the screen full of films. Then the video shows the real app in use with the remote: arrows, OK, search. It ends with the fact that all of this is free.

## Visual identity

- Background #1d1f20 (the app's `theme-color`), white text, and the SegoeUI font from `fonts/`.
- The Lampa logo is concentric arcs (`img/logo-icon.svg`); the wordmark is `img/logo.svg`.
- Warm lamp glow as the one accent: it appears only in the hook and the finale.
- The app itself is shown in a floating screen with rounded corners. A small remote D-pad in the corner lights up on each press.
- All UI is real: captures of the app from `index.html`, with live TMDB data at 2× resolution.

## Storyboard (20.5 s, 1920×1080, 30 fps, 120 BPM: one bar = 2 s)

| # | Time | Scene | Text | Motion / sound |
|---|---|---|---|---|
| 1 | 0.0–2.5 | Hook: dark screen. The logo's arcs light up one by one, then a burst of warm light reveals a tilted wall of real posters. | «Включи Лампу.» | 4 tuned plucks, one per arc; a "click" and a chord bloom as the light spreads; a soft build into the beat. |
| 2 | 2.5–6.5 | Reveal: the real main screen «Сейчас смотрят». The focus moves right twice, from «Обитель зла» to «Хитрый Койот», and the background tint changes. | «Фильмы и сериалы в твоём ТВ» | The beat comes in. Presses land on beats (3.5, 4.5), with the D-pad lighting up and soft clicks in key. |
| 3 | 6.5–10.5 | OK: the «Хитрый Койот» card opens (backdrop, 7.5 TMDB, genres, «Смотреть»). Slow push-in. | «Нажал ОК — и всё о фильме» | OK on the D-pad at 6.25, the card on the downbeat at 6.5. |
| 4 | 10.5–14.5 | Search: «д-ю-н-а» is typed on the on-screen keyboard (camera close in), then results «Фильмы»: Дюна 2021 / 1984 / Часть вторая / Часть третья, with a scroll down to them. | «Найдётся всё» (lands with the results) | Letters on eighth notes (11.0–11.75), results at 12.0. |
| 5 | 14.5–17.5 | The screen moves left (the real side menu), and platforms appear on the right. | «Телевизор. Приставка. Смартфон.» and the chips LG webOS · Samsung Tizen · Android · MSX · macOS · Windows · 12 языков | Words one at a time, chips one at a time, each a quiet note. |
| 6 | 17.5–20.5 | Finale: the lamp glow, the logo and the LAMPA wordmark. | «Это Бесплатно.» and «yumata.github.io/lampa» | A final chord, the beat stops, the pad rings out. |

Total: 2.5 + 4 + 4 + 4 + 3 + 3 = 20.5 s.

## Sound

The music is synthesized for this video (numpy): C major, the progression Fmaj7 – G6 – Em7 – Am7, 120 BPM.

- **Parts:** kick, soft clap, hats, bass, a pad with sidechain ducking, and a plucked arpeggio with delay.
- **Effects are part of the track:** remote clicks and typing are short notes from the current chord, and the "switch" sound is a chord bloom.
- **Mix:** a shared reverb, effects about 10–12 dB below the music, and a soft limiter on the master.

## Sources

- The app: `index.html` and `app.min.js` (v3.3.4), captured in headless Chromium. The TMDB API was routed to api.themoviedb.org, because the default mirror has an expired certificate. Metrics and ads were blocked for the capture.
- Texts: approved by the user.
