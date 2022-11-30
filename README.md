<p align="center"> <img src="./logo/logofinal.png" alt="CATE" class="center" width=300/> </p>

<h1 align="center">CATE - Collect Analyze Treatment Exhibition</h1>

The project to be developed will be a health plan conciliation management system for the partner company [Dom Rock](https://www.domrock.net/) in conjunction with the College Fatec São José dos Campos Professor Jessen Vidal.

<h2 align="center">📋 Table of Contents</h2>

<!--ts-->
   * [Introduction](#cate---collect-analyze-treatment-exhibition)
   * [Features](#-features)
   * [Application Demo](#-application-demo)
   * [Project](#-project)
   * [Challenge](#-challenge)
   * [Solution](#-solution)
   * [Deliveries](#-deliveries)
   * [Running the System](#-running-the-system)
   * [Technologies](#-technologies)
   * [Members](#-members)
   * [Licenses](#-licenses)
   * [Project Dictionary](https://github.com/API-6-SEMESTRE/Documentation/blob/main/Files/dictionary.md)
<!--te-->

<h2 align="center">✅ Features</h2>

- [x] Bronze, Silver and Gold data processing levels
- [x] Data extraction
- [x] LOG of the data extraction process
- [x] Data cleaning
- [x] Raw data storage in MongoDB
- [x] Persistence process LOG in MongoDB
- [x] Data crossing
- [x] LOG of the data crossing process
- [x] Cross-data storage in MongoDB
- [x] Cross data storage in DW
- [x] Storing LOGs in MongoDB
- [x] Application of LGPD
- [x] Reports in Power BI
- [x] Bonus
  - [x] Machine Learning Implementation

<h2 align="center">📺 Application demo</h2>

<div align="center">

![Alt Text](./demonstration-application/dash_api.png)

</div>

<h2 align="center">🖥 Project</h2>

Project being developed in a partnership with Dom Rock, tech company that provides a platform which allows the capture of unstructured and structured data in an automated manner and promotes the optimized visualization of analyses, information, and data that enables recurring financial gains for various business areas of Dom Rock's clients. The platform was designed and built with the most advanced technologies of big data and artificial intelligence with self-scaling cloud architecture. In recent years the platform has been recognized as one of the best in Brazil by qualified rankings and through open innovation programs of large corporations and organizations.

<h2 align="center">📈 Challenge</h2>

Challenge proposed by Dom Rock - The client manages a health plan management system that has the following need: A solution that reconciles information from a health operator's demonstrative and the list of beneficiaries of that operator's health plans for each monthly competence. As the data contains personal information, the implementation of the LGPD (Brazilian General Data Protection Law) law is mandatory for audit purposes.

<h2 align="center">💡 Solution</h2>

CATE is the project that enables better data management, allowing for better performance, integrity, security, and privacy.
With a good data flow defined, it is possible to generate discrepancies reports and display them to the controller, allowing for quick correction.

<h2 align="center">💎 Deliveries</h2>

Below is the planning and progress during the project Sprints.

|   **SPRINT**    |  **DELIVERY DATE**  | **WHAT WILL BE DELIVERED** |
|-----------------|-----------------------|-------------------------|
|  1  |  08/29/2022 to 09/18/2022  | Data modeling, data processing levels (Bronze and Silver), data extraction from the bases, LOG of the extraction process, persistence of raw data in MongoDB, LOG of the persistence process in MongoDB.
|  2  |  09/19/2022 to 10/09/2022  | Cleaning of data extracted from the databases, analysis and cross-checking of data via Python and persistence of cross-data in MongoDB.
|  3  |  10/13/2022 to 11/06/2022  | LGPD application, DW modeling and implementation, cross-data persistence in DW, Power BI modeling and implementation, integration between DW and Power BI, reports in Power BI.
|  4  |  11/07/2022 to 27/11/2022  | Improvements and Machine Learning (bonus).

<h2 align="center">🚀 Running the System</h2>

<h3>📑 Prerequisites</h3>

Before starting, you will need installed in your machine the following tools:
[Git](https://git-scm.com), [Python](https://www.python.org/) and [PIP](https://pypi.org/project/pip/).
Besides this it is good to have an IDE to work with the code, for example [VSCode](https://code.visualstudio.com/) or [PyCharm](https://www.jetbrains.com/pt-br/pycharm/).

<h3>🎲 Running Python</h3>

```bash
# Clone this repository
$ git clone https://github.com/API-6-SEMESTRE/Projeto

# Run the following command in the terminal to isntall the PIP libraries
$ pip install -r src/requirements.txt

# Run the following commands:

## BRONZE Level - Extraction of data from spreadsheets and persistence in MongoDB with raw data
## Add "-v" to the end of the command to print the processing to the console
$ python3 src/et_l.py -l bronze

## SILVER level - Crossing the data that is already in MongoDB and persisting the cross-data in MongoDB
## Add "-v" to the end of the command to print the processing to the console
$ python3 src/et_l.py -l silver

## GOLD level - Process of loading the cross data that are in MongoDB to the DW
## Add "-v" to the end of the command to print the processing to the console
$ python3 src/et_l.py -l gold

## ALL level - Runs all processes in the sequence BRONZE > SILVER > GOLD
## Add "-v" to the end of the command to print the processing to the console
$ python3 src/et_l.py -l all

# Done!
```

<h2 align="center">🛠 Technologies</h2>

The following tools were used in building the project:

<p align="center">
 <a href="https://www.mongodb.com/">
  <img src="https://img.shields.io/static/v1?label=MongoDB&message=NoSQL Database&color=47A248&style=for-the-badge&logo=mongodb"/>
 </a>
 <a href="https://www.mysql.com/">
  <img src="https://img.shields.io/static/v1?label=MySQL&message=Relational Database&color=4479A1&style=for-the-badge&logo=mysql"/>
 </a>
 <a href="https://powerbi.microsoft.com/pt-br/">
  <img src="https://img.shields.io/static/v1?label=Power BI&message=Reports&color=F2C811&style=for-the-badge&logo=Power BI"/>
 </a>
</p>
<p align="center">
  <a href="https://www.python.org/">
  <img src="https://img.shields.io/static/v1?label=Python&message=Data Analysis&color=3776AB&style=for-the-badge&logo=Python"/>
</a>
<a href="https://pandas.pydata.org/">
  <img src="https://img.shields.io/static/v1?label=Pandas&message=Data Analysis&color=150458&style=for-the-badge&logo=pandas"/>
</a>
<a href="https://pypi.org/project/pip/">
  <img src="https://img.shields.io/static/v1?label=PIP&message=Data Analysis&color=3775A9&style=for-the-badge&logo=PyPI"/>
</a>
</p>
<p align="center">
  <a href="https://git-scm.com/">
  <img src="https://img.shields.io/static/v1?label=Git&message=DevOps&color=F05032&style=for-the-badge&logo=Git"/>
</a>
  <a href="https://github.com/">
  <img src="https://img.shields.io/static/v1?label=GitHub&message=DevOps&color=181717&style=for-the-badge&logo=GitHub"/>
</a>
<a href="https://www.atlassian.com/br/software/jira">
  <img src="https://img.shields.io/static/v1?label=Jira&message=Process&color=0052CC&style=for-the-badge&logo=Jira Software"/>
 </a>
 <a href="https://www.microsoft.com/pt-br/microsoft-teams/log-in">
  <img src="https://img.shields.io/static/v1?label=Microsoft Teams&message=Process&color=6264A7&style=for-the-badge&logo=Microsoft Teams"/>
 </a>
</p>

<h2 align="center">👥 Members</h2>

<table align="center">
    <tr>
        <td align="center">
            <a href="https://linkedin.com/in/tairik-nishimura/">
                <img style="border-radius: 50%;" src="./photos/tairik.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Tairik Johnny</b>
                </sub>
            </a>
            <br />
            <p>Scrum Master</p>
            <a href="[https://www.mongodb.com/](https://linkedin.com/in/tairik-nishimura/)">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://www.linkedin.com/in/maxx-barcelos-aaa106b2/">
                <img style="border-radius: 50%;" src="./photos/maximiles.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Maximiles Barcelos</b>
                </sub>
            </a>
            <br />
            <p>Product Owner</p>
            <a href="https://www.linkedin.com/in/maxx-barcelos-aaa106b2/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://www.linkedin.com/in/jeferson-tadeu-das-neves-a98343190/">
                <img style="border-radius: 50%;" src="./photos/jeferson.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Jeferson Neves</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://www.linkedin.com/in/jeferson-tadeu-das-neves-a98343190/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://linkedin.com/in/devanir-ramos-junior/">
                <img style="border-radius: 50%;" src="./photos/devanir.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Devanir Ramos</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://linkedin.com/in/devanir-ramos-junior/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
    </tr>
    <tr>
        <td align="center">
            <a href="https://www.linkedin.com/in/jos%C3%A9-francisco-forneiro-junior/">
                <img style="border-radius: 50%;" src="./photos/jose.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>José Francisco</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://www.linkedin.com/in/jos%C3%A9-francisco-forneiro-junior/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://www.linkedin.com/in/alan-bezerra/">
                <img style="border-radius: 50%;" src="./photos/alan.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Alan Lucas</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://www.linkedin.com/in/alan-bezerra/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://www.linkedin.com/in/leonardo-gabriel-silva-11b8b8178/">
                <img style="border-radius: 50%;" src="./photos/leonardo.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Leonardo Gabriel</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://www.linkedin.com/in/leonardo-gabriel-silva-11b8b8178/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://www.linkedin.com/in/henrique-zucareli-santiago/">
                <img style="border-radius: 50%;" src="./photos/henrique.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Henrique Zucareli</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://www.linkedin.com/in/henrique-zucareli-santiago/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
    </tr>
</table>

<h2 align="center">📝 License</h2>

All information resulting from Learning through Integrated Projects at Fatec São José dos Campos - Prof. Jessen Vidal follows the Open Source Initiative (OSI) or Academic Free License 3.0 (AFL-3.0) license.
