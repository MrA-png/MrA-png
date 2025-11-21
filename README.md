<!-- Banner -->
<div align="center">
  <img src="https://i.imgur.com/yZ8M5Q0.gif" width="650" alt="Banner"/>
</div>

<h1 align="center">Hi, I'm Azhrul 👋</h1>

<p align="center">
  <b>Software Engineer (1–2 years)</b> — passionate about Full Stack Development, AI, and modern coding workflow.<br/>
  I love exploring new technologies, especially Artificial Intelligence 🤖 and how ChatGPT can accelerate IT development.<br/>
  Currently practicing <b>Vibe Coding</b> and sharpening skills for future growth.
</p>

---

# 🌗 Automatic Dark / Light Mode Stats

<div align="center">

<!-- GitHub Stats -->
<picture>
  <source srcset="https://github-readme-stats.vercel.app/api?username=MrA-png&show_icons=true&theme=tokyonight&hide_border=true" media="(prefers-color-scheme: dark)" />
  <source srcset="https://github-readme-stats.vercel.app/api?username=MrA-png&show_icons=true&theme=default&hide_border=true" media="(prefers-color-scheme: light)" />
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=MrA-png&show_icons=true&theme=default&hide_border=true"/>
</picture>

<!-- Top Languages -->
<picture>
  <source srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=MrA-png&layout=compact&theme=tokyonight&hide_border=true" media="(prefers-color-scheme: dark)" />
  <source srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=MrA-png&layout=compact&theme=default&hide_border=true" media="(prefers-color-scheme: light)" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MrA-png&layout=compact&theme=default&hide_border=true"/>
</picture>

</div>

---

# 📈 Auto-Updating Contribution Graph

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=MrA-png&theme=react-dark&area=true&hide_border=true"/>
</div>

---

# 📆 Auto-Update Stats (Daily)

Tambahkan file GitHub Actions agar stats otomatis refresh tiap hari.

### Buat file:
`.github/workflows/update-stats.yml`

Isi dengan:

```yml
name: Update Stats

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: anmol098/waka-readme-stats@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
