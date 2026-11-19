# FlipClock CYD 2.0

Orologio digitale con animazione a palette flip, ispirato agli orologi e agli indicatori delle stazioni ferroviarie. Progettato per **ESP32 CYD 2.8" (ESP32-2432S028R)**.

## Installa dal browser

**Web Flasher:** https://fraland71.github.io/FlipClock/

1. Collega la scheda al computer con un cavo USB dati.
2. Apri il Web Flasher con Chrome o Edge su desktop (Web Serial).
3. Premi **Installa FlipClock 2.0**, scegli la porta USB e segui le istruzioni.
4. Se richiesto, riavvia la scheda dopo l'installazione.

> **Attenzione:** il flash può cancellare configurazioni e impostazioni preesistenti. Utilizza solo un ESP32 CYD 2.8" compatibile. Non è un firmware per ESP32-S3. Le revisioni hardware diverse non sono state testate.

## Struttura dei file

- `index.html` — pagina Web Flasher per GitHub Pages
- `manifest.json` — manifest ESP Web Tools
- `firmware/FlipClock_CYD_2.0.merged.bin` — firmware merged da 8 MiB; offset flash `0x0000`

Il file merged include bootloader, partizioni e applicazione. **La cartella firmware e il file .bin devono essere presenti per consentire l'installazione online.**

## Attivazione di GitHub Pages

In **Settings → Pages**, seleziona **Deploy from a branch → main → / (root)**, poi salva. Dopo il deploy, apri https://fraland71.github.io/FlipClock/.

Questo repository distribuisce il firmware compilato, non il codice sorgente Arduino.

© 2026 Francesco Landi.
