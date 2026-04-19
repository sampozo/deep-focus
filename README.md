# DeepFocus - Premium Deep Work Timer App

DeepFocus es una aplicación móvil de productividad basada en el método Deep Work de Cal Newport, diseñada con una estética premium y funcionalidades zero-backend.

## Funcionalidades

- **Temporizador Deep Work**: 3 bloques de trabajo de 90 min + 2 descansos
- **Estética Premium**: Gradiente 145deg, glassmorphism, sombras de profundidad
- **Haptics**: Vibración táctil en alarmas de transición
- **Wake Lock**: Pantalla siempre encendida durante sesiones
- **Audio**: Tonos de transición trabajo/descanso
- **Diseño responsive**: Safe areas para notch/pantallas modernas
- **Zero-Backend**: Sin dependencias de red para funcionar

## Stack Tecnológico

- **Frontend**: HTML5 + CSS3 + Vanilla JS
- **Build**: Vite + vite-plugin-singlefile
- **Mobile**: Capacitor 6.x (Android/iOS)
- **Haptics**: Capacitor Haptics Plugin

## Generación Local del APK

### Requisitos Previos

```bash
# Node.js 18+
node -v

# Android Studio (para Android)
# Java JDK 17+
java -version
```

### Pasos

1. **Instalar dependencias**:
```bash
npm install
```

2. **Sincronizar Capacitor**:
```bash
npm run sync
```

3. **Ejecutar en dispositivo/emulador**:
```bash
npm run open:android
```

4. **Generar APK de debug**:
```bash
npm run build:android
```

El APK se generará en: `android/app/build/outputs/apk/debug/`

## Estructura del Proyecto

```
deep-focus/
├── index.html          # App principal
├── package.json      # Dependencias npm
├── vite.config.js   # Config Vite
├── capacitor.config.json
├── README.md
└── android/       # Proyecto Android (generado por Capacitor)
```

## Credits

- **SPIng 2026** - Diseño y desarrollo
- **Fonts**: Outfit, JetBrains Mono (Google Fonts)