# Portón - Hardware (PCB)

Proyecto de hardware (PCB) para un sistema de portón automatizado basado en ESP32-S3.

## Estructura del repositorio

- `kicad/` — Proyecto KiCad (esquemático y PCB).
- `bom/` — Lista de componentes (Bill of Materials) exportada desde KiCad.
- `datasheets/` — Hojas de datos de los componentes principales.

## Componentes principales

- **MCU:** ESP32-S3-WROOM-1
- **Driver de motor (Puente H):** DRV8871
- **Regulador buck:** C780769 (3.8V–32V, 2A)
- **Otros:** ver `bom/BOM_porton.csv`

## Cómo abrir el proyecto

1. Instalar [KiCad 10.0+](https://www.kicad.org/).
2. Abrir `kicad/porton.kicad_pro`.

## Generar BOM

```bash
kicad-cli sch export bom -o bom/BOM_porton.csv kicad/porton.kicad_sch
```

## Licencia

(Definir licencia)
