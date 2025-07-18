# Update the logo base path to reflect the latest branch 'main' instead of a specific commit hash
base_logo_url_main = "https://raw.githubusercontent.com/gilbarbara/logos/main/logos"

# Redefine logos with updated paths
logos_main = {
    "Python": f"{base_logo_url_main}/python.svg",
    "R": f"{base_logo_url_main}/r-lang.svg",
    "MySQL": f"{base_logo_url_main}/mysql.svg",
    "Oracle": f"{base_logo_url_main}/oracle.svg",
    "PostgreSQL": f"{base_logo_url_main}/postgresql.svg",
    "TensorFlow": f"{base_logo_url_main}/tensorflow.svg",
    "PyTorch": f"{base_logo_url_main}/pytorch-icon.svg",
    "Tableau": f"{base_logo_url_main}/tableau-software.svg",
    "Power BI": f"{base_logo_url_main}/power-bi.svg",
    "AWS": f"{base_logo_url_main}/amazon-web-services.svg",
    "Azure": f"{base_logo_url_main}/microsoft-azure.svg",
    "GCP": f"{base_logo_url_main}/google-cloud.svg",
    "Git": f"{base_logo_url_main}/git-icon.svg",
    "GitHub": f"{base_logo_url_main}/github-icon.svg",
    "Pandas": f"{base_logo_url_main}/pandas-icon.svg",
    "Matplotlib": f"{base_logo_url_main}/matplotlib-icon.svg"
}

# Generate table rows for categorized skills
def make_skill_table(skill_list):
    cells = "".join(f'<td align="center"><img src="{logos_main.get(skill, "")}" height="40"/><br>{skill}</td>' for skill in skill_list)
    return f"<table><tr>{cells}</tr></table>"

# Final README content with logo URLs from friend's repo
final_readme_with_friend_logos = f"""
<h1 align="center">Hey! 👋 I'm Aditya Patel</h1>
<h3 align="center">Data Scientist | Machine Learning | Real-Time Analytics | Big Data</h3>

<p align="center">
  <a href="https://github.com/AdityaPatel1068" target="_blank">GitHub</a> • 
  <a href="https://www.linkedin.com/in/adityapatel2609/" target="_blank">LinkedIn</a> • 
  <a href="mailto:adityapatelcareer@gmail.com">Email</a> • 
  <a href="https://theadityapatel.com" target="_blank">Portfolio</a>
</p>

---

### 🧠 About Me
Hi, I'm Aditya — a Data Scientist with hands-on experience in healthcare, finance, and retail domains, specializing in predictive modeling, data engineering, and real-time analytics. I’ve designed and deployed end-to-end ML pipelines using tools like **Apache NiFi, Talend, Snowflake, Power BI**, and **AWS**, focusing on cost-efficiency, compliance, and scalability.

---

### 🎓 Education

#### 🎓 Master of Science in Data Science (2023 – 2024)
**New Jersey Institute of Technology** — CGPA: 4.0  
Coursework: ML, Applied Stats, Data Mining, Cloud, Big Data, Visualization, Python for ML

#### 🎓 B.Tech. in Mechanical Engineering (2015 – 2019)
**Dr. A.P.J. Abdul Kalam Technical University** — CGPA: 3.2  

---

### 💻 Technical Skills

#### 🧮 Languages, Libraries & Frameworks
{make_skill_table(["Python", "R", "MySQL", "Oracle", "PostgreSQL", "TensorFlow", "PyTorch"])}

#### 📊 Visualization & Reporting
{make_skill_table(["Tableau", "Power BI", "Pandas", "Matplotlib"])}

#### ☁️ Cloud & Platforms
{make_skill_table(["AWS", "Azure", "GCP"])}

#### ⚙️ Version Control & DevOps
{make_skill_table(["Git", "GitHub"])}

---

### 🚀 Featured Projects

- 🔤 **ASL Interpreter**: Real-time deep learning model for sign language → 96% accuracy  
- 🧪 **AI Grading Engine**: OCR + GPT + Cheating Pattern Detection for handwritten answer sheets  
- 🌎 **Climate Trend Modeler**: ViT + UNet to forecast temperature fluctuations from climate data  
- 🎥 **Harmful Algal Bloom Predictor**: Detects blooms using satellite data + geospatial ML  
- 🎬 **IMDB Movie Analysis**: Movie trend analytics using IMDb and Rotten Tomatoes datasets  

---

### 📈 GitHub Activity

![snake gif](https://github.com/AdityaPatel1068/AdityaPatel1068/blob/output/github-snake-dark.svg)

---

### 📬 Contact Me

- 📧 **Email**: [adityapatelcareer@gmail.com](mailto:adityapatelcareer@gmail.com)  
- 💼 **LinkedIn**: [linkedin.com/in/adityapatel2609](https://linkedin.com/in/adityapatel2609)  
- 🌐 **Portfolio**: [theadityapatel.com](https://theadityapatel.com)  
- 🧠 **LeetCode**: [leetcode.com/Rexus_Reborn](https://leetcode.com/Rexus_Reborn/) — *123 solved*
"""

# Save the final version with friend's GitHub-hosted icons
friend_logo_readme_path = Path("/mnt/data/README_friend_icons.md")
friend_logo_readme_path.write_text(final_readme_with_friend_logos)

friend_logo_readme_path.name
