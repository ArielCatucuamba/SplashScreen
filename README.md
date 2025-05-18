# 📸 Aplicación de Galería de Fotos usando Ionic

## Guía para Cambiar el Ícono y el Splash Screen en Ionic/Capacitor
## 1. Preparar las imágenes 🙂‍↔️🙂‍↕️
   Ícono ℹ️

      -Crea una imagen cuadrada de 1024x1024 px en formato PNG.
      -Fondo transparente recomendado.
      -Nómbrala como icon.png.
   Splash Screen ❗❗❗

      -Crea una imagen de 2732x2732 px en formato PNG.
      -Fondo sólido recomendado.
      -Nómbrala como splash.png.
   
## 2. Colocar las imágenes en el proyecto 🖼️🖼️🖼️🖼️
   Copia icon.png y splash.png en la carpeta:

     assets/
   La ruta debe ser:

        assets/icon.png
        assets/splash.png
   
## 3. Generar los recursos para las plataformas
   Abre una terminal en la raíz del proyecto y ejecuta:

    npx @capacitor/assets generate
   

## 4. Sincronizar los recursos con las plataformas
  Ejecuta en la terminal:
  
      npx cap sync


  
## 5. Verificar la configuración del Splash Screen
  Asegúrate de que en tu archivo capacitor.config.ts exista la configuración para el plugin SplashScreen. 
  Ejemplo:
  ```

  plugins: {
  SplashScreen: {
    launchShowDuration: 3000,
    launchAutoHide: true,
    // ...otros parámetros opcionales
  }
}
  ```

## 6. Instalar y ejecutar la app
  Desinstala la app anterior del emulador/dispositivo para evitar caché.
  Ejecuta la app de nuevo desde Android Studio o con:
  ```
  npx cap open android
```
  Luego ejecutarla desde Android Studio verifica que todo este sincronizado y que se hayan echo los cambios correspondientes.
  


---

## 🚀 Funcionalidades (separadas por branches)

- Activación de la cámara del dispositivo  
- Captura de imágenes y almacenamiento local  
- Visualización de imágenes capturadas a modo de galería  
- Carga manual de imágenes mediante botón  
- Visualización del nombre del archivo debajo de cada imagen  
- Opción de captura de imagen con calidad al 50%  
- Visualización de imágenes en un nuevo tab (Tab 3)  

---

## 🖼️ Icono y Splash Screen

| Imagen 1 | Imagen 2 |
|----------|----------|
| ![img1](![image](https://github.com/user-attachments/assets/8853126f-ac2d-4e53-a803-9d25160c9477)
) | ![img2](![image](https://github.com/user-attachments/assets/2449b4e3-d1fe-45cf-a8e8-0bed22b8c214)
) |


---

## 🛠️ Tecnologías Utilizadas

- Node.js  
- Visual Studio Code  
- Interfaz de comandos  

---

## 🌱 Branch Principal

La rama `main` contiene la implementación base sin los cambios.  
Cada funcionalidad extra fue implementada en su respectiva rama.

---

## 🖼️ Galería de Capturas

| ![Imagen 1](https://github.com/user-attachments/assets/1fda43be-2040-4def-b2ca-b55cb5c040ee) | ![Imagen 2](https://github.com/user-attachments/assets/959de9bd-7dd8-4da2-9dfc-73b15cf6a256) |
|:--:|:--:|
| ![Imagen 3](https://github.com/user-attachments/assets/95e3faca-14ff-47d2-96bc-bb58f1b1a5c2) | ![Imagen 4](https://github.com/user-attachments/assets/84699e27-8a25-4ad4-ac53-8ad3c711ef43) |



