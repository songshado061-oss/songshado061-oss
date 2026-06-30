<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=6C3EF5&height=200&section=header&text=Welcome&fontSize=80&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Zex%20Dev%20botat%20discord&descAlignY=60&descSize=28&descColor=ffffff" width="100%"/>
<br/>
<img src="https://i.pinimg.com/originals/0f/29/87/0f2987e3ffecf886a47511e29532a753.gif" width="350"/>
<br/>
<img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=900&size=50&pause=1000&color=A855F7&center=true&vCenter=true&width=700&height=80&lines=Zex+Dev+botat+discord" />
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1000&color=00D4FF&center=true&vCenter=true&width=600&lines=Discord+Bot+Developer+🤖;Node.js+%26+Python+Only+⚡;Building+Powerful+Bots+🚀" />
<br/>
---
## 🌟 About Me
<table>
<tr>
<td>
```yaml
Name     : Zex Dev
Role     : Discord Bot Developer
Focus    : Node.js & Python ONLY
Passion  : Building powerful bots
World    : Discord is my home 🏠
Status   : Always coding... ⚡

</td> </tr> </table> <br/>
🛠️ Programming Languages
<br/>
<a href="https://nodejs.org"><img src="https://skillicons.dev/icons?i=nodejs" width="65" height="65"/></a>

<a href="https://python.org"><img src="https://skillicons.dev/icons?i=python" width="65" height="65"/></a>

<br/><br/>

<img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"/> &nbsp; <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/> <br/> <img src="https://img.shields.io/badge/Discord.js-5865F2?style=for-the-badge&logo=discord&logoColor=white"/> &nbsp; <img src="https://img.shields.io/badge/discord.py-5865F2?style=for-the-badge&logo=discord&logoColor=white"/> <br/>
📊 GitHub Stats
<img src="https://github-readme-stats.vercel.app/api?username=ZexDev&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=A855F7&icon_color=A855F7&text_color=ffffff" width="47%"/> &nbsp; <img src="https://github-readme-streak-stats.herokuapp.com/?user=ZexDev&theme=tokyonight&hide_border=true&background=0d1117&stroke=A855F7&ring=A855F7&fire=ff6600&currStreakLabel=ffffff" width="47%"/>
<br/><br/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ZexDev&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=A855F7&text_color=ffffff" width="40%"/> <br/>
🐍 Snake Game — My Contributions
<picture> <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ZexDev/ZexDev/output/github-contribution-grid-snake-dark.svg"/> <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ZexDev/ZexDev/output/github-contribution-grid-snake.svg"/> <img src="https://raw.githubusercontent.com/ZexDev/ZexDev/output/github-contribution-grid-snake.svg" width="100%"/> </picture> <br/>
💬 Connect With Me
<a href="https://discord.com"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white"/></a>

<a href="https://youtube.com"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white"/></a>

<br/>
<img src="https://capsule-render.vercel.app/api?type=waving&color=6C3EF5&height=150&section=footer&text=Zex+Dev+botat+discord&fontSize=35&fontColor=ffffff&animation=fadeIn&fontAlignY=65" width="100%"/> <br/> <img src="https://komarev.com/ghpvc/?username=ZexDev&color=A855F7&style=for-the-badge&label=PROFILE+VIEWS"/> </div> ```
name: Generate Snake
on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
      - uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
