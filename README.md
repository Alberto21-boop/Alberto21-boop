## Oi eu sou o Àlberto Barbòsa !👋 


![Alberto21 GitHub Stats](https://github-readme-stats.vercel.app/api?username=Alberto21-boop&show_icons&theme=blue-green)
![Alberto21 GitHub Stats](https://github-readme-stats.vercel.app/api/top-langs/?username=Alberto21-boop&show_icons&theme=blue-green)

## Tecnologias que uso no meu trabalho e no meu dia!

<div style="display: inline_block"><br/>
  <img align="center" alt="C#" src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white" />
  <img align="center" alt="MySQL" src="https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white" />
  <img align="center" alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
  
  </div><br>
  
 
   ![Alberto21 GitHub Stats](https://github.com/Alberto21-boop/Alberto21-boop/blob/output/github-contribution-grid-snake.svg)
   
    name: Generate Datas

   on:
   schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

  DEV em construção


