<div align="center">

# 🌐 websimple1

**A static site plus a Flask API, packaged in one Docker image — the payload deployed by the CloudFormation stack.**
*Sitio estático más una API Flask, empaquetados en una imagen Docker: la carga que despliega el stack de CloudFormation.*

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)

</div>

---

## 🌟 What it is

A landing page built on the **Salient** HTML template, bundled with the [students Flask API](https://github.com/Osomar1705/api-student) and a `Dockerfile`.

This repository is cloned into `/var/www/html` at boot by the `UserData` script in [**cf-mv-2webs**](https://github.com/Osomar1705/cf-mv-2webs), which is how it ends up being served from an EC2 instance.

---

## 🚀 Run it

```bash
docker build -t websimple1 .
docker run -p 8080:80 websimple1     # http://localhost:8080
```

Or just open `index.html` in a browser for the static side.

---

## 🇪🇸 En español

Landing page basada en la plantilla HTML **Salient**, empaquetada junto a la [API Flask de estudiantes](https://github.com/Osomar1705/api-student) y su `Dockerfile`.

El script `UserData` de [**cf-mv-2webs**](https://github.com/Osomar1705/cf-mv-2webs) clona este repositorio dentro de `/var/www/html` al arrancar la instancia EC2 — así es como termina sirviéndose en AWS.

> 📌 Trabajo del curso de **Cloud Computing (UTEC)**. Archivado, pero sigue siendo clonable por la plantilla.

---

<div align="center">

[**Osmar Vilchez Aguirre**](https://github.com/Osomar1705) · UTEC 🇵🇪

</div>
