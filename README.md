# Paso 1: Configuración de Git

```bash
git config --global user.name "Carlos Contreras"
git config --global user.email "A100154945@my.uvm.edu.mx"
```

# Paso 2: Creación y Gestión del Repositorio

## 4. Inicializar el repositorio local
```bash
mkdir proyecto-control-versiones
cd proyecto-control-versiones
git init
```

## 5. Crear y configurar el README
```bash
echo "# Proyecto de Control de Versiones
Este proyecto demuestra el uso de Git y GitHub para el control de versiones en ingeniería de software." > README.md
git add README.md
git commit -m "Agrega archivo README inicial"
```

## 6. Conectar con GitHub
```bash
git remote add origin https://github.com/tuusuario/proyecto-control-versiones.git
git branch -M main
git push -u origin main
```

# Parte 3: Trabajo Colaborativo y Uso de Ramas

## 7. Crear una nueva rama para una funcionalidad
```bash
git checkout -b feature
echo "Esta es una funcionalidad nueva que será implementada." > funcionalidad.txt
git add .
git commit -m "Agrega nueva funcionalidad en la rama feature"
git push origin feature
```

## 8. Crear un Pull Request
- Abrir GitHub y crear un Pull Request desde la rama `feature` hacia `main`.
- Incluir descripción detallada de los cambios realizados.

## 9. Merge y limpieza de ramas
- Realizar el merge del PR en la rama `main` desde GitHub.
- Eliminar la rama `feature` desde la interfaz de GitHub.

# Parte 4: Gestión de Issues y Documentación

## 10. Crear y gestionar issues
- Crear un Issue simulando una mejora o error.
- Etiquetarlo, asignarle un milestone y comentar una posible solución.

## 11. Documentar la experiencia
```bash
echo "# EXPERIENCIA.md
Durante esta actividad aprendí a configurar Git, usar ramas, conectar con GitHub y gestionar colaboraciones. Las principales dificultades fueron aprender los comandos y comprender el flujo de trabajo entre local y remoto." > EXPERIENCIA.md
git add EXPERIENCIA.md
git commit -m "Agrega archivo EXPERIENCIA.md con reflexiones"
git push origin main
```

## 11.1 Documentar investigación (reporte académico)
```bash


El control de versiones es un sistema que registra los cambios realizados en un archivo o conjunto de archivos a lo largo del tiempo, permitiendo recuperar versiones específicas más adelante. Es esencial en el desarrollo de software porque facilita la colaboración, el seguimiento de cambios y la prevención de errores cuando múltiples desarrolladores trabajan sobre el mismo proyecto.



1. Git
2. GitHub
3. GitLab
4. Bitbucket
5. Subversion (SVN)


GitHub es una plataforma de desarrollo colaborativo basada en Git. Permite alojar repositorios, hacer seguimiento de errores, gestionar versiones y colaborar con otros desarrolladores.



- Se creó cuenta de GitHub
- Se instaló Git en macOS
- Se configuró Git con nombre y correo del estudiante



- Se creó carpeta local y repositorio con `git init`
- Se creó archivo README.md
- Se conectó con GitHub
- Se creó una rama llamada `feature` y se desarrolló una funcionalidad
- Se creó Pull Request, se hizo merge y se limpió la rama



El control de versiones es una herramienta fundamental en la ingeniería de software moderna. Permite gestionar cambios, colaborar eficientemente y mantener la integridad del código. Git y GitHub son herramientas populares y poderosas que mejoran la organización y la calidad del desarrollo de software.



- Git SCM: https://git-scm.com/
- GitHub Docs: https://docs.github.com/
- Atlassian: https://www.atlassian.com/git/tutorials
- Pro Git Book: https://git-scm.com/book/en/v2" > REPORTE.md
git add REPORTE.md
git commit -m "Agrega archivo REPORTE.md con investigación sobre control de versiones"
git push origin main
```

# Parte 5: Extensiones y Exploración Avanzada (Opcional)

## 12. Explorar GitHub Pages
- Investigar cómo activar GitHub Pages desde la pestaña "Pages" en configuración del repositorio.
- Seleccionar la rama `main` y la carpeta raíz (`/root`) para publicar la página.

## 13. GitHub Actions para CI
- Explorar cómo crear un archivo `.github/workflows/main.yml` con una acción básica de validación o test.
