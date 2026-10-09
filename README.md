<div align="center">

<img src="logo.png" alt="بانگ App Icon" width="120" style="border-radius:24px;" />

# 🕌 بانگ — Kurdistan Prayer Times

### Open-source prayer time database for the Kurdistan Region of Iraq

[![License](https://img.shields.io/badge/license-open--source-green?style=flat-square)](LICENSE)
[![Cities](https://img.shields.io/badge/cities-36-gold?style=flat-square)](#available-cities)
[![Data](https://img.shields.io/badge/format-JSON-blue?style=flat-square)](#data-format)
[![Pages](https://img.shields.io/badge/demo-live-brightgreen?style=flat-square)](https://bang-kurdistan.github.io/)

<br />

**بانگ** (Bang) is a prayer times app built for Kurdistan.
This repository is the **open data layer** behind it — accurate, city-level Islamic prayer schedules for every day of the year.

**[🌐 Live Demo](https://bang-kurdistan.github.io/)** · **[🔗 App links](https://bang-kurdistan.github.io/links/)** · **[📥 Download Data](#downloads)** · **[🐛 Report Issue](https://github.com/Bang-Kurdistan/kurdistan-prayer-times/issues)**

<br />

[<img src="https://developer.apple.com/assets/elements/badges/download-on-the-app-store.svg" height="44" alt="Download on the App Store" />](https://apps.apple.com/us/app/bang-%D8%A8%D8%A7%D9%86%DA%AF/id627367343)&nbsp;&nbsp;
[<img src="https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg" height="44" alt="Get it on Google Play" />](https://play.google.com/store/apps/details?id=com.c4kurd.bang)

</div>

---

## ✨ Features

|                          |                                                                     |
| ------------------------ | ------------------------------------------------------------------- |
| 🏙️ **36 Cities**         | Complete prayer time coverage across the Kurdistan Region           |
| 📅 **365 Days**          | Full-year schedules with 6 daily prayer times per city              |
| 🔍 **Search & Filter**   | Find any city instantly, filter by month                            |
| 📊 **Today Highlight**   | Automatically highlights today's row with a summary strip           |
| 📥 **CSV Downloads**     | Download individual city tables or all 36 cities at once            |
| 📱 **Responsive**        | Sleek dark UI that works beautifully on desktop, tablet, and mobile |
| 🌐 **Bilingual**         | Column headers in both English and Kurdish (Sorani)                 |
| ⚡ **Zero Dependencies** | Pure HTML/CSS/JS — no frameworks, no build step                     |

---

## 🌍 About the App

**بانگ** is a prayer times application built for Kurdistan.

The app provides accurate prayer times for cities across the Kurdistan Region of Iraq, helping Muslims know exactly when to pray no matter where they are in the region.

This repository serves as the **open data source** for the app. All prayer time data is freely available as JSON files, and the interactive web viewer is deployed via GitHub Pages.

---

## 📍 Available Cities

<table>
<tr><td>

|   # | Kurdish    | English    |
| --: | ---------- | ---------- |
|   1 | هه‌ولێر    | Hawler     |
|   2 | سلێمانی    | Slemany    |
|   3 | دهۆك       | Duhok      |
|   4 | كه‌ركووك   | Kirkuk     |
|   5 | هه‌ڵه‌بجه‌ | Halabja    |
|   6 | سۆران      | Soran      |
|   7 | كۆیه‌      | Koya       |
|   8 | ئاكرێ      | Akre       |
|   9 | چه‌مچه‌ماڵ | Chamchamal |
|  10 | قه‌ڵادزێ   | Qaladze    |
|  11 | رانیه‌     | Ranya      |
|  12 | كفری       | Kfri       |

</td><td>

|   # | Kurdish       | English     |
| --: | ------------- | ----------- |
|  13 | كه‌لار        | Kalar       |
|  14 | زاخۆ          | Zaxo        |
|  15 | ده‌ربه‌ندیخان | Darbandixan |
|  16 | موسڵ          | Mosul       |
|  17 | توزخورماتو    | Tuzxurmatu  |
|  18 | ئامێدی        | Amedi       |
|  19 | سەیدسادق      | Said Sadiq  |
|  20 | پێنجوێن       | Penjuin     |
|  21 | هەڵەبجەی تازە | Halabja Nwe |
|  22 | عەربەت        | Arbat       |
|  23 | پیرەمەگرون    | Piramagrun  |
|  24 | تاسڵوجە       | Tasluja     |

</td><td>

|   # | Kurdish    | English     |
| --: | ---------- | ----------- |
|  25 | بازیان     | Bazyan      |
|  26 | دوکان      | Dukan       |
|  27 | تەکیە      | Takya       |
|  28 | حاجی ئاوا  | Haji Awa    |
|  29 | خەلەکان    | Xalakan     |
|  30 | تەقتەق     | Taq Taq     |
|  31 | بەرزنجە    | Barznja     |
|  32 | قەرەداغ    | Qaradax     |
|  33 | قادر کەرەم | Qadir Karam |
|  34 | خانەقین    | Xanaqin     |
|  35 | چوارتا     | Chwarta     |
|  36 | قەسرێ      | Qasre       |

</td></tr>
</table>

---

## 📂 Data Format

Each city has a JSON file in the `data/` directory containing an array of daily entries:

```json
{
  "ID": 1,
  "Date": "01-01",
  "Fajr": "06:02",
  "Sunrise": "07:21",
  "Dhuhr": "12:16",
  "Asr": "02:45",
  "Maghrib": "05:06",
  "Isha": "06:21"
}
```

### Fields

| Field     | Description         | Kurdish      |
| --------- | ------------------- | ------------ |
| `ID`      | Row number (1–366)  |              |
| `Date`    | Day-Month (`MM-DD`) | بەروار       |
| `Fajr`    | Dawn prayer         | بانگی بەیانی |
| `Sunrise` | Sunrise time        | خۆرهەڵات     |
| `Dhuhr`   | Noon prayer         | نیوەڕۆ       |
| `Asr`     | Afternoon prayer    | عەسر         |
| `Maghrib` | Sunset prayer       | شێوان        |
| `Isha`    | Night prayer        | خەوتنان      |

---

## 📥 Downloads

### From the Web

Visit the **[live site](https://bang-kurdistan.github.io/)** and use:

- **"Download CSV"** button — downloads the currently selected city's prayer times as a CSV file
- **"Download All Cities"** button — fetches all 36 cities and generates a single combined CSV

### From This Repository

```
data/
├── Akre.json
├── Amedi.json
├── Arbat.json
├── ...
└── Zaxo.json        # 36 JSON files total
```

Clone or download individual files directly:

```bash
# Clone the entire repository
git clone https://github.com/Bang-Kurdistan/kurdistan-prayer-times.git

# Or fetch a single city's data
curl -O https://raw.githubusercontent.com/Bang-Kurdistan/kurdistan-prayer-times/main/data/Hawler.json
```

---

## 🏗️ Project Structure

```
kurdistan-prayer-times/
├── index.html          # Interactive web viewer (single file, zero deps)
├── prayer-data.js      # All city data bundled as JS (no server needed)
├── .nojekyll           # Disables Jekyll so GitHub Pages serves all files
├── data/               # Prayer time JSON files (one per city)
│   ├── Hawler.json
│   ├── Slemany.json
│   └── ...
├── excel_files/        # Original Excel source files
├── logo.png
├── katakani-bang.sqlite # SQLite database used in the app
├── LICENSE
└── README.md
```

---

## 🤝 Contributing

Contributions are welcome! You can help by:

- 🌆 **Adding new cities** — provide prayer time data in the same JSON format
- 🔧 **Correcting times** — if you find inaccuracies, open an issue or submit a PR
- 🌐 **Improving the web UI** — styling, accessibility, new features

---

## 📄 License

This project is open source and freely available for public use. See [LICENSE](LICENSE) for details.

---

<div align="center">

**Built with ❤️ in Kurdistan**

</div>
