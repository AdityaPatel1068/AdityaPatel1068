# Generate a version of the README with text labels instead of icons

text_skills_readme = """
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
**Python**, **R**, **MySQL**, **Oracle**, **PostgreSQL**, **TensorFlow**, **PyTorch**

#### 📊 Visualization & Reporting
**Tableau**, **Power BI**, **Pandas**, **Matplotlib**

#### ☁️ Cloud & Platforms
**AWS**, **Azure**, **GCP**

#### 🗃️ Databases & ETL Tools
**MySQL**, **PostgreSQL**, **Oracle**

#### ⚙️ Version Control & DevOps
**Git**, **GitHub**

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

# Save the version with plain text skills
text_readme_path = Path("/mnt/data/README_text_skills.md")
text_readme_path.write_text(text_skills_readme)

text_readme_path.name
