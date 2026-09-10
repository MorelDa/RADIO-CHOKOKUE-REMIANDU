# Radio Chokokue Remiandú 95.1 FM — PWA pura

Este proyecto es una **PWA web instalable**. No contiene APK, Capacitor, Android Studio ni código Android nativo.

## Instalación correcta

1. Publica todo el contenido en un dominio con **HTTPS**.
2. Abre la web desde Chrome o Samsung Internet.
3. Espera a que cargue completamente.
4. Usa el botón **Instalar aplicación** cuando el navegador lo ofrezca, o el menú del navegador → **Instalar aplicación / Añadir a pantalla de inicio**.
5. La aplicación instalada será una PWA gestionada por el navegador.

## Importante sobre Play Protect

El aviso de Google Play Protect de "app diseñada para una versión anterior de Android" corresponde a un **APK**. Una PWA pura no contiene `targetSdkVersion`, `compileSdkVersion` ni configuración de APK.

Por tanto, **no conviertas este proyecto a APK con un generador Android antiguo** si quieres mantenerlo como PWA.

## Actualizaciones

El Service Worker usa una versión de caché propia. Cuando publiques cambios importantes, incrementa `CACHE_NAME` en `sw.js` (por ejemplo `v4`, `v5`, etc.).
