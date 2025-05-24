# File Metadata Microservice

This is the boilerplate for the File Metadata Microservice project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/file-metadata-microservice

Este proyecto es un microservicio para subir archivos y obtener la metadata del archivo subido: nombre, tipo y tamaño en bytes.

---

## Tecnologías usadas

- Node.js
- Express
- Multer (para manejo de subida de archivos)
- Cors
- dotenv

---

## Instalación

1. Clona este repositorio:

```bash
git clone https://github.com/TheMasterShoot/project-filemetadata-microservice.git
```

2. Instala las dependencias:

```bash
npm install
```

3. (Opcional) Crea un archivo `.env` para configurar el puerto si lo deseas:

```
PORT=3000
```

---

## Uso

1. Ejecuta el servidor:

```bash
npm start
```

2. Abre tu navegador y ve a:

```
http://localhost:3000/
```

3. Usa el formulario para subir un archivo.

4. El servidor responderá con un JSON con la metadata del archivo, por ejemplo:

```json
{
  "name": "archivo.png",
  "type": "image/png",
  "size": 24567
}
```

---

## Estructura del proyecto

```
/
├── public/         # Archivos estáticos
├── views/          # Página HTML con el formulario de subida
├── .env            # Variables de entorno (opcional)
├── index.js        # Servidor Express
├── package.json
└── README.md
```

---

## Nota

El campo del formulario para subir el archivo debe tener el atributo `name="upfile"` para que el backend lo procese correctamente.

---

## Pruebas

1. Debes proporcionar tu propio proyecto, no el URL de ejemplo.
2. Puedes enviar un formulario que incluya una subida de archivo.
3. El campo de entrada del archivo en el formulario debe tener el atributo `name="upfile"`.
4. Cuando envías un archivo, recibes un JSON con el nombre, tipo y tamaño del archivo en bytes.

---


