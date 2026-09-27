<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:00ff9f&height=200&section=header&text=Abdalrheem%20Nail&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Break%20it.%20Understand%20it.%20Build%20it%20better.&descAlignY=58&descSize=18" alt="Abdalrheem Nail" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/r7eam">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=00FF9F&center=true&vCenter=true&width=650&lines=Cybersecurity+Engineer;Vulnerability+Researcher+%40+HackerOne;Found+a+bug+in+AWS+VPC+CNI+%F0%9F%90%9B;Top+10+%40+SulyCyberCon+CTF+2025+%F0%9F%9A%A9;Full-Stack+Developer" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <a href="https://hackerone.com/r7eam"><img src="https://img.shields.io/badge/HackerOne-@r7eam-494649?style=for-the-badge&logo=hackerone&logoColor=white" alt="HackerOne" /></a>
  <a href="https://linkedin.com/in/r7eam"><img src="https://img.shields.io/badge/LinkedIn-r7eam-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:aabdalrheem5@gmail.com"><img src="https://img.shields.io/badge/Email-aabdalrheem5%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://x.com/r7eem_17"><img src="https://img.shields.io/badge/X-@r7eem__17-000000?style=for-the-badge&logo=x&logoColor=white" alt="X" /></a>
  <a href="https://leetcode.com/r7eam"><img src="https://img.shields.io/badge/LeetCode-r7eam-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=r7eam&label=Profile%20views&color=00ff9f&style=flat-square" alt="Profile views" />
</p>

---

### `root@r7eam:~# whoami`

```yaml
name:       Abdalrheem Nail
role:       Cybersecurity Engineer & Independent Vulnerability Researcher
degree:     B.Eng. Cybersecurity — Northern Technical University (2026)
based_in:   Iraq 🇮🇶
focus:      [vulnerability research, source code review, detection engineering, full-stack]
hunting_on: HackerOne (@r7eam)
languages:  { arabic: native, english: intermediate }
motto:      "To defend a system, first learn how to break it."
```

---

### 🐛 `root@r7eam:~# cat findings.log`

| Target | Vulnerability | Severity | Status |
| :-- | :-- | :-: | :-: |
| **AWS** · [`amazon-vpc-cni-k8s`](https://github.com/aws/amazon-vpc-cni-k8s) | Missing bounds check in `DelNetwork` → `aws-node` panic (node-level CNI DoS) | ![Medium](https://img.shields.io/badge/Medium-FFA500?style=flat-square) | ![Resolved](https://img.shields.io/badge/Resolved-2EA043?style=flat-square) |

<details>
<summary><b>📄 Read the write-up summary</b></summary>
<br />

- **Where:** the gRPC `DelNetwork` handler in the AWS VPC CNI plugin for Kubernetes (EKS).
- **Bug:** a missing `return` after a validation check let execution continue with a malformed
  `vpc.amazonaws.com/pod-eni` annotation.
- **Impact:** an index-out-of-bounds panic crashes the `aws-node` DaemonSet, taking down pod
  networking for the whole node — a node-level denial of service.
- **Proof:** reproduced on a live EKS cluster.
- **Outcome:** reported through HackerOne and **fixed in VPC CNI v1.23.0**.

</details>

---

### 🏆 `root@r7eam:~# git log --oneline --graph achievements`

```text
* 2026        🐛  Resolved AWS vulnerability (amazon-vpc-cni-k8s) via HackerOne
* Apr 2026    🎓  Graduated — B.Eng. Cybersecurity, Northern Technical University
* 2025        🚩  Top 10 — SulyCyberCon CTF Competition
* 2025        🚩  Finalist — MOI CTF
* 2025        💻  Full-Stack Web Development Trainee — QAF Lab (Tech Hub Bootcamp)
*             🚩  Participant — 2nd National Cybersecurity Competition (CTF), Iraq
* 2024        🏅  Certificate of Achievement — Information Security & AI Competition, University of Mosul
```

---

### 📜 Certifications

<p align="left">
  <img src="https://img.shields.io/badge/CAPT-Certified_Associate_Penetration_Tester-00ff9f?style=for-the-badge&labelColor=0d1117" alt="CAPT" />
  <img src="https://img.shields.io/badge/CORE-Certified_Cybersecurity_Foundation-00ff9f?style=for-the-badge&labelColor=0d1117" alt="CORE" />
</p>
<p align="left">
  <img src="https://img.shields.io/badge/Cisco-Introduction_to_Cybersecurity-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white" alt="Cisco Introduction to Cybersecurity" />
  <img src="https://img.shields.io/badge/QAF_Lab-Full_Stack_Developer-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="QAF Lab Full Stack Developer" />
</p>

<sub>CAPT and CORE issued by Hackviser.</sub>

---

### 🛠️ Featured Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>🍯 Universal Login Honeypot & Deception Framework</h4>
      <sub><i>Graduation project</i></sub>
      <p>A deception platform that lures attackers into fake login surfaces and streams every
      interaction into a SIEM pipeline — with Python enrichment, real-time Kibana dashboards,
      and webhook alerting.</p>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
      <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
      <img src="https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white" />
      <img src="https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white" />
      <img src="https://img.shields.io/badge/Kibana-E8478B?style=flat-square&logo=kibana&logoColor=white" />
      <img src="https://img.shields.io/badge/NGINX-009639?style=flat-square&logo=nginx&logoColor=white" />
      <img src="https://img.shields.io/badge/Docker_Compose-2496ED?style=flat-square&logo=docker&logoColor=white" />
    </td>
    <td width="50%" valign="top">
      <h4>📱 Al-Nukhba App</h4>
      <sub><i>Frontend development</i></sub>
      <p>Mobile frontend with responsive layouts, usability-focused screens, and clean navigation.</p>
      <img src="https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
      <h4>🎬 Movie Platform</h4>
      <sub><i>University project</i></sub>
      <p>Full-stack movie platform backed by a MySQL schema designed for accurate, efficient reporting.</p>
      <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
    </td>
  </tr>
</table>

---

### 🧰 Arsenal

| Domain | Skills |
| :-- | :-- |
| 🔍 **Vulnerability Research** | Source code review · Bug bounty (HackerOne) · Responsible disclosure · Kubernetes / AWS EKS |
| ⚔️ **Offensive Security** | Penetration testing · Kali Linux · CTF competitions |
| 🛡️ **Defensive Security** | Threat detection · Network monitoring · Anomaly detection · Honeypots & deception · Secure system design |
| 📈 **SIEM & Monitoring** | Elasticsearch · Kibana · Log analysis · Webhook alerting |

<p align="left">
  <img src="https://skillicons.dev/icons?i=py,js,ts,cpp,bash,html,css&perline=12" alt="Languages" />
  <br />
  <img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,nestjs,django,tailwind,mysql,mongodb&perline=12" alt="Web stack" />
  <br />
  <img src="https://skillicons.dev/icons?i=linux,kali,docker,kubernetes,aws,nginx,elasticsearch,git&perline=12" alt="Security and infrastructure" />
</p>

---

### 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=r7eam&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true" alt="GitHub stats" height="170" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=r7eam&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages" height="170" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=r7eam&theme=tokyonight&hide_border=true" alt="GitHub streak" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=r7eam&theme=tokyo-night&hide_border=true&area=true" alt="Contribution graph" width="100%" />
</p>

---

### 🐍 Contribution Snake

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/r7eam/r7eam/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/r7eam/r7eam/output/github-snake.svg" />
    <img alt="Contribution snake animation" src="https://raw.githubusercontent.com/r7eam/r7eam/output/github-snake.svg" />
  </picture>
</p>

---

<p align="center">
  <b>🔐 Found something? Want to collaborate on security research?</b><br />
  <a href="mailto:aabdalrheem5@gmail.com">aabdalrheem5@gmail.com</a> · responsible disclosure always welcome
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:00ff9f,100:0d1117&height=120&section=footer" alt="Footer" width="100%" />
</p>
