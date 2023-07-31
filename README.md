# an3172123
![header](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=120&animation=fadeIn&section=footer&text=🚗🚘🚛&fontAlign=70)
<a href="s">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=dkssud8150&exclude_repo=dkssud8150.github.io&layout=compact&theme=tokyonight" />
</a>
<img src="https://raw.githubusercontent.com/dkssud8150/github-stats-transparent/output/generated/languages.svg" width="49.2%" />
[![Ashutosh's github activity graph](https://activity-graph.herokuapp.com/graph?username=dkssud8150&theme=nord)](https://github.com/ashutosh00710/github-readme-activity-graph)
![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=dkssud8150&theme=nord_dark)
[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=dkssud8150&theme=tokyonight)](https://git.io/streak-stats)
[![willianrod's wakatime stats](https://github-readme-stats.vercel.app/api/wakatime?username=dkssud8150)](https://github.com/anuraghazra/github-readme-stats)
<code><img alt = "3.1 Python" height="20" src="https://cdn.icon-icons.com/icons2/2699/PNG/512/pytorch_logo_icon_170820.png"> pytorch</code>
[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=an3172)](https://solved.ac/an3172/)

name: GitHub-Profile-3D-Contrib

on:
  schedule: # 03:00 JST == 18:00 UTC
    - cron: "0 18 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    name: generate-github-profile-3d-contrib
    steps:
      - uses: actions/checkout@v2
      - uses: yoshi389111/github-profile-3d-contrib@0.6.0
        env:
          GITHUB_TOKEN: $
          USERNAME: $
      - name: Commit & Push
        run: |
          git config user.name github-actions
          git config user.email github-actions@github.com
          git add -A .
          git commit -m "generated"
          git push

