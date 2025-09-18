# 1. Desarrollo de un Sistema de Gestión de Ventas para TechZone 🛒

## 1.1. Problematica ⚠️
### La empresa TechZone enfrenta dificultades en la gestión de sus ventas debido a procesos manuales y poco organizados. Actualmente, el registro de clientes, productos y transacciones se realiza en hojas de cálculo y documentos físicos, lo que genera errores frecuentes, duplicidad de información y pérdida de tiempo en la atención al cliente.
### Además, la falta de un sistema centralizado impide un adecuado control de inventario y limita la capacidad de generar reportes en tiempo real para la toma de decisiones estratégicas.

## 1.2. Objetivos 🎯
### 1.2.1. Objetivo General
#### Desarrollar un Sistema de Gestión de Ventas para TechZone que permita automatizar y optimizar el registro de clientes, productos e inventario, mejorando la eficiencia operativa y facilitando la toma de decisiones.

### 1.2.2 Objetivos Especificos. 
* Proporcionar una interfaz amigable que facilite el uso del sistema de TechZone.
* Implementar un flujo de trabajo con Git para llevar control de versiones del sistema durante todo el desarrollo.
* Centralizar el código en GitHub para facilitar la colaboración, respaldo y visibilidad del proyecto.
* Configurar un archivo .gitignore para excluir archivos innecesarios del repositorio.

## 1.3. Requerimientos 📜
|Funcionales|No Funcionales|
|-----------|--------------|
|El sistema debe de ser responsive|Los comandos deberan estar en Git|
|El cliente podra agregar producto al carrito|El README tendra todo el proceso de desarrollo|
|El sistema tendra una ventana de login|Los commits deberán tener mensajes claros y descriptivos|
|El cliente podra actualizar sus datos personales|Se deberán usar pull requests para revisión de código antes de fusionar cambios|
|El sistema tendra un libro de reclamaciones|Los archivos sensibles deberán ser excluidos con `.gitignore`|
|El sistema brindara un resumen de compra al finalizar la venta|Se deberán etiquetar versiones estables con tags en Git|

## 1.4. Tecnologias utilizadas 💻
* java/html/javaScript/css.
* Git/GitHub.
* Visual Studio Code

## 1.5. Instalacion y Ejecucion ▶️
```bash
git clone "enlace URL del remote"
```
![URL del GitHub](imgMarkdown/URLgitClone.png)
![Comando git clone](imgMarkdown/gitClone.png)

## 1.6. Roles y Creditos 👥
|N°|Nombre|Rol|Funciones|
|--|------|---|---------|
|1|Luciano|Git Master|Control de Versiones|
|2|Peter|Dev Backend|Implementacion de APIs|
|3|Sheroo|Dev Frontend|Diseño con CSS|
# 2. Flujo de trabajo GIT
## 2.1. Configuración de identidad
### Comandos
```bash
git config --global user.name "Tu Nombre"
```
```bash
git config --global user.email "tuemail@example.com" 
```
![Comando de identidad](imgMarkdown/configIdentidad.png)

## 2.2. Verificar que la carpeta este creada
![Imagen de carpeta creada](imgMarkdown/carpetaHDW.png)

## 2.3. Abriendo proyecto desde GitBash
### Crear carpeta del proyecto
```bash
mkdir "Nombre del Proyecto"
```
### Entrar a la carpeta
```bash
cd "Nombre de la carpeta"
```
![Comando desde GitBash](imgMarkdown/abriendoProyecto.png)

## 2.4. Inicializando GIT en la carpeta “Proyecto_HDW”
```bash
git init
```
![Comando para inicializar](imgMarkdown/initHDW.png)

## 2.5. Primer archivo “README.md” referido al primer commit
### Para ingresar texto (echo "") y sea dirigido (>) a README.md
```bash
echo "# TEXTO" > README.md
```
### Agregar el archivo (add.)
```bash
git add. "indica que se agregara"
```
### Realizar el COMMIT
```bash
git commit -m "como se llamara el commit"
```
![Primer commit ](imgMarkdown/primerCommit.png)

## 2.6. Agregando “LICENSE” y “.gitignore”
### Agregar LICENSE
```bash
touch LICENSE
```
### Agregar .gitignore
```bash 
touch .gitignore
```
### Verificar si esta o no agregado (add.)
```bash
git status
```
![comando para agregar license y gitignore](imgMarkdown/licenseGitignore.png)

## 2.7. Repositorio local GIT al remoto GitHub
### Conectar al remoto
```bash
git remote add origin "URL del repositorio"
```
### Verificar el vinculo del repositorio
```bash
git remote -v
```
![del local al remoto](imgMarkdown/gitGitHub.png)

## 2.8. Clases y su commit
### Ver el estado
```bash
git status
```
### Agregar
```bash
git add .
```
### Realizar el segundo COMMIT
```bash
git commit -m "como se llama el commit"
```
![segundo commit](imgMarkdown/segundoCommit.png)

## 2.9. Ramas en Git a GitHub
### Crear rama
```bash
git checkout -b "Nombre de la rama"
```
### Volver a la rama principal
```bash
git git switch main
```
![Comando para crear rama](imgMarkdown/Ramas.png)

### Verificar ramas creadas 
```bash
git branch
```
### Subir ramas a GitHub
```bash
git push --all origin
```
![Comando para mostrar y subir ramas](imgMarkdown/verYsubirRamas.png)
![Ramas de GitHub](imgMarkdown/ramasDeGithub.png)

## 2.10. Auditar archivos
### Lista de archivos del proyecto
```bash
git ls-files
```
![Comando para auditar archivos](imgMarkdown/auditarArchivos.png)

## 2.11. Viendo commits  y el ID de commits
### ver commit
```bash
git log --oneline
```
### Ver detalle de commit
```bash
git show <ID de commit>
```
![Comando para ver el detalle del commit](imgMarkdown/IDcommits.png)

## 2.12. Primera version
### Subir al remoto
```bash
git push origin "nombre de la rama"
```
### Subir la version
```bash
git tag -a "numero de version" -m "nombre del commit"
```
### Subir la version
```bash
git push origin "numero de version"
```
![Comando para poner version parte 1](imgMarkdown/versionParte1.png)
![Comando para poner version parte 2](imgMarkdown/versionParte2.png)

## 2.13. Compare & pull request
![pull request 1](imgMarkdown/pull1.png)
![pull request 2](imgMarkdown/pull2.png)
![pull request 3](imgMarkdown/pull3.png)

## 2.14. Ramas fucionada y no fucionadas
### Fucionar ramas
```bash
git pull origin main
```
![Comando pull](imgMarkdown/pullGit.png)
### Validando ramas 
```bash
git branch --no-merged
```
```bash
git branch --merged
```
![Comando merged](imgMarkdown/merged.png)

## 2.15. Limpiando main para que solo quede LICENSE, README.md y .gitignore
### Guardando todo el código en la rama “backup”
```bash
git push origin backup
```
![rama de respaldo](imgMarkdown/ramaBackup.png)

### Borrando todos los archivos preservando LICENSE, README.md y .gitignore
```bash
git rm -r --cached *
```
```bash
git reset HEAD LICENSE READNME.md .gitignore
```
![Comando para borrar](imgMarkdown/borrarRM.png)

### Commit y push al GitHub
![Comando para commitear](imgMarkdown/commitBorrar.png)
![Comando para subir al remoto](imgMarkdown/pushBorrar.png)

## 2.16. Eliminando archivos duplicados en otra rama
![archivos duplicados](imgMarkdown/eliminarDuplicados.png)
### Confirmando la eliminacion de los archivos y realizando su commit
```bash
git add -u
```
![Comando para eliminar](imgMarkdown/confirmaEliminacion.png)
![Comando para actualizar](imgMarkdown/actualizandoBorrado.png)

## 2.17. Conflicto
![rama de conflicto](imgMarkdown/ramaConflicto.png)
![rama de subir conflicto](imgMarkdown/subirConflicto.png)
![carpetas para conflicto](imgMarkdown/ramasConflicto.png)
### Creando archivos para generar conflicto
```bash
git add "archivo"
```
```bash
git commit -m "nombre para commit"
```
![commit y archivos de conflicto](imgMarkdown/commitYarchivosConclicto.png)
### Se visualiza el conflicto
![se ve el conflicto](imgMarkdown/registroConflicto.png)
![se ve el conflicto](imgMarkdown/registroConflicto2.png)
### Solucion de conflicto
![solucion de conflicto](imgMarkdown/solucionConflicto.png)
### Eliminando rama de prueba para conflicto
![Eliminando rama conflicto](imgMarkdown/eliminarRamaConflicto.png)

## 2.17. Versiones actuales
![versiones](imgMarkdown/versionesSubidas.png)

# 3. Capturas de Pantallas
## 3.1. Pagina Inicio
![Inicio](imgMarkdown/paginaInicio.png)

## 3.2. Pagina Producto
![Productos](imgMarkdown/paginaProductos.png)

## 3.3. Pagina Nosotros
![Nosotros](imgMarkdown/paginaNosotros.png)

## 3.4. Pagina Contacto
![Contacto](imgMarkdown/paginaContacto.png)