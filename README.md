## Hi there 👋


# 🚀 Muhammet Hanifi Yıldırım | Developer & Dreamer

---

### ⚡ Hakkımda
Ben, hayallerini koda dökmeyi seven, **azimli** ve **hayalperest** bir yazılım geliştiriciyim. Dijital dünyalar inşa etmeye olan tutkum, beni **Unreal Engine** ile oyun tasarlamaya ve hem **mobil** hem de **masaüstü** platformlarda çalışan kullanıcı odaklı uygulamalar geliştirmeye itiyor.

- 🌱 Şu an bilgisayar programcılığı üzerine eğitim alıyor ve modern yazılım mimarilerini keşfediyorum.
- 🎮 Oyun mekanikleri ve 3D dünyalar tasarlamak en büyük hobim ve işim.
- 💻 Full-stack geliştirme süreçlerinde C#, Kotlin ve React gibi teknolojilerle projeler üretiyorum.
- 🎯 Hedefim; her zaman sınırları zorlayan, görsel estetiği yüksek ve performanslı yazılımlar ortaya koymak.

---



## 🌐 Socials:
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/Whyildiriw) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/muhammetyıldırım-coder) 

# 💻 Tech Stack:
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white) ![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Kotlin](https://img.shields.io/badge/kotlin-%237F52FF.svg?style=for-the-badge&logo=kotlin&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![Firebase](https://img.shields.io/badge/firebase-%23039BE5.svg?style=for-the-badge&logo=firebase) ![.Net](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white) ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) ![Apache](https://img.shields.io/badge/apache-%23D42029.svg?style=for-the-badge&logo=apache&logoColor=white) ![Firebase](https://img.shields.io/badge/firebase-a08021?style=for-the-badge&logo=firebase&logoColor=ffcd34) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white) ![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white) ![Adobe Photoshop](https://img.shields.io/badge/adobe%20photoshop-%2331A8FF.svg?style=for-the-badge&logo=adobe%20photoshop&logoColor=white) ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white) ![Unreal Engine](https://img.shields.io/badge/unrealengine-%23313131.svg?style=for-the-badge&logo=unrealengine&logoColor=white) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
# 📊 GitHub Stats:
![](https://github-readme-stats.shion.dev/api?username=Muhammet252&theme=chartreuse-dark&hide_border=false&include_all_commits=false&count_private=false)<br/>
![](https://streak-stats.demolab.com/?user=Muhammet252&theme=chartreuse-dark&hide_border=false)<br/>
![](https://github-readme-stats.shion.dev/api/top-langs/?username=Muhammet252&theme=chartreuse-dark&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

---
[![](https://komarev.com/ghpvc/?username=Muhammet252&icon=0&color=0)](https://visitcount.itsvg.in)




name: Generate Snake
permissions:
  contents: write
on:
  schedule:
    - cron: "0 0 * * *"   # runs daily
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: arnav7777
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake.gif
            dist/github-snake-dark.svg?palette=github-dark
            dist/github-snake-light.svg?palette=github-light
            
      - name: Push snake
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
