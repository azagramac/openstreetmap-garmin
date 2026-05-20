[![🛠️ Build map](https://github.com/azagramac/OSMforGarmin/actions/workflows/workflow-spain.yaml/badge.svg)](https://github.com/azagramac/OSMforGarmin/actions/workflows/workflow-spain.yaml)

# 🛰️ Garmin Map Builder – OpenStreetMap
<img width="96" alt="osm-logo" src="https://github.com/user-attachments/assets/cbe6581f-0e95-443f-8d97-7ee3fb2ec22a" />

Compilación de mapas .img compatibles con dispositivos Garmin eTrex 22x / 30x / 32x / GPSMAP 66, 67... y similares, usando datos oficiales de OpenStreetMap.

<img width="240" height="320" alt="imagen" src="https://github.com/user-attachments/assets/8e6c5f65-7af5-4761-9f2b-76638043a326" />
<img width="240" height="320" alt="imagen" src="https://github.com/user-attachments/assets/11b08321-67a4-4b25-99c5-adb66d5c7622" />


---

## 🚀 Características

- ✅ Generación automática del fichero `*-gmapsupp.img` de diferentes regiones, España Peninsular, Islas Canarias e Islas Baleares de [Geofabrik](https://download.geofabrik.de/europe/spain.html).

---

## 📱 Dispositivos compatibles

| 🛰️ Dispositivo            | 💾 Memoria interna               | 💿 Tarjeta SD / microSD         | 📝 Notas |
|----------------------------|---------------------------------|--------------------------------|----------|
| Garmin eTrex 20 / 22x      | ✅ Solo `gmapsupp.img`           | ✅ Acepta múltiples nombres      | Recomendado usar SD para varios mapas |
| Garmin eTrex 30 / 32x      | ✅ Solo `gmapsupp.img`           | ✅ Acepta múltiples nombres      | Probado con éxito con este proyecto |
| Garmin GPSMAP 64           | ✅ Solo `gmapsupp.img`           | ✅ Acepta múltiples nombres      | Recomendado usar SD para varios mapas |
| Garmin GPSMAP 65s          | ✅ Solo `gmapsupp.img`           | ✅ Acepta múltiples nombres      | — |
| Garmin GPSMAP 66i,st,sr | ❌ No reconoce en interna        | ✅ Requiere SD y renombrar a `gmapsupp.img` | ⚠️ Importante: siempre en SD |
| Garmin GPSMAP 67 / 67i     | ❌ No reconoce en interna        | ✅ Requiere SD y renombrar a `gmapsupp.img` | — |
| Otros Garmin compatibles   | ✅ Normalmente `gmapsupp.img`    | ✅ Acepta múltiples nombres      | Depende del modelo y firmware |

---

## 📂 Archivo generado

- `peninsula-gmapsupp.img`: Mapa principal con la región España 🇪🇸 (península).
- `canarias-gmapsupp.img`: Mapa con la región 🇮🇨 Islas Canarias.
- `baleares-gmapsupp.img`: Mapa con la región 🏝️ Islas Baleares.

---

## 📦 Instalación
💽 En memoria interna Garmin

- Conecta el dispositivo Garmin por USB.
- Renombra `*-gmapsupp.img` correspondiente a `gmapsupp.img`.
- Copia `gmapsupp.img` dentro de la carpeta `Garmin`.

💾 En tarjeta SD externa (recomendada para múltiples mapas)

- Inserta la tarjeta SD (formateada en `FAT32`, máximo 32GB).
- Crea la carpeta `Garmin` en la raíz.
- Copia el fichero `*-gmapsupp.img` (puedes renombrar para tener varios mapas simultáneos, ej.: `peninsula-gmapsupp.img`, `baleares-gmapsupp.img`, `canarias-gmapsupp.img`, ...) dentro de la carpeta `Garmin`.

> ⚠️ Nota: En memoria interna del dispositivo solo se reconoce un archivo .img llamado `gmapsupp.img`
> En tarjeta SD puedes tener varios mapas con diferentes nombres.

> ⚠️ Nota: en los dispositivos GPSMAP como el 66 (probado en 66st), hay que copiar el fichero `*-gmapsupp.img`, renombrarlo a `gmapsupp.img`, y copiarlo a `Garmin` en la tarjeta MicroSD. No copiar a la memoria interna del GPSMAP!!!. 

### ⚙️ Activación del mapa en el dispositivo Garmin
<img width="240" height="320" alt="imagen" src="https://github.com/user-attachments/assets/0e9a8318-0652-4c84-ad09-519cead889cb" />
<img width="240" height="320" alt="imagen" src="https://github.com/user-attachments/assets/6fd81662-9777-4603-9a51-740d966a42c5" />
<img width="240" height="320" alt="imagen" src="https://github.com/user-attachments/assets/3cff965a-d91c-4911-8cd9-39505259977a" />
<img width="240" height="320" alt="imagen" src="https://github.com/user-attachments/assets/c599c9b7-cb08-4377-91f6-a8bb467472e3" />

---

## 🧪 Environment
- ☕ Java 17
- 📦 [mkgmap](https://www.mkgmap.org.uk/download/mkgmap.html) `r4924`
- 🔀 [splitter](https://www.mkgmap.org.uk/download/splitter.html) `r654`
- 🗺️ Datos OSM de [Geofabrik](https://download.geofabrik.de/)
