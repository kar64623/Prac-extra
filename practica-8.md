## Cuestionario 

### ¿Cómo se inicializa un repositorio en Git? 
Para empezar, debemos de estar dentro de la carpeta donde queramos inicializar el repositorio, una vez dentro hacemos uso del siguiente comando: 

```bash 
git init
```
### ¿Cómo creas un repositorio en Github?
Para empezar un repositorio en Github tenemos que irnos a la interfaz web de [Github](https://github.com), donde iniciaremos sesión con una cuenta que ya tengamos creada, del lado derecho, dentro de la cabezera de la página, veremos una cruz donde daremos click y posteriormente seleccionaremos _New repository_, nos cargará una interfaz donde podremos darle las caracterísitcas a nuestro nuevo repositorio

### ¿Cómo vinculas un repositorio local de Git con uno remoto en Github?
Con el comando _git remote add origin_ y de argumento pondremos el link de nuestro repositorio de github.

```bash 
git remote add origin https://github.com/kar64623/Amerike
```

### ¿Cúal es el flujo de trabajo en Git y Github? 
Git funciona como un **sistema** de control de versionado. Github es una **plataforma** que nos permite alamcenar ese control de versiones y hacerlo público, su flujo de trabajo funciona a partir de ramas y commits. La rama **main** funciona como una rama principal de la cual emergen otras que al final se fusionan con la **main**

```bash 
git add 
git commit -m "Mensaje del commit"
git push origin main 
```

### ¿Para qué sirve el archivo .gitignore?
Sirve para establecer incluir todo lo que no queramos subir a nuestro repositorio.

```bash 
touch .gitignore 
echo "*.exe" >> .gitignore
```

### ¿Cuál es el propósito de una rama?
El propósito de una rama es el de separar el flujo de trabajo de la rama **main**. Para crear una rama se usa el siguiente comando: 

```bash 
git branch rama1
```

### ¿Qué es una fusión?
Es la manera en cómo se unen dos o más ramas 

```bash 
git merge rama1
```

### Los tipos de fusión que existen 
- Fast-Forward: La fusión se logró de manera automática. 
- Manual-Merge: Es necesario hacer la fusión de manera manual para resolver problemas. 

### ¿Cómo puedes ver el historial de tu repositorio?
El historial se puede visitar de la siguiente manera: 

```bash 
git log 
```
Esto despliega todo el historial incluyendo los detalles de los cambios realizados, cabe destacar que se pueden agregar filtros de búsqueda dentro de las flags del comando. 

### ¿Cuál es el propósito de una etiqueta? 
Nos permite _versionar_ nuestro código

```bash 
git tag v1.0.0.
```
