<div align="center">

<!-- Animated Gradient Header -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=🌍%20Flag%20Icons&fontSize=60&fontColor=fff&animation=fadeIn&fontAlignY=35&desc=Beautiful%20Country%20Flags%20for%20Developers%20%26%20Designers&descAlignY=55&descSize=18" />

<!-- Badges Row -->
<p align="center">
  <a href="https://github.com/PashtunObserver/flag-icons/stargazers">
    <img src="https://img.shields.io/github/stars/PashtunObserver/flag-icons?style=for-the-badge&logo=github&color=f59e0b&labelColor=1e293b" alt="Stars" />
  </a>
  <a href="https://github.com/PashtunObserver/flag-icons/network/members">
    <img src="https://img.shields.io/github/forks/PashtunObserver/flag-icons?style=for-the-badge&logo=github&color=6366f1&labelColor=1e293b" alt="Forks" />
  </a>
  <a href="https://github.com/PashtunObserver/flag-icons/issues">
    <img src="https://img.shields.io/github/issues/PashtunObserver/flag-icons?style=for-the-badge&logo=github&color=ef4444&labelColor=1e293b" alt="Issues" />
  </a>
  <a href="#license">
    <img src="https://img.shields.io/github/license/PashtunObserver/flag-icons?style=for-the-badge&logo=open-source-initiative&color=10b981&labelColor=1e293b" alt="License" />
  </a>
</p>

<!-- Quick Stats -->
<p align="center">
  <img src="https://img.shields.io/badge/Countries-249+-10b981?style=flat-square&logo=google-earth&logoColor=white" />
  <img src="https://img.shields.io/badge/Formats-PNG%20%7C%20JPG%20%7C%20SVG-6366f1?style=flat-square&logo=image&logoColor=white" />
  <img src="https://img.shields.io/badge/Sizes-16px%20to%20128px-f59e0b?style=flat-square&logo=resize&logoColor=white" />
  <img src="https://img.shields.io/badge/CDN-jsDelivr-ef4444?style=flat-square&logo=cloudflare&logoColor=white" />
</p>

<!-- Website Link -->
<p align="center">
  <a href="https://www.pashtomedium.com/" target="_blank">
    <img src="https://img.shields.io/badge/🔗%20Visit%20Our%20Website-pashtomedium.com-6366f1?style=for-the-badge&logo=google-chrome&logoColor=white&labelColor=1e293b" />
  </a>
</p>

</div>

---

## 📖 Table of Contents

- [✨ Features](#-features)
- [🚀 Quick Start](#-quick-start)
- [📦 Installation](#-installation)
- [🎯 Usage Examples](#-usage-examples)
  - [HTML / CSS](#html--css)
  - [React](#react)
  - [Vue.js](#vuejs)
  - [Angular](#angular)
  - [Python / Django](#python--django)
  - [Markdown](#markdown)
- [📐 Available Sizes](#-available-sizes)
- [🎨 Available Formats](#-available-formats)
- [🌍 Supported Countries](#-supported-countries)
- [🔧 CDN URLs](#-cdn-urls)
- [📱 Live Demo](#-live-demo)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [👨‍💻 Author](#-author)

---

## ✨ Features

<div align="center">

| 🎯 Feature | 💡 Description |
|:---|:---|
| 🌍 **249+ Countries** | Complete collection of world flags including territories & regions |
| 🖼️ **3 Formats** | PNG, JPG, and SVG for every use case |
| 📐 **4 Sizes** | 16px, 32px, 64px, and 128px resolutions |
| ⚡ **jsDelivr CDN** | Lightning-fast global CDN delivery |
| 🎨 **High Quality** | Crisp, professional flag designs |
| 📱 **Responsive** | Perfect scaling on any device |
| 🆓 **100% Free** | Open source and free to use |
| 🔗 **Easy Integration** | One-line URL — no setup required |

</div>

---

## 🚀 Quick Start

Get any flag in **one line** of code:

```html
<!-- Afghanistan Flag - 64x64 PNG -->
<img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/af.png" alt="Afghanistan" width="64" />

<!-- United States Flag - 128x128 SVG -->
<img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/128x128/us.svg" alt="USA" width="128" />

<!-- Japan Flag - 32x32 JPG -->
<img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/32x32/jp.jpg" alt="Japan" width="32" />
```

> 💡 **Tip:** Replace `af`, `us`, `jp` with any [ISO country code](#-supported-countries) and adjust size/format as needed!

---

## 📦 Installation

### Option 1: Direct CDN (Recommended) ⭐
No installation needed! Just use the jsDelivr CDN URLs directly in your project.

### Option 2: Clone Repository
```bash
git clone https://github.com/PashtunObserver/flag-icons.git
```

### Option 3: npm (Coming Soon)
```bash
npm install @pashtunobserver/flag-icons
```

---

## 🎯 Usage Examples

### HTML / CSS

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    .flag {
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
      transition: transform 0.3s ease;
    }
    .flag:hover {
      transform: scale(1.1);
    }
  </style>
</head>
<body>
  <!-- Basic usage -->
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/gb.png" 
       alt="United Kingdom" class="flag" width="64" />

  <!-- With tooltip -->
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/de.png" 
       alt="Germany" title="Germany" class="flag" width="64" />
</body>
</html>
```

### React

```jsx
import React from 'react';

// Reusable Flag Component
const Flag = ({ countryCode, size = 64, format = 'png', alt, className = '' }) => {
  const url = `https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/${size}x${size}/${countryCode.toLowerCase()}.${format}`;

  return (
    <img 
      src={url} 
      alt={alt || countryCode} 
      width={size} 
      height={size}
      className={`rounded-lg shadow-md hover:scale-110 transition-transform ${className}`}
      loading="lazy"
    />
  );
};

// Usage
function App() {
  return (
    <div className="flex gap-4 p-8">
      <Flag countryCode="AF" size={64} alt="Afghanistan" />
      <Flag countryCode="US" size={128} format="svg" alt="USA" />
      <Flag countryCode="JP" size={32} format="jpg" alt="Japan" />
    </div>
  );
}

export default App;
```

### Vue.js

```vue
<template>
  <div class="flag-gallery">
    <img 
      v-for="country in countries" 
      :key="country.code"
      :src="getFlagUrl(country.code)" 
      :alt="country.name"
      :width="flagSize"
      class="flag-image"
    />
  </div>
</template>

<script>
export default {
  data() {
    return {
      flagSize: 64,
      flagFormat: 'png',
      countries: [
        { code: 'AF', name: 'Afghanistan' },
        { code: 'US', name: 'United States' },
        { code: 'GB', name: 'United Kingdom' },
      ]
    };
  },
  methods: {
    getFlagUrl(code) {
      return `https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/${this.flagSize}x${this.flagSize}/${code.toLowerCase()}.${this.flagFormat}`;
    }
  }
};
</script>

<style scoped>
.flag-image {
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  margin: 8px;
  transition: transform 0.3s ease;
}
.flag-image:hover {
  transform: translateY(-4px);
}
</style>
```

### Angular

```typescript
// flag.service.ts
import { Injectable } from '@angular/core';

@Injectable({
  providedIn: 'root'
})
export class FlagService {
  private readonly baseUrl = 'https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main';

  getFlagUrl(countryCode: string, size: number = 64, format: string = 'png'): string {
    return `${this.baseUrl}/${size}x${size}/${countryCode.toLowerCase()}.${format}`;
  }
}

// flag.component.ts
import { Component, Input } from '@angular/core';

@Component({
  selector: 'app-flag',
  template: `
    <img [src]="flagUrl" [alt]="countryName" [width]="size" class="flag-img" />
  `,
  styles: [`
    .flag-img {
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
    }
  `]
})
export class FlagComponent {
  @Input() countryCode: string = '';
  @Input() countryName: string = '';
  @Input() size: number = 64;
  @Input() format: string = 'png';

  get flagUrl(): string {
    return `https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/${this.size}x${this.size}/${this.countryCode.toLowerCase()}.${this.format}`;
  }
}
```

### Python / Django

```python
# utils.py
FLAG_BASE_URL = "https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main"

def get_flag_url(country_code, size=64, format="png"):
    """
    Generate a flag icon URL.

    Args:
        country_code (str): ISO country code (e.g., 'AF', 'US')
        size (int): Flag size in pixels (16, 32, 64, 128)
        format (str): Image format ('png', 'jpg', 'svg')

    Returns:
        str: Complete CDN URL for the flag
    """
    return f"{FLAG_BASE_URL}/{size}x{size}/{country_code.lower()}.{format}"


# Django Template Usage
# In your template:
# <img src="{{ flag_url }}" alt="{{ country_name }}" width="64">

# views.py
from django.shortcuts import render
from .utils import get_flag_url

def country_detail(request, country_code):
    context = {
        'flag_url': get_flag_url(country_code, size=128, format='png'),
        'flag_svg': get_flag_url(country_code, size=64, format='svg'),
    }
    return render(request, 'country_detail.html', context)
```

### Markdown

```markdown
<!-- In your README or documentation -->
![Afghanistan](https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/af.png)
![United States](https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/us.png)
![United Kingdom](https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/gb.png)

<!-- With link -->
[![Afghanistan](https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/32x32/af.png)](https://en.wikipedia.org/wiki/Afghanistan)
```

---

## 📐 Available Sizes

<div align="center">

| Size | Best For | Example URL |
|:---|:---|:---|
| **16×16** | Favicons, inline text, dropdowns | `.../16x16/af.png` |
| **32×32** | Lists, tables, small UI elements | `.../32x32/af.png` |
| **64×64** | Cards, profiles, general UI ⭐ | `.../64x64/af.png` |
| **128×128** | Hero sections, large displays | `.../128x128/af.png` |

</div>

> ⭐ **Recommended:** `64×64` is the sweet spot for most use cases.

---

## 🎨 Available Formats

<div align="center">

| Format | Extension | Best For | Scalable |
|:---|:---|:---|:---:|
| **PNG** | `.png` | Web, transparency, universal support | ❌ |
| **JPG** | `.jpg` | Smaller file size, photos | ❌ |
| **SVG** | `.svg` | Infinite scaling, crisp at any size | ✅ |

</div>

> 💡 **Pro Tip:** Use **SVG** for logos and icons that need to scale perfectly. Use **PNG** for maximum compatibility.

---

## 🌍 Supported Countries

We support **249+ countries and territories** including:

<div align="center">

| Region | Examples |
|:---|:---|
| 🌏 **Asia** | AF, CN, IN, JP, PK, KR, SA, TH, VN |
| 🌍 **Europe** | DE, FR, GB, IT, ES, NL, PL, RU, SE, CH |
| 🌎 **Americas** | US, CA, BR, MX, AR, CO, PE, CL |
| 🌍 **Africa** | ZA, NG, EG, KE, GH, MA, TZ, UG |
| 🌏 **Oceania** | AU, NZ, FJ, PG, SB |
| 🏴 **Regions** | GB-ENG, GB-SCT, GB-WLS, GB-NIR, XK, EU |

</div>

<details>
<summary>📋 <b>Click to view all 249+ country codes</b></summary>

```
AD Andorra          | AE United Arab Emirates | AF Afghanistan      | AG Antigua and Barbuda
AI Anguilla          | AL Albania              | AM Armenia            | AO Angola
AQ Antarctica        | AR Argentina            | AS American Samoa    | AT Austria
AU Australia         | AW Aruba                | AX Åland Islands      | AZ Azerbaijan
BA Bosnia and Herz...| BB Barbados             | BD Bangladesh         | BE Belgium
BF Burkina Faso      | BG Bulgaria             | BH Bahrain            | BI Burundi
BJ Benin             | BL Saint Barthélemy     | BM Bermuda            | BN Brunei
BO Bolivia           | BQ Caribbean Netherlands| BR Brazil             | BS Bahamas
BT Bhutan            | BV Bouvet Island        | BW Botswana           | BY Belarus
BZ Belize            | CA Canada               | CC Cocos Islands      | CD DR Congo
CF Central African.. | CG Congo                | CH Switzerland        | CI Côte d'Ivoire
CK Cook Islands      | CL Chile                | CM Cameroon           | CN China
CO Colombia          | CR Costa Rica           | CU Cuba               | CV Cape Verde
CW Curaçao           | CX Christmas Island      | CY Cyprus             | CZ Czech Republic
DE Germany           | DJ Djibouti             | DK Denmark            | DM Dominica
DO Dominican Rep...    | DZ Algeria              | EC Ecuador            | EE Estonia
EG Egypt             | EH Western Sahara       | ER Eritrea            | ES Spain
ET Ethiopia          | EU Europe               | FI Finland            | FJ Fiji
FK Falkland Islands  | FM Micronesia           | FO Faroe Islands      | FR France
GA Gabon             | GB-ENG England          | GB-NIR Northern Ire...| GB-SCT Scotland
GB-WLS Wales         | GB United Kingdom       | GD Grenada            | GE Georgia
GF French Guiana     | GG Guernsey             | GH Ghana              | GI Gibraltar
GL Greenland         | GM Gambia               | GN Guinea             | GP Guadeloupe
GQ Equatorial Guinea | GR Greece               | GS South Georgia      | GT Guatemala
GU Guam              | GW Guinea-Bissau        | GY Guyana             | HK Hong Kong
HM Heard Island      | HN Honduras             | HR Croatia            | HT Haiti
HU Hungary           | ID Indonesia            | IE Ireland            | IL Israel
IM Isle of Man       | IN India                | IO British Indian...  | IQ Iraq
IR Iran              | IS Iceland              | IT Italy              | JE Jersey
JM Jamaica           | JO Jordan               | JP Japan              | KE Kenya
KG Kyrgyzstan        | KH Cambodia             | KI Kiribati           | KM Comoros
KN Saint Kitts       | KP North Korea          | KR South Korea        | KW Kuwait
KY Cayman Islands    | KZ Kazakhstan           | LA Laos               | LB Lebanon
LC Saint Lucia       | LI Liechtenstein        | LK Sri Lanka          | LR Liberia
LS Lesotho           | LT Lithuania            | LU Luxembourg         | LV Latvia
LY Libya             | MA Morocco              | MC Monaco             | MD Moldova
ME Montenegro        | MF Saint Martin         | MG Madagascar         | MH Marshall Islands
MK North Macedonia   | ML Mali                 | MM Myanmar            | MN Mongolia
MO Macao             | MP Northern Mariana      | MQ Martinique         | MR Mauritania
MS Montserrat        | MT Malta                | MU Mauritius          | MV Maldives
MW Malawi            | MX Mexico               | MY Malaysia           | MZ Mozambique
NA Namibia           | NC New Caledonia        | NE Niger              | NF Norfolk Island
NG Nigeria           | NI Nicaragua            | NL Netherlands        | NO Norway
NP Nepal             | NR Nauru                | NU Niue               | NZ New Zealand
OM Oman              | PA Panama               | PE Peru               | PF French Polynesia
PG Papua New Guinea  | PH Philippines          | PK Pakistan           | PL Poland
PM Saint Pierre      | PN Pitcairn             | PR Puerto Rico        | PS Palestine
PT Portugal          | PW Palau                | PY Paraguay           | QA Qatar
RE Réunion           | RO Romania              | RS Serbia             | RU Russia
RW Rwanda            | SA Saudi Arabia         | SB Solomon Islands    | SC Seychelles
SD Sudan             | SE Sweden               | SG Singapore          | SH Saint Helena
SI Slovenia          | SJ Svalbard             | SK Slovakia           | SL Sierra Leone
SM San Marino        | SN Senegal              | SO Somalia            | SR Suriname
SS South Sudan       | ST São Tomé             | SV El Salvador        | SX Sint Maarten
SY Syria             | SZ Eswatini             | TC Turks and Caicos   | TD Chad
TF French Southern.. | TG Togo                 | TH Thailand           | TJ Tajikistan
TK Tokelau           | TL Timor-Leste          | TM Turkmenistan       | TN Tunisia
TO Tonga             | TR Türkiye              | TT Trinidad            | TV Tuvalu
TW Taiwan            | TZ Tanzania             | UA Ukraine            | UG Uganda
UM US Minor Outlying | US United States        | UY Uruguay            | UZ Uzbekistan
VA Vatican City      | VC Saint Vincent        | VE Venezuela          | VG British Virgin Is.
VI US Virgin Islands | VN Vietnam              | VU Vanuatu            | WF Wallis and Futuna
WS Samoa             | XK Kosovo               | YE Yemen              | YT Mayotte
ZA South Africa      | ZM Zambia               | ZW Zimbabwe
```

</details>

---

## 🔧 CDN URLs

### URL Structure

```
https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/{SIZE}x{SIZE}/{CODE}.{FORMAT}
```

### Parameters

| Parameter | Description | Example |
|:---|:---|:---|
| `{SIZE}` | Image dimension (16, 32, 64, 128) | `64` |
| `{CODE}` | ISO 3166-1 alpha-2 country code (lowercase) | `af`, `us`, `gb` |
| `{FORMAT}` | Image format extension | `png`, `jpg`, `svg` |

### Examples

```
🇦🇫 Afghanistan  →  https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/af.png
🇺🇸 USA           →  https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/us.png
🇬🇧 UK            →  https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/gb.png
🇯🇵 Japan         →  https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/jp.png
🇩🇪 Germany       →  https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/de.png
🇫🇷 France        →  https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/fr.png
```

---

## 📱 Live Demo

<div align="center">

🌐 **Try the interactive gallery:** [https://pashtunobserver.github.io/flag-icons/](https://pashtunobserver.github.io/flag-icons/)

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/af.png" width="48" />
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/us.png" width="48" />
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/gb.png" width="48" />
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/jp.png" width="48" />
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/de.png" width="48" />
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/fr.png" width="48" />
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/in.png" width="48" />
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/br.png" width="48" />
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/cn.png" width="48" />
  <img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/au.png" width="48" />
</p>

</div>

---

## 🤝 Contributing

We welcome contributions from the community! 🙌

```bash
# 1. Fork the repository
# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/flag-icons.git

# 3. Create a feature branch
git checkout -b feature/amazing-feature

# 4. Make your changes and commit
git commit -m "Add amazing feature"

# 5. Push to your fork
git push origin feature/amazing-feature

# 6. Open a Pull Request
```

### Contribution Guidelines
- 🐛 **Bug Reports:** Open an issue with detailed description
- 💡 **Feature Requests:** Open an issue with the `enhancement` label
- 🎨 **Flag Updates:** Ensure flags follow official designs
- 📖 **Documentation:** Help improve this README

---

## 📄 License

```
MIT License

Copyright (c) 2026 PashtunObserver

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

<div align="center">

[![MIT License](https://img.shields.io/badge/License-MIT-10b981?style=for-the-badge&logo=open-source-initiative&logoColor=white)](LICENSE)

</div>

---

## 👨‍💻 Author

<div align="center">

<img src="https://cdn.jsdelivr.net/gh/PashtunObserver/flag-icons@main/64x64/af.png" width="48" style="border-radius: 50%;" />

### **Rashid Ahmad SST IT**

🎓 **Gold Medalist** · **BS Computer Science** · **University of Swat**

<p>
  <a href="https://www.pashtomedium.com/" target="_blank">
    <img src="https://img.shields.io/badge/🔗%20Website-pashtomedium.com-6366f1?style=for-the-badge&logo=google-chrome&logoColor=white" />
  </a>
</p>

<p>
  <a href="https://github.com/PashtunObserver" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-PashtunObserver-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</p>

> 💬 *"Built with ❤️ for developers worldwide"*

</div>

---

<div align="center">

<!-- Footer Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer&text=Happy%20Coding!%20🚀&fontSize=30&fontColor=fff&animation=fadeIn" />

<p>
  <a href="https://www.pashtomedium.com/" target="_blank">
    <strong>🔗 Backlink: https://www.pashtomedium.com/</strong>
  </a>
</p>

<p>
  <sub>Made with ❤️ by <a href="https://www.pashtomedium.com/">PashtunObserver</a> · © 2026 All Rights Reserved</sub>
</p>

</div>
