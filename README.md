<div align="center">

# ArtimaDev Studio &bull; Ingeniería Android Nativa de Precisión

[![Website](https://img.shields.io/badge/Web-artimadev.com-3b82f6?style=for-the-badge&logo=google-chrome&logoColor=white)](https://artimadev.com)
[![Deployed on Cloudflare Pages](https://img.shields.io/badge/Cloudflare_Pages-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)](https://artimadev.com)
[![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com)
[![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Jetpack Compose](https://img.shields.io/badge/Jetpack_Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white)](https://developer.android.com/jetpack/compose)
[![Location](https://img.shields.io/badge/Sede-Barcelona%2C_Espa%C3%B1a-06b6d4?style=for-the-badge&logo=google-maps&logoColor=white)](#)
[![Ko-fi](https://img.shields.io/badge/Apoyar-Ko--fi-FF5E5B?style=for-the-badge&logo=kofi&logoColor=white)](https://ko-fi.com/artimadev)

<p align="center">
  Repositorio oficial del portal corporativo, catálogo de fichas técnicas, buscador interactivo de códigos DTC y centro legal multi-app para Google Play Console de <b>ArtimaDev Studio</b> (Estudio independiente de ingeniería Android con sede en <b>Barcelona, España</b>).
</p>

</div>

---

## 📌 Visión General y Pilares de Ingeniería

**ArtimaDev Studio** es un estudio independiente especializado en el diseño y desarrollo de aplicaciones nativas para el ecosistema Android bajo cuatro pilares innegociables:

1. **Rendimiento 100% Nativo:** Desarrollo íntegro en **Kotlin** con **Jetpack Compose**, Material 3, Coroutines, Flow y widgets modernos con **Jetpack Glance**.
2. **Arquitectura Offline-First:** Persistencia y procesamiento local en el dispositivo mediante **Room SQLite** y **DataStore**, sin obligar al usuario a registrar cuentas en servidores externos.
3. **Privacidad por Diseño (0 Trackers):** Sin SDKs publicitarios intrusivos, sin venta de datos a terceros y con cumplimiento estricto del RGPD / GDPR europeo y las políticas de Seguridad de Datos de Google Play Console.
4. **Eficiencia Energética Real:** Tareas diferidas con **Android WorkManager** y escuchas pasivas del sistema sin *WakeLocks* parásitos, respetando el modo *Doze* de Android.

---

## 🚀 Suite de 6 Aplicaciones Android (Catálogo Oficial)

| # | Aplicación | Package ID | Categoría | Acento | Estado | Tecnologías y Protocolos Clave |
| :-: | :--- | :--- | :--- | :--- | :--- | :--- |
| **1** | **[Motorpedia OBD2 Pro](motorpedia.html)** | `com.artimadev.motorpedia` | Automoción / Diagnóstico ECU | Cyan / Azul | **Google Play** | Bluetooth BLE/Classic, ELM327, SAE J1979, Modo Drag, +50.000 DTCs Offline |
| **2** | **[CineMatch](cinematch.html)** | `com.artimadev.cinematch` | Streaming & Descubrimiento | Rojo / Rosa | **Google Play** | API Oficial TMDB, 12 Plataformas, Modo Duelo 1vs1, Candado Parental PIN, 9 Idiomas |
| **3** | **[Baterix](baterix.html)** | `com.artimadev.baterix` | Telemetría de Batería & Salud | Esmeralda | **Google Play / Beta** | `BatteryManager` API (mA, mV, °C), Alerta 80% Carga, Widgets Jetpack Glance |
| **4** | **[Pluvio](pluvio.html)** | `com.artimadev.pluvio` | Meteorología / Nowcasting 60m | Azul Cielo | **Google Play / Beta** | Previsión minuto a minuto (60 min), Open-Meteo API, WorkManager, Glance Widget |
| **5** | **[QuickMute](quickmute.html)** | `com.artimadev.quickmute` | Control Instantáneo de Audio | Púrpura | **Beta Abierta** | `AudioManager` API, Quick Settings Tile, Alarm Safe (`STREAM_ALARM`), Auto-Restore Timer |
| **6** | **[Kippo](kippo.html)** | `com.artimadev.kippo` | Tickets, Garantías y Vencimientos | Ámbar / Naranja | **Nuevo / Beta** | Escáner de tickets térmicos, Alertas de Garantía (3 años) y Devolución, Room DB Offline |

---

## 🛠️ Especificaciones Técnicas por Aplicación

### 1. ⚡ [Motorpedia OBD2 Pro](motorpedia.html) (`com.artimadev.motorpedia`)
Suite de diagnóstico automotriz multimarca vía adaptadores ELM327 (Bluetooth Clásico y BLE 4.0/5.0):
* Lectura y borrado de códigos de fallo de motor y transmisión (**Check Engine / MIL Off**).
* Cuadro de instrumentos en tiempo real (RPM, refrigerante, presión de turbo Boost/MAP, caudalímetro MAF, sondas lambda).
* **Modo Drag** para cronometrar aceleración (0-100 km/h y 400m) y test de salud de batería 12V / alternador (14.4V).
* Incluye en la web un **Buscador Interactivo de +50.000 códigos DTC** en español y guía de adaptadores ELM327 por semáforo.

### 2. 🎬 [CineMatch](cinematch.html) (`com.artimadev.cinematch`)
Recomendador inteligente y 100% legal de películas y series:
* Filtrado cruzado simultáneo entre **12 plataformas de streaming** (Netflix, Prime Video, Disney+, Max, SkyShowtime, Apple TV+, Movistar Plus+, Filmin, Crunchyroll, Rakuten TV, Atresplayer y Pluto/Mitele).
* **Modo Duelo 1 vs 1 en pareja:** Dos personas votan en secreto pasando un único teléfono Android en el sofá hasta hacer *Match*.
* **Candado Parental certificado por TMDB:** Bloqueo por PIN local de 4 dígitos basado en las calificaciones oficiales por edad (+7, +12, +16, +18).

### 3. 🔋 [Baterix](baterix.html) (`com.artimadev.baterix`)
Monitor de telemetría energética en tiempo real y protección contra la degradación química de celdas de litio:
* Lectura en directo de corriente de carga/descarga en miliamperios (`mA`), voltaje (`mV`) y temperatura (`°C`) mediante `BatteryManager`.
* **Alarma configurable al 80% de carga** (regla 20-80%) para evitar el estrés de alta tensión en el cátodo y triplicar los ciclos de vida útil.
* Widgets nativos en pantalla de inicio con **Jetpack Glance** y arquitectura pasiva sin *WakeLocks* parásitos.

### 4. 🌧️ [Pluvio](pluvio.html) (`com.artimadev.pluvio`)
Radar de lluvia hiperlocal a muy corto plazo (*Nowcasting* de 60 minutos):
* Previsión minuto a minuto sobre tu ubicación exacta impulsada por **Open-Meteo**.
* Avisos preventivos automáticos en segundo plano programados con **Android WorkManager**.
* Widget limpio y directo en pantalla de inicio construido con **Jetpack Glance**.

### 5. 🔇 [QuickMute](quickmute.html) (`com.artimadev.quickmute`)
Control instantáneo de canales de sonido en Android:
* Silenciamiento rápido desde **Quick Settings Tile** en la barra de notificaciones o widgets de escritorio.
* Aislamiento inteligente: silencia multimedia (`STREAM_MUSIC`) y notificaciones manteniendo intactas las alarmas del despertador (`STREAM_ALARM`) y llamadas prioritarias.
* Temporizador de restauración automática de volumen para reuniones, clases o cine.

### 6. 🧾 [Kippo](kippo.html) (`com.artimadev.kippo`)
Gestor privado de tickets de compra, facturas, garantías y vencimientos:
* Digitalización rápida de tickets en papel térmico antes de que la tinta se borre con el paso del tiempo.
* Alertas automáticas programadas con **WorkManager** antes de que venza el plazo de devolución (15/30/60 días) o la garantía legal (2/3 años).
* Bóveda documental 100% privada y local en el dispositivo (**Room SQLite**) sin subir facturas ni hábitos de consumo a servidores en la nube.

---

## 📂 Estructura de Archivos del Repositorio (10 Archivos)

```text
artimadev-web/
├── index.html          # Portada corporativa, propuesta de valor, catálogo Bento de las 6 apps y stack
├── privacidad.html     # Centro legal unificado con pestañas interactivas (General + las 6 aplicaciones)
├── soporte.html        # Centro de ayuda, guía de Beta Testers en Google Play (mailto por app) y Ko-fi
├── motorpedia.html     # Ficha Motorpedia OBD2 Pro, buscador web de +50.000 DTCs y guía ELM327
├── cinematch.html      # Ficha CineMatch, Modo Duelo 1vs1, 12 plataformas y Candado Parental TMDB
├── baterix.html        # Ficha Baterix, telemetría mA/mV/°C, alarma al 80% y widgets Jetpack Glance
├── pluvio.html         # Ficha Pluvio, radar de lluvia a 60 minutos (Nowcasting) y WorkManager
├── quickmute.html      # Ficha QuickMute, Quick Settings Tile, protección de alarmas y temporizador
├── kippo.html          # Ficha Kippo, gestor privado de tickets térmicos, facturas y alertas de garantía
└── README.md           # Documentación técnica y arquitectura del portal corporativo
```

---

## ☁️ Sistema de Diseño y Despliegue en Cloudflare Pages

* **Estética UI/UX:** Inspirada en portales de ingeniería de software de alto nivel (*Linear*, *Vercel*, *Raycast*), con fondo oscuro profundo (`#08080a`), textura *dot-grid*, tarjetas Bento Grid con bordes translúcidos (`border-white/10`) y halos ambientales por aplicación.
* **Stack Frontend:** HTML5 semántico, **Tailwind CSS** (vía CDN), tipografías `Plus Jakarta Sans` y `JetBrains Mono`, e iconografía vectorial SVG personalizada sin dependencias pesadas.
* **Despliegue Continuo (CI/CD):** Alojado en **Cloudflare Pages** con distribución en red Edge global, compresión Brotli/Gzip, HTTP/3 y certificados SSL automáticos.
  * *Build command:* Ninguno requerido (sitio estático puro de carga instantánea).
  * *Build output directory:* `/` (raíz del repositorio).

---

## 🤝 Contacto, Soporte y Comunidad

* **Estudio:** ArtimaDev Studio — Sede en **Barcelona, España (UE)**
* **Contacto y Soporte Técnico Directo:** [artimadev@gmail.com](mailto:artimadev@gmail.com)
* **Programa Oficial de Beta Testers:** [soporte.html#testers](soporte.html#testers)
* **Centro Legal y Privacidad (Play Console):** [privacidad.html](privacidad.html)
* **Apoyar el Desarrollo Independiente:** [ko-fi.com/artimadev](https://ko-fi.com/artimadev)

---

<div align="center">
  <p>&copy; 2026 ArtimaDev Studio (Barcelona, España). Todos los derechos reservados.</p>
</div>
