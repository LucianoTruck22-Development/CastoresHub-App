<div align="center">

  <img src="https://raw.githubusercontent.com/LucianoTruck22-Development/CastoresHub-App/main/assets/banner.png" alt="CastoresHub Banner" width="100%" onerror="this.style.display='none'"/>

  # 🚛 CastoresHub App
  ### El Cliente Oficial de Telemetría y Gestión Logística para Castores Trucking VTC
  
  **Euro Truck Simulator 2** &bull; **American Truck Simulator**

  <p align="center">
    <a href="https://github.com/LucianoTruck22-Development/CastoresHub-App/releases/latest">
      <img src="https://img.shields.io/github/v/release/LucianoTruck22-Development/CastoresHub-App?style=for-the-badge&color=0070f3&label=Descargar%20Última%20Versión" alt="Última Versión"/>
    </a>
    <a href="https://hub.castorestrucking.mx/">
      <img src="https://img.shields.io/badge/Web%20Hub-castorestrucking.mx-000000?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Sitio Web"/>
    </a>
    <a href="https://discord.gg/kXZX89erVc">
      <img src="https://img.shields.io/badge/Discord-Comunidad%20VTC-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord"/>
    </a>
  </p>

  <p align="center">
    <img src="https://img.shields.io/badge/Plataforma-Windows%2010%20%7C%2011%20(64--bit)-blue?style=flat-square&logo=windows" alt="Plataforma Windows"/>
    <img src="https://img.shields.io/badge/Motor-Tauri%20v2%20%2B%20Rust-orange?style=flat-square&logo=tauri" alt="Tauri v2"/>
    <img src="https://img.shields.io/badge/Juegos-ETS2%20%7C%20ATS-red?style=flat-square&logo=steam" alt="ETS2 & ATS"/>
    <img src="https://img.shields.io/badge/Estado-Producción%20Activa-emerald?style=flat-square" alt="Estado Activo"/>
  </p>

</div>

---

## 📌 ¿Qué es CastoresHub App?

**CastoresHub App** es la aplicación de escritorio oficial diseñada exclusivamente para los conductores de **Castores Trucking VTC**. 

Construida con tecnología de alto rendimiento (**Tauri v2 + Rust**), se conecta de forma nativa a la simulación de **Euro Truck Simulator 2** y **American Truck Simulator** mediante el SDK oficial de telemetría de SCS Software. Rastrea en tiempo real cada kilómetro conducido, flete completado, consumo de diésel, salud mecánica y progreso en la empresa sin impactar el rendimiento de tus juegos.

---

## ✨ Características Principales

- 📦 **Registro y Hoja de Ruta Automática:** Detección en vivo de contratos, cargas, pesos, orígenes, destinos y cálculo de navegación GPS.
- 💾 **Persistencia y Modo Offline (SQLite):** Guarda tus viajes localmente incluso si juegas sin conexión a internet; tus entregas se sincronizan de forma segura tan pronto vuelvas a estar online.
- 🌐 **Soporte Multijugador Completo:** Compatible de forma nativa con **TruckersMP**, **HaulMP**, **SCS Convoy** y modo **Singleplayer**.
- 🎮 **Discord Rich Presence (RPC):** Muestra en tu perfil de Discord qué estás conduciendo, la carga transportada, origen, destino y distancia restante sin desconexiones.
- 🚚 **Diagnóstico y "Mi Unidad":** Monitoreo detallado del estado del camión y remolque (daño por componentes, odómetro acumulado, autonomía y combustible restante).
- 📋 **Despachador Integrado:** Generación y asignación de rutas personalizadas sincronizadas directamente con la economía de la VTC.
- 🔄 **Actualizador Automático Integrado:** Notificaciones e instalación en un clic de las últimas versiones y mejoras de estabilidad.

---

## 📥 Descarga e Instalación

### Requisitos del Sistema
- **Sistema Operativo:** Windows 10 / 11 (64-bit).
- **Juegos Soportados:** Euro Truck Simulator 2 y/o American Truck Simulator (instalaciones oficiales de Steam).
- **Componentes Requeridos:** [Visual C++ Redistributable (x64)](https://aka.ms/vs/17/release/vc_redist.x64.exe) y WebView2 Runtime (incluido en Windows 10/11).

### Pasos de Instalación:
1. Ve a la sección de [**Releases (Lanzamientos)**](https://github.com/LucianoTruck22-Development/CastoresHub-App/releases/latest).
2. Descarga el instalador ejecutable más reciente: `CastoresHub_x.x.x_x64-setup.exe`.
3. Ejecuta el instalador y sigue los pasos del asistente.
4. Abre **CastoresHub App**, inicia sesión con tus credenciales de la VTC o vincula tu cuenta de Discord.
5. Inicia tu simulador (ETS2 o ATS) y ¡a rodar! El rastreador detectará tu camión automáticamente.

---

## ❓ Preguntas Frecuentes & Solución de Problemas

<details>
<summary><b>1. ¿Windows SmartScreen muestra una advertencia al abrir el instalador?</b></summary>
<br>
Al tratarse de una aplicación interna de comunidad firmada recientemente, haz clic en <i>"Más información"</i> y luego en <i>"Ejecutar de todas formas"</i>. El ejecutable está libre de amenazas y auditado para la empresa.
</details>

<details>
<summary><b>2. La app no detecta el juego al entrar al camión</b></summary>
<br>
Asegúrate de que el plugin de telemetría (<code>scs-telemetry.dll</code>) esté instalado en la carpeta de plugins de tu juego (<code>bin/win_x64/plugins/</code>). Puedes reinstalar el plugin o verificar las rutas desde la pestaña de <b>Configuración</b> dentro de la aplicación.
</details>

<details>
<summary><b>3. ¿Funciona en servidores de TruckersMP?</b></summary>
<br>
Sí. CastoresHub detecta automáticamente cuando estás conectado a TruckersMP y muestra el nombre del servidor y el estado de los compañeros de la empresa en línea.
</details>

---

## 🔒 Privacidad y Seguridad

- **Sin Telemetría Invasiva:** CastoresHub únicamente lee datos de simulación provistos por el SDK oficial de SCS Software mientras el juego está abierto.
- **Credenciales Protegidas:** Los tokens de autenticación se almacenan localmente cifrados mediante el almacén seguro de Tauri (Stronghold).
- **Código Cerrado:** Este repositorio sirve exclusivamente para distribución de versiones, anuncios de parches, reporte de incidencias y documentación para los conductores.

---

## 🌐 Enlaces Oficiales & Soporte

- 🌍 **Portal Web Oficial:** [https://hub.castorestrucking.mx/](https://hub.castorestrucking.mx/)
- 💬 **Discord Oficial de Castores Trucking:** [Unirse a la comunidad](https://discord.gg/kXZX89erVc)
- 🎫 **Mesa de Ayuda / Soporte:** Si experimentas problemas con tus entregas o la aplicación, abre un ticket en nuestro Discord o portal de soporte.

---

<div align="center">
  <sub>Desarrollado con ❤️ por <b>LT Developer</b> para <b>Castores Trucking VTC</b>.<br/>
  Euro Truck Simulator 2 y American Truck Simulator son marcas registradas de SCS Software. Esta aplicación no está afiliada ni respaldada por SCS Software.</sub>
</div>

