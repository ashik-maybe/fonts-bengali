# 📁 Bengali Fonts

![Font Types](https://img.shields.io/badge/TTF%20%7C%20OTF-included-F9F6EE)
🇧🇩

A curated collection of Bengali fonts for Linux, design, publishing, and localization workflows. Includes Unicode-compliant fonts, legacy ANSI fonts, and variable/static weights—organized for sparse install and zero-residue setup.

## 📦 Structure

```bash
fonts-bengali/
├── Common-Bangla-Fonts/
│   ├── *.ttf
│   ├── Baloo_Da_2/
│   ├── Hind_Siliguri/
│   ├── Noto_Sans_Bengali/
│   ├── Noto_Serif_Bengali/
│   ├── ruposhibangla/
│   └── ...
└── README.md
```

## 🔤 Font Categories

- **Unicode Fonts**: Noto, Hind, Tiro, Baloo Da 2
- **Legacy Fonts**: SolaimanLipi, Nikosh, SutonnyMJ
- **UI vs Print Variants**: Ruposhi Bangla UI & Print
- **Variable Weights**: BalooDa2, Noto Sans/Serif Bengali
- **Decorative & Handwriting**: BenSen, Akaash, Sagarnormal

## ⚠️ Licensing Note

Fonts are sourced from various authors and projects. Some are open-source, others are freeware or proprietary. Please verify individual font licenses before redistribution or commercial use.

## 🛠️ Quick Install (Linux)

```bash
git clone --depth=1 --filter=blob:none --sparse https://github.com/ashik-maybe/fonts-bengali.git /tmp/bnfonts \
&& cd /tmp/bnfonts \
&& git sparse-checkout set Common-Bangla-Fonts \
&& mkdir -p ~/.local/share/fonts \
&& cp -r Common-Bangla-Fonts/* ~/.local/share/fonts/ \
&& fc-cache -fv
```

This command:

- Clones only the `Common-Bangla-Fonts` folder (no history, no blobs)
- Installs fonts to `~/.local/share/fonts` (XDG-compliant)
- Refreshes font cache for immediate use

<!-- ## 🧵 Selective Install (e.g. Noto Only)

```bash
find Common-Bangla-Fonts/Noto_* -type f -iname "*.ttf" \
  -exec cp {} ~/.local/share/fonts/ \; \
&& fc-cache -fv
``` -->
