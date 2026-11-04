<div align="center">

# ArtimaDev &bull; Android Engineering Studio

[![Website](https://img.shields.io/badge/Web-artimadev.com-3b82f6?style=for-the-badge&logo=google-chrome&logoColor=white)](https://artimadev.com)
[![Deployed on Cloudflare Pages](https://img.shields.io/badge/Cloudflare_Pages-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)](https://artimadev.com)
[![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com)
[![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Location](https://img.shields.io/badge/Sede-Barcelona%2C_Espa%C3%B1a-06b6d4?style=for-the-badge&logo=google-maps&logoColor=white)](#)
[![Ko-fi](https://img.shields.io/badge/Apoyar-Ko--fi-FF5E5B?style=for-the-badge&logo=kofi&logoColor=white)](https://ko-fi.com/artimadev)

<p align="center">
  Repositorio oficial del portal corporativo, fichas técnicas y centro legal multi-app de <b>ArtimaDev Studio</b> (Estudio independiente de ingeniería Android con sede en Barcelona, España).
</p>

</div>

---

## 📌 Visión General

**ArtimaDev** es un estudio independiente enfocado en ingeniería de software nativa para Android. Diseñamos y desarrollamos soluciones optimizadas bajo principios de:

1. **Rendimiento 100% Nativo:** Desarrollo exclusivo en **Kotlin** con **Jetpack Compose**, Coroutines y Flow.
2. **Arquitectura Offline-First:** Procesamiento de datos y almacenamiento en local mediante Room SQLite y DataStore. Cero necesidad de registrar cuentas en servidores externos.
3. **Privacidad y Cero Telemetría Invasiva:** Sin rastreadores publicitarios, sin venta de datos a terceros y cumplimiento estricto con el RGPD y las directrices de Google Play Console.
4. **Eficiencia Energética:** Cero servicios en segundo plano permanentes (*Zero WakeLocks*), compatibilidad plena con el modo Doze de Android.

---

## 🚀 Suite de Aplicaciones (Catálogo Oficial)

| Aplicación | Package ID | Categoría | Estado | Tecnologías / Protocolos Clave |
| :--- | :--- | :--- | :--- | :--- |
| **[Motorpedia Pro](motorpedia.html)** | `com.artimadev.motorpedia` | Automoción / OBD2 & UDS | **Producción** (Google Play) | Bluetooth BLE/Classic, ELM327, SAE J1979, ISO 14229 UDS, +50.000 DTCs Offline |
| **[CineMatch](cinematch.html)** | `com.artimadev.cinematch` | Streaming & Entretenimiento | **Producción** (Google Play) | TMDb API, 12 Plataformas, Algoritmo Duelo 1vs1, Candado Parental TMDB, 9 Idiomas |
| **[QuickMute](quickmute.html)** | `com.artimadev.quickmute` | Audio & Productividad | **Beta Abierta** | AudioManager API, Quick Settings Tile, Widgets Glance, Auto-Restore Timer |
| **[Batterix](baterix.html)** | `com.artimadev.baterix` | Telemetría Energética | **Fase de Pruebas** | BatteryManager API, Alarma Umbral 80%, mA / mV / °C en vivo, Glance Widgets |
| **[Pluvio](pluvio.html)** | `com.artimadev.pluvio` | Meteorología / Nowcasting | **En Desarrollo** | Nowcasting a 60 min, Open-Meteo API, Android WorkManager, Glance AppWidget |

---

## 🛠️ Especificaciones de los Proyectos

### 1. ⚡ [Motorpedia OBD2 Pro](motorpedia.html)
Suite profesional de diagnosis automotriz multimarca vía adaptadores ELM327 (Bluetooth y BLE):
* Lectura y borrado de códigos de fallo de motor y transmisión (Check Engine / MIL Off).
* Cuadro de relojes personalizable con telemetría en tiempo real (RPM, temperatura de refrigerante, presión de turbo Boost/MAP, caudalímetro MAF, sondas lambda).
* Modo Drag para medición precisa de aceleración (0-100 km/h y 400m).
* Test eléctrico de batería y alternador (12V en reposo y 14.4V en carga).
* Buscador web integrado y biblioteca local con más de 50.000 códigos DTC en español.

### 2. 🎬 [CineMatch](cinematch.html)
El recomendador inteligente y legal de cine y series:
* Filtrado cruzado simultáneo entre 12 plataformas contratadas en España y Latinoamérica (Netflix, Prime Video, Disney+, Max, SkyShowtime, Movistar Plus+, Filmin, etc.).
* **Modo Duelo 1 vs 1:** Dos personas eligen qué ver en el sofá pasando un único teléfono Android por turnos hasta hacer "Match".
* **Candado Parental Oficial:** Bloqueo mediante PIN de 4 dígitos basado en las certificaciones por edad oficiales de TMDB (+7, +12, +16, +18).
* Soporte nativo para 9 idiomas y fichas completas con tráilers en alta definición.

### 3. 🔇 [QuickMute](quickmute.html)
Control táctil instantáneo de canales de sonido en Android:
* Botón integrado en la cortina de Ajustes Rápidos (*Quick Settings Tile*).
* Aislamiento de canales: silencia multimedia y juegos manteniendo las alarmas del despertador y llamadas prioritarias activas.
* Temporizador de auto-restauración para reuniones, clases o sesiones de cine.

### 4. 🔋 [Batterix](baterix.html)
Monitor avanzado de carga en tiempo real y protección contra la degradación química de celdas de litio:
* Lectura en vivo de corriente de entrada/salida en miliamperios (mA), voltaje y temperatura térmica en °C.
* Alerta sonora y vibración al alcanzar el umbral de protección del 80% de carga (regla 20-80% para triplicar los ciclos de vida útil).
* Widgets nativos construidos con Jetpack Glance para Android 12+.

### 5. 🌧️ [Pluvio](pluvio.html)
Radar meteorológico hiperlocal de precipitaciones a muy corto plazo (Nowcasting a 60 minutos):
* Gráfica de intensidad de lluvia minuto a minuto en tu posición exacta.
* Avisos preventivos en segundo plano programados con Android WorkManager.
* Widget minimalista de escritorio sin mapas pesados ni publicidad invasiva.

---

## 📂 Arquitectura de Archivos del Portal

```text
artimadev-web/
├── index.html          # Portal corporativo principal, hero y catálogo Bento Grid
├── motorpedia.html     # Ficha de Motorpedia Pro, buscador DTC web y guía de adaptadores
├── cinematch.html      # Ficha de CineMatch, Modo Duelo 1vs1 y Candado Parental
├── quickmute.html      # Ficha de QuickMute, control de canales y Quick Settings Tile
├── baterix.html        # Ficha de Batterix, telemetría mA y protección al 80%
├── pluvio.html         # Ficha de Pluvio, nowcasting de 60 minutos y widget Glance
├── soporte.html        # Centro de atención técnica, canal de Beta Testers y Ko-fi
├── privacidad.html     # Centro legal y política de privacidad interactiva multi-app
└── README.md           # Documentación técnica del repositorio
```

---

## ☁️ Infraestructura y Despliegue

* **Alojamiento:** [Cloudflare Pages](https://pages.cloudflare.com/) con CDN distribuida globalmente, compresión Brotli y certificados SSL automáticos.
* **Stack Web:** HTML5 semántico, Tailwind CSS vía CDN, tipografías *Plus Jakarta Sans* y *JetBrains Mono*, e iconografía vectorial SVG nativa.
* **Diseño:** Modo oscuro profundo (`#08080a`), textura dot-grid, tarjetas Bento Grid con microinteracciones y diseño 100% responsive.

---

## 🤝 Soporte, Comunidad y Mecenazgo

* **Soporte Técnico Directo:** [artimadev@gmail.com](mailto:artimadev@gmail.com)
* **Programa Oficial de Beta Testers:** [soporte.html#testers](soporte.html#testers)
* **Apoyo al Desarrollo Independiente:** [ko-fi.com/artimadev](https://ko-fi.com/artimadev)
* **Sede:** Barcelona, España (Unión Europea).

---

<div align="center">
  <p>&copy; 2026 ArtimaDev Studio. Todos los derechos reservados.</p>
</div>
