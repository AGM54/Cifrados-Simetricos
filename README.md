# Proyecto de Cifrados Simétricos

## 📌 Descripción
Este laboratorio demuestra la implementación de **cifrados simétricos** usando **AES-CBC y AES-ECB**, aplicados a imágenes y comunicación en red. Se realizan pruebas de seguridad para analizar cómo se comportan estos cifrados y cómo pueden capturarse con Wireshark.

---

## 📂 Archivos en el Proyecto

### 🔹 Cifrado de Imágenes:
- `tux.ppm` → Imagen original en formato PPM.
- `tux_ecb.ppm` → Imagen cifrada con **AES-ECB**.
- `tux_cbc.ppm` → Imagen cifrada con **AES-CBC**.
- `tux_ecb.png` y `tux_cbc.png` → Versiones en PNG de las imágenes cifradas.
- `gato.jpg` → Imagen alternativa de prueba.
- `gato_ecb.png` y `gato_cbc.png` → Imagen alternativa cifrada con AES-ECB y AES-CBC.
- `imagen_nueva.ppm` → Imagen adicional de prueba.

### 🔹 Código para Cifrado de Imágenes:
- `cifrados.ipynb` → Jupyter Notebook con la implementación del cifrado de imágenes en **AES-ECB y AES-CBC**.


### 🔹 Comunicación Segura con Sockets y Wireshark:
- `servidor.py` → Servidor TCP que recibe mensajes cifrados con **AES-CBC**.
- `cliente.py` → Cliente TCP que envía mensajes cifrados al servidor.
- `archivos_prueba/` → Carpeta con archivos de prueba para cifrado y descifrado.

---

## 🚀 Ejecución

### 🔹 1. Cifrado y Descifrado de Imágenes
1. **Ejecutar el código en `cifrados.ipynb`** dentro de Jupyter Notebook.
2. **Comparar las imágenes originales vs. cifradas** (`tux_ecb.png`, `tux_cbc.png`).

### 🔹 2. Comunicación Cifrada con Sockets (Wireshark)
1. **Ejecutar el servidor** en una computadora o terminal:
   ```bash
   python servidor.py
   ```
2. **Ejecutar el cliente** en otra computadora o en otra terminal:
   ```bash
   python cliente.py
   ```
3. **Enviar mensajes desde el cliente** y ver cómo el servidor los descifra.
4. **Capturar el tráfico con Wireshark** y analizar los datos cifrados.
5. **Aplicar el filtro en Wireshark** para ver solo el tráfico relevante:
   ```
   tcp.port == 4444
   ```

---

