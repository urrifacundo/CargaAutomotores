# Carga HERMES Automotores

Página para clasificar las denuncias del crudo de Cassandra (Sustraído / Inmediato / Hallado) y descargar el Excel en formato HERMES.

El crudo se procesa en la computadora de cada operador: no se sube a ningún servidor, y este repositorio no guarda datos.

## Cómo publicarla (una sola vez)

1. En github.com: **New repository**. Nombre, por ejemplo `carga-hermes`. Visibilidad **Public** (GitHub Pages gratis lo necesita; solo se publica el código de la página, nunca los datos).
2. **Add file → Upload files** → subir `index.html` (y este README) → **Commit changes**.
3. **Settings → Pages** → en *Build and deployment*: Source **Deploy from a branch**, Branch **main** y carpeta **/ (root)** → **Save**.
4. En 1–2 minutos queda en `https://TU-USUARIO.github.io/carga-hermes/`. Ese link es el que se pasa a los operadores.

Para actualizarla: subir el `index.html` nuevo encima del anterior (Add file → Upload files) y hacer commit.

## Uso diario

1. Abrir el link, escribir el nombre del operador y elegir la **Parte** (Mitad 1 o Mitad 2 si son dos).
2. Cargar o arrastrar el crudo `.xlsx` de Cassandra.
3. Pestaña **Autos**: 1 Sustraído · 2 Inmediato · 3 Hallado · 0 No corresponde · Enter confirma y pasa a la siguiente. Corregir patente, marca, modelo, chasis, motor y coordenadas si hace falta.
4. Revisar **A revisar** (casos dudosos).
5. Cada operador: **Guardar avance** (.json). Uno junta los dos con **Unir avances** y toca **Descargar HERMES**.

El avance queda guardado en el navegador de cada operador: si se cierra la página, se vuelve a cargar el mismo crudo y sigue donde estaba.
