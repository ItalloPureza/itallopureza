from pathlib import Path
from PIL import Image
import shutil, zipfile, os

base = Path("/mnt/data/itallo_github_profile")
assets = base / "assets"
assets.mkdir(parents=True, exist_ok=True)

source_banner = Path("/mnt/data/a_wide_cinematic_pixel_art_landscape_scene_at_nig.png")
banner_path = assets / "banner.png"
shutil.copy2(source_banner, banner_path)

readme = r'''<p align="center">
  <img src="assets/banner.png" alt="Pixel-art fantasy landscape in violet and cyan tones" width="100%" />
</p>

<h1 align="center">ÍTALLO.EXE</h1>

<p align="center">
  <strong>BI &amp; DATA ANALYTICS · SQL · PYTHON · POWER BI</strong>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/itallo-pureza99/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-7C5CFC?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://github.com/ItalloPureza">
    <img src="https://img.shields.io/badge/GitHub-Portfolio-30303B?style=flat-square&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <a href="mailto:purezaitallo@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact-30303B?style=flat-square&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>

<p align="center">
  <code>Curiosity.exe → Data → Insights → Impact</code>
</p>

---

## `01 // PLAYER PROFILE`

### EN

I'm **Ítallo Oliveira**, a Computer Science graduate based in Belo Horizonte, Brazil, working with **Business Intelligence, Data Analytics, data pipelines, APIs, and automation**.

I enjoy turning scattered information into reliable data products. For me, a dashboard is only the visible layer: trustworthy analytics also depends on extraction, transformation, persistence, modeling, business rules, validation, and the systems behind the data.

My focus is on connecting technical implementation with real business needs — building solutions that are understandable, maintainable, and useful for decision-making.

### PT-BR

Sou **Ítallo Oliveira**, bacharel em Ciência da Computação, de Belo Horizonte/MG, com experiência prática em **Business Intelligence, Análise de Dados, pipelines, APIs e automação**.

Gosto de transformar informações dispersas em soluções confiáveis. Um dashboard é apenas a camada visível: por trás de uma análise consistente existem extração, tratamento, armazenamento, modelagem, regras de negócio, validação e os sistemas que sustentam os dados.

Meu foco é conectar a implementação técnica às necessidades do negócio, construindo soluções úteis para análise e tomada de decisão.

```text
PLAYER       : Ítallo Oliveira
CLASS        : BI & Data Analytics
SPECIALTY    : SQL · Python · Power BI
SYSTEMS      : ETL · APIs · Integrations
AUTOMATION   : n8n · AI workflows
LOCATION     : Belo Horizonte, Brazil
MISSION      : Turn data into reliable decisions
```

## `02 // SKILL TREE`

<details>
<summary><strong>📊 BI & Analytics</strong></summary>

- Power BI dashboards and operational reporting
- Data modeling, DAX, and KPI definition
- SQL queries and relational data analysis
- Exploratory analysis and data validation
- Business rules and metric consistency
- Translating business questions into actionable insights

</details>

<details>
<summary><strong>⚙️ Data Engineering & ETL</strong></summary>

- Python-based extraction and transformation
- ETL workflows and data persistence
- MySQL and relational databases
- Historical data collection and analysis
- Data quality and consistency checks
- Investigating refresh, volume, and processing bottlenecks

</details>

<details>
<summary><strong>🔌 APIs & Integrations</strong></summary>

- REST API integrations and pagination
- Response handling and data validation
- Connecting business systems and services
- Troubleshooting errors and inconsistencies
- Technical documentation and integration reliability

</details>

<details>
<summary><strong>🤖 Automation & AI</strong></summary>

- Workflow automation with n8n
- Python scripts for repetitive tasks and validation
- API-driven automation
- Exploring practical AI applications in technical workflows
- Connecting data processes and business operations

</details>

## `03 // CURRENT LOADOUT`

<p>
  <img src="https://img.shields.io/badge/Python-30303B?style=for-the-badge&logo=python&logoColor=9B83FF" alt="Python" />
  <img src="https://img.shields.io/badge/SQL-30303B?style=for-the-badge&logo=mysql&logoColor=9B83FF" alt="SQL" />
  <img src="https://img.shields.io/badge/Power%20BI-30303B?style=for-the-badge&logo=powerbi&logoColor=9B83FF" alt="Power BI" />
  <img src="https://img.shields.io/badge/Power%20Query-30303B?style=for-the-badge&logo=microsoftpowerpoint&logoColor=9B83FF" alt="Power Query" />
  <img src="https://img.shields.io/badge/APIs-30303B?style=for-the-badge&logo=fastapi&logoColor=9B83FF" alt="APIs" />
  <img src="https://img.shields.io/badge/n8n-30303B?style=for-the-badge&logo=n8n&logoColor=9B83FF" alt="n8n" />
  <img src="https://img.shields.io/badge/AWS-30303B?style=for-the-badge&logo=amazonwebservices&logoColor=9B83FF" alt="AWS" />
  <img src="https://img.shields.io/badge/Git-30303B?style=for-the-badge&logo=git&logoColor=9B83FF" alt="Git" />
</p>

| Technology | How I use it |
|:--|:--|
| SQL / MySQL | Querying, organizing, and persisting data |
| Python | ETL, validation, integrations, and automation |
| Power BI / DAX | Data modeling, indicators, and dashboards |
| Power Query | Data preparation and transformation |
| REST APIs | Integrating systems and extracting information |
| n8n | Workflow automation |
| AWS | Cloud foundations and infrastructure concepts |
| Git / GitHub | Version control and project documentation |

## `04 // FEATURED QUEST`

### [Painel Operacional — Power BI](https://github.com/ItalloPureza/painel_operacional)

**A reusable operational BI model designed to bring sector indicators into one consistent experience.**

The starting problem was familiar: information spread across different systems, parallel spreadsheets, and teams reporting different numbers. When metrics disagree, meetings can turn into debates about which source is correct.

The project brings the experience together in a central operational dashboard:

- **Centralized overview:** a home page with the operational sectors and role-based visibility through Row-Level Security (RLS).
- **Goals vs. results:** targets and actual results presented together, with goals supplied through an internal API in the original implementation.
- **Historical team attribution:** results are associated with the team a person belonged to at the time, preserving historical interpretation when teams change.
- **Data freshness monitoring:** a data-health view indicating how current each source is.

The public portfolio version is intended to be reusable: it uses fictional data and a spreadsheet in place of the original database. A written guide is included to help people understand, maintain, and adapt the model, including with AI-assisted workflows.

**Technologies:** Power BI · Power Query · DAX · RLS · APIs · AWS · Python

> The demonstration uses fictional data. Company data, credentials, and confidential implementation details should never be included in the public repository.

**[Open the repository →](https://github.com/ItalloPureza/painel_operacional)**

## `05 // QUEST LOG`

These are recurring problem spaces from my professional experience — not claims of separate public projects.

- **Operational intelligence:** consolidating indicators and applying consistent business rules.
- **Data pipelines & historical analysis:** extracting, transforming, persisting, and validating data for reliable analysis over time.
- **Integration & data quality:** investigating APIs, comparing sources, and finding discrepancies.
- **Automation & reliability:** reducing manual work and improving the dependability of data processes.

## `06 // EDUCATION & CERTIFICATIONS`

- **B.Sc. in Computer Science** — completed in 2025
- **AWS Academy Graduate — Cloud Foundations**
- **CertiProf — Lifelong Learning**
- **Alura — Desenvolvendo com Inteligência: IA para Dev**

## `07 // PASSIVE SKILLS`

```text
[+] Analytical thinking
[+] Troubleshooting
[+] Data storytelling
[+] Systems thinking
[+] Technical communication
[+] Continuous improvement
[+] Business-oriented problem solving
```

I care about more than making something work once. I want to understand why it works, where it can fail, how it scales, and whether the result can be trusted.

## `08 // OUTSIDE THE TERMINAL`

When I'm away from data and technical problems, I'm usually exploring games and the systems behind them:

- 🎮 RPGs and immersive worlds
- 🕹️ Retro games and nostalgia
- 🎨 Indie games and creative experiences
- 🎮 Nintendo and classic games
- 🧱 Minecraft, exploration, and building

Maybe that's part of the connection: I enjoy exploring systems, understanding their rules, and discovering different ways to solve problems.

## `09 // CONNECT`

- **LinkedIn:** [linkedin.com/in/itallo-pureza99](https://www.linkedin.com/in/itallo-pureza99/)
- **GitHub:** [github.com/ItalloPureza](https://github.com/ItalloPureza)
- **Email:** [purezaitallo@gmail.com](mailto:purezaitallo@gmail.com)
- **Location:** Belo Horizonte, MG, Brazil

---

<p align="center">
  <strong>Curiosity is the engine. Data is the map. Solutions are the objective.</strong>
</p>

<p align="center">
  <code>END OF TRANSMISSION // ITALLO.EXE</code>
</p>
'''

(base / "README.md").write_text(readme, encoding="utf-8")

zip_path = Path("/mnt/data/Itallo_GitHub_Profile_Package.zip")
with zipfile.ZipFile(zip_path, "w", zipfile.ZIP_DEFLATED) as z:
    z.write(base / "README.md", "README.md")
    z.write(banner_path, "assets/banner.png")

print("Created files:")
print(f"README: {base / 'README.md'}")
print(f"Banner: {banner_path}")
print(f"ZIP package: {zip_path}")
