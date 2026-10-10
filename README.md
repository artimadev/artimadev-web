<div align="center">

# ArtimaDev &bull; Android Engineering Studio

[![Website](https://img.shields.io/badge/Web-artimadev.com-3b82f6?style=for-the-badge&logo=google-chrome&logoColor=white)](https://artimadev.com)
[![Deployed on Cloudflare Pages](https://img.shields.io/badge/Cloudflare_Pages-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)](https://artimadev.com)
[![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com)
[![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Location](https://img.shields.io/badge/Sede-Barcelona%2C_Espa%C3%B1a-zinc?style=for-the-badge&logo=google-maps&logoColor=red)](#)

<p align="center">
  Repositorio oficial del portal corporativo y centro de documentación legal para la suite de aplicaciones nativas Android de <b>ArtimaDev Studio</b>.
</p>

</div>

---

## 📌 Visión General

**ArtimaDev** es un estudio de desarrollo de software enfocado en ingeniería Android nativa de alto rendimiento. Desarrollamos soluciones optimizadas bajo principios de arquitectura limpia, privacidad local (*offline-first*) y cero consumo residual en segundo plano. 

Este sitio web centraliza:
* La presentación técnica y enlaces directos de descarga de nuestra suite de aplicaciones.
* La infraestructura legal y de políticas de privacidad requerida para el cumplimiento normativo de **Google Play Console**.
* El canal de captación y coordinación de testers para fases de prueba cerradas.

---

## 🚀 Suite de Aplicaciones

| Aplicación | Categoría | Estado | Stack / Protocolo |
| :--- | :--- | :--- | :--- |
| **Motorpedia Pro** | Diagnosis Automotriz OBD2 / UDS | Producción | Bluetooth BLE/Classic, ISO 14229, DTC Engine |
| **CineMatch** | Streaming & Recomendación | Producción | TMDb API, Multiplataforma, Algoritmo 1vs1 |
| **Baterix** | Telemetría de Energía & Batería | Beta Cerrada | BatteryManager API, Umbral 80%, No-WakeLock |
| **QuickMute** | Control de Audio & Productividad | Beta Cerrada | AudioManager, Quick Settings Tile, Sound Profiles |

### 🛠️ Detalles de los Proyectos

* **[Motorpedia Pro](motorpedia.html):** Suite de diagnosis vehicular profesional multimarca. Comunicación bidireccional mediante adaptadores ELM327, monitorización de telemetría de motor en tiempo real, análisis de sondas lambda, soporte de tramas UDS y biblioteca local de códigos de avería (DTC).
* **[CineMatch](cinematch.html):** Recomendador ágil de catálogo de cine y series integrado con las 12 principales plataformas de streaming. Incorpora modo duelo en terminal compartido para resolver la indecisión al elegir contenido y candado parental verificado.
* **[Baterix](baterix.html):** Monitorización precisa de ciclos y amperaje (mA) en tiempo real. Diseñado para mitigar la degradación química en terminales con carga rápida mediante alertas preventivas al alcanzar el 80% de carga.
* **[QuickMute](quickmute.html):** Herramienta táctil para la gestión inmediata de canales de sonido. Permite silenciar la salida multimedia al instante sin alterar las alarmas críticas del sistema, integrable en los ajustes rápidos de Android.

---

## 📂 Arquitectura del Repositorio

El sitio web está implementado en **HTML5 semántico** y estilizado mediante **Tailwind CSS**, priorizando tiempos de carga casi instantáneos y compatibilidad móvil estricta:

```text
artimadev-web/
├── index.html          # Portada principal, catálogo de 4 apps y stack técnico
├── motorpedia.html     # Ficha técnica de Motorpedia Pro y buscador de fallos DTC
├── cinematch.html      # Ficha técnica y características de CineMatch
├── baterix.html        # Especificaciones del monitor de salud de batería
├── quickmute.html      # Documentación de la utilidad de perfiles de sonido
├── privacidad.html     # Política de privacidad global requerida por Google Play
└── README.md           # Documentación técnica del repositorio
