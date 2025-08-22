<div align="center">

# ​ Hi, I'm **YOUR_NAME**

💻 Full-Stack Developer | Passionate about building scalable web applications

[![Profile Views](https://komarev.com/ghpvc/?username=pranjitbis&style=flat-square)](https://github.com/pranjitbis)
[![Followers](https://img.shields.io/github/followers/pranjitbis?style=flat-square)](https://github.com/pranjitbis?tab=followers)
[![Stars](https://img.shields.io/github/stars/pranjitbis?affiliations=OWNER&style=flat-square)](https://github.com/pranjitbis?tab=repositories)

</div>

---

## ​ Live Activity — Contribution Snake

<p align="center">
  <img src="https://raw.githubusercontent.com/pranjitbis/pranjitbis/output/snake.svg" alt="Contribution Snake" />
</p>

---

## ​​ Tech Stack

### Frontend
<p>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5"/>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3"/>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript"/>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" alt="React"/>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" alt="Next.js"/>
</p>

### Backend
<p>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" alt="Node.js"/>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/express/express-original.svg" alt="Express.js"/>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" alt="Next.js API"/>
</p>

### Databases
<p>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" alt="MySQL"/>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" alt="MongoDB"/>
  <img height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" alt="PostgreSQL"/>
</p>

---

## ​ GitHub Stats

<div align="center">

<a href="https://github.com/anuraghazra/github-readme-stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=pranjitbis&show_icons=true&rank_icon=github&hide_border=true" alt="GitHub Stats"/>
</a>
<a href="https://github.com/anuraghazra/github-readme-stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=pranjitbis&layout=compact&hide_border=true" alt="Top Languages"/>
</a>
<a href="https://github.com/DenverCoder1/github-readme-streak-stats">
  <img height="165" src="https://streak-stats.demolab.com?user=pranjitbis&hide_border=true" alt="GitHub Streak"/>
</a>

</div>

---

## ​ Featured Projects

- **Project A** — short description · [Live](#) · [Code](#)
- **Project B** — short description · [Live](#) · [Code](#)

*(Add as many as you'd like)*

---

## ​ Connect

[![Gmail Badge](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:YOUR_EMAIL)
[![LinkedIn Badge](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_LINKEDIN)
[![Twitter Badge](https://img.shields.io/badge/Twitter-000000?style=flat&logo=x&logoColor=white)](https://twitter.com/YOUR_TWITTER)

---

### ​​ Setup Contribution Snake (One-Time)

1. Ensure your repository is named **`pranjitbis`** (must match your GitHub username).
2. Add this file as `.github/workflows/snake.yml`:

```yaml
name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"   # runs daily at midnight UTC
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: pranjitbis
          outputs: |
            dist/snake.svg
      - name: Upload artifact
        uses: actions/upload-artifact@v4
        with:
          name: snake
          path: dist/snake.svg
      - name: Push to output branch
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
