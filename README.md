# 🌸 Lizzendy Lashes · Cejas y Pestañas

## 📖 Descripción del Proyecto

Este es el sitio web oficial para **Lizzendy Lashes**, un estudio especializado en extensiones de pestañas y diseño de cejas. El sitio está diseñado para transmitir una imagen elegante, femenina y profesional, destacando la calidad artesanal del trabajo (hecho a mano, pestaña por pestaña).

El sitio web está construido como una página de una sola vista (Single Page Application estática) que presenta de manera clara los servicios, precios y el proceso de trabajo, con un fuerte enfoque en el diseño visual y la experiencia de usuario.

## 🎯 Objetivos Comerciales del Sitio

El sitio web ha sido construido para cumplir los siguientes objetivos:

1. **Generar confianza y credibilidad:** El diseño elegante y las fotos de alta calidad (incluyendo un video de demostración) muestran a las clientas el nivel de profesionalismo y cuidado que pueden esperar.
2. **Comunicar claramente la oferta de servicios:** La estructura clara de la página permite que las visitantes encuentren de inmediato qué servicios ofreces y sus precios.
3. **Facilitar la acción (Reservar cita):** Los llamados a la acción (CTA) estratégicamente ubicados ("Reservar cita", "Escríbenos por Instagram") dirigen a las clientas hacia el siguiente paso natural: contactarte.
4. **Posicionar la marca:** El uso de colores, tipografías y elementos visuales únicos (como los divisores de pestañas) refuerzan la identidad de **Lizzendy Lashes** como un estudio premium y de alta calidad.

## 🌐 Despliegue en AWS (S3 + CloudFront)

El sitio web está alojado en Amazon Web Services (AWS) para garantizar que esté siempre disponible y se cargue rápidamente para tus clientas. Para actualizar el sitio web en producción, el proceso es el siguiente:

1. **Subir Archivos:** Una vez que hayas realizado los cambios en los archivos locales, cárgalos al bucket de S3 (el origen de tu sitio).
2. **Invalidar Caché (Importante):** Después de subir los archivos, es necesario **invalidar la caché** en CloudFront. Esto le indica a la red de distribución que debe buscar los archivos más recientes. Puedes hacerlo desde la consola de AWS (CloudFront → Distribución → Invalidations → Create Invalidation → `/*`) o configurar una política automática.
