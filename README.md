# Ambidextro Browser Port
A browser port of [Ambidextro](https://store.steampowered.com/app/3445580/Ambidextro/),
originally created by Majorariatto / Alva Majo.
###### plz don't sue me

## Play online

- https://ambidextro.netlify.app/
- https://ambidextro.surge.sh/

## Run locally

1. Install [7-Zip](https://www.7-zip.org/) or use [win-rar](https://www.win-rar.com/start.html?&L=0) if gay
2. Download all four archive parts:
   - [browser port.7z.001](https://github.com/chromecrash/Ambidextro-browser-port/raw/refs/heads/main/browser%20port.7z.001)
   - [browser port.7z.002](https://github.com/chromecrash/Ambidextro-browser-port/raw/refs/heads/main/browser%20port.7z.002)
   - [browser port.7z.003](https://github.com/chromecrash/Ambidextro-browser-port/raw/refs/heads/main/browser%20port.7z.003)
   - [browser port.7z.004](https://github.com/chromecrash/Ambidextro-browser-port/raw/refs/heads/main/browser%20port.7z.004)
3. Select all four files, right-click → 7-Zip → Extract (on Windows 11: right-click → Show more options first).
4. In the extracted folder, run `python -m http.server 8000`.
5. Open `http://localhost:8000` in your browser and click `Ambidextro.html`.

Note: saves are stored in the browser (IndexedDB), per site.

## Hosting

Upload the extracted folder (from step 2&3 of run locally) to any static host that supports 100+ MB files,
e.g. [Netlify](https://www.netlify.com/). More options:
[list of static hosts](https://fmhy.net/developer-tools#static-page-hosting).

## How it was made
I downloaded them game and uploaded the .pck to [gdsdecomp](https://github.com/GDRETools/gdsdecomp) and then gave [opencode](https://github.com/anomalyco/opencode) access to that folder and asked it to remove all steam dependencies so it could run on browser.

## Credits

- Original game: Majorariatto / Alva Majo
- Web port: chromecrash (Steam integration removed, translation loading and saves adapted for WebAssembly)
