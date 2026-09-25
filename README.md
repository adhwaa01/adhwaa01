<h1 align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&pause=1000&color=2ECC71&center=true&vCenter=true&width=600&lines=Hi%2C+I'm+Adhwaa+Rajib+Aqiilah+%F0%9F%91%8B;Software+Engineering+Student;Fullstack+Developer;Problem+Solver" alt="Typing SVG" />
  </a>
</h1>

---

name: Generate Snake Animation
 
on:
  schedule:
    - cron: "0 0 * * *"   # tiap hari jam 00:00 UTC
  workflow_dispatch:
  push:
    branches:
      - main
 
jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    steps:
      - name: Generate the snake SVG
        uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
 
      - name: Push output to "output" branch
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 

---

### 👩‍💻 About Me

Mahasiswa Software Engineering yang fokus membangun aplikasi *fullstack* untuk menyelesaikan masalah nyata di lapangan — mulai dari manajemen bengkel, antrean digital BBM, hingga e-commerce UMKM. Tertarik mendalami arsitektur software yang scalable dan mulai eksplorasi IoT & AI/ML.

- 🔭 Sedang mengerjakan **IoT Healthcare Project**
- 🌱 Sedang memperdalam **Software Architecture** & **REST API design**
- 💬 Ajak diskusi soal: **Laravel, React, sistem digitalisasi**
- ⚡ Fun fact: *(Hmm.....)*

---

### 🛠️ Tech Stack

**Languages**
<p>
  <img src="https://skillicons.dev/icons?i=php,js,python,mysql" />
</p>

**Frameworks & Tools**
<p>
  <img src="https://skillicons.dev/icons?i=laravel,react,nodejs,flask,flutter,postgres,git,github,postman,figma" />
</p>

---

### 🚀 Featured Projects

<table>
  <tr>
    <td width="50%">
      <h4>🔧 Workshop Management System</h4>
      <p>Sistem manajemen bengkel untuk mengelola operasional harian secara digital.</p>
      <p><b>Stack:</b> Laravel · MySQL</p>
      <a href="#">🔗 Repo</a>
    </td>
    <td width="50%">
      <h4>🏍️ BengkelMotorWRT</h4>
      <p>Pencatatan transaksi dan inventori bengkel motor secara real-time.</p>
      <p><b>Stack:</b> Laravel · MySQL</p>
      <a href="#">🔗 Repo</a>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h4>⛽ MigasQueue</h4>
      <p>Digitalisasi antrean pengisian gas & pelaporan discrepancy transaksi.</p>
      <p><b>Stack:</b> React · Node.js · PostgreSQL</p>
      <a href="#">🔗 Repo</a>
    </td>
    <td width="50%">
      <h4>👕 Lapak Baju Bandung</h4>
      <p>Digitalisasi bisnis fashion lokal menjadi platform e-commerce.</p>
      <p><b>Stack:</b> Laravel · MySQL</p>
      <a href="#">🔗 Repo</a>
    </td>
  </tr>
  <tr>
    <td width="50%" colspan="2">
      <h4>🩺 IoT Healthcare Project <i>(On Going)</i></h4>
      <p>Sistem monitoring kesehatan berbasis IoT untuk deteksi dini kondisi pasien.</p>
      <p><b>Stack:</b> Flutter · Python · IoT Sensors</p>
      <a href="#">🔗 Repo</a>
    </td>
  </tr>
</table>

---

### 📚 Currently Learning

`Backend Development` `Frontend Development` `Fullstack Development` `REST API` `Software Architecture` `IoT` `AI & Machine Learning`

---



<p align="center"><i> From Adhwaa's GitHub — thanks for stopping by!</i></p>
