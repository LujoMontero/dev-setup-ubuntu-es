<div align="center">

# ⚙️ Dev Setup Ubuntu ES

### Scripts de configuración de entorno de desarrollo en Ubuntu / WSL

![Shell](https://img.shields.io/badge/Shell_Script-121011?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu_20.04+-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

</div>

---

## 📌 ¿Qué hace este proyecto?

Colección de scripts Shell modulares para configurar un entorno de desarrollo completo en Ubuntu o WSL desde cero. Cada herramienta tiene su propio script independiente, comentado y seguro, listo para ejecutar paso a paso.

---

## 🗂️ Scripts incluidos

```
scripts/
├── 01-instalacion-base.sh     # Actualiza el sistema y prepara el entorno
├── 02-instalar-zsh.sh         # Instala zsh como shell predeterminada
├── 03-configurar-zsh.sh       # Instala Oh My Zsh + plugins útiles
├── 04-instalar-git.sh         # Git con usuario, correo y plantilla de commits
├── 05-instalar-ssh.sh         # Genera claves SSH para GitHub
├── 06-instalar-ruby.sh        # Ruby con rbenv (versión seleccionable)
├── 07-instalar-node.sh        # Node.js con nodenv
├── 08-instalar-python.sh      # Python con pyenv + paquetes esenciales
├── 09-instalar-java.sh        # Java LTS + Maven con SDKMAN
├── 10-instalar-postgresql.sh  # PostgreSQL oficial (v16/v17)
├── 11-instalar-docker.sh      # Docker + Docker Compose
├── 12-instalar-terraform.sh   # Terraform (IaC)
└── 13-instalar-kubernetes.sh  # kubectl + herramientas K8s
```

---

## ⚙️ Requisitos

- Ubuntu 20.04+ o WSL2
- Conexión a internet
- Permisos de superusuario (`sudo`)
- Terminal con `bash` o `zsh`

---

## 🚀 Instalación

```bash
# 1. Clonar el repositorio
git clone https://github.com/LujoMontero/dev-setup-ubuntu-es.git
cd dev-setup-ubuntu-es

# 2. Dar permisos de ejecución a todos los scripts
chmod +x scripts/*.sh

# 3. Ejecutar el script base (obligatorio primero)
./scripts/01-instalacion-base.sh
```

---

## ▶️ Ejecución paso a paso

```bash
# Shell y terminal
./scripts/02-instalar-zsh.sh

# ⚠️ Cierra y vuelve a abrir la terminal antes de continuar

./scripts/03-configurar-zsh.sh

# Herramientas de desarrollo
./scripts/04-instalar-git.sh
./scripts/05-instalar-ssh.sh

# Lenguajes (instala solo los que necesites)
./scripts/06-instalar-ruby.sh
./scripts/07-instalar-node.sh
./scripts/08-instalar-python.sh
./scripts/09-instalar-java.sh

# Base de datos y contenedores
./scripts/10-instalar-postgresql.sh
./scripts/11-instalar-docker.sh

# DevOps (opcional)
./scripts/12-instalar-terraform.sh
./scripts/13-instalar-kubernetes.sh
```

---

## 📋 Tabla de herramientas instaladas

| Script | Herramienta | Gestor de versiones |
|---|---|---|
| 02-03 | zsh + Oh My Zsh | — |
| 04 | Git | — |
| 05 | SSH keys | — |
| 06 | Ruby | rbenv |
| 07 | Node.js | nodenv |
| 08 | Python | pyenv |
| 09 | Java + Maven | SDKMAN |
| 10 | PostgreSQL 16/17 | repositorio oficial |
| 11 | Docker + Compose | repositorio oficial |
| 12 | Terraform | repositorio HashiCorp |
| 13 | kubectl | repositorio oficial |

---

## 💡 Recomendación de uso

Ejecuta los scripts **en orden** si estás configurando un sistema desde cero. Si ya tienes algunas herramientas instaladas, puedes ejecutar solo los scripts que necesites de forma independiente, sin riesgo de romper configuraciones existentes.

---

## 🤝 Contribuir

```bash
# Fork → crea tu rama → cambios → commit → Pull Request
git checkout -b feature/nuevo-script
git commit -m "feat: agregar script para instalar X"
git push origin feature/nuevo-script
```

---

## 📄 Licencia

MIT — ver [LICENSE](./LICENSE)

---

## 👨‍💻 Autor

**Luis Montero** · [GitHub](https://github.com/LujoMontero) · [LinkedIn](https://www.linkedin.com/in/luis-montero-if/)
