# VIGÍA — Documentación académica (archivo de investigación)

> **Estado: en mantenimiento, desactualizado.** Este repositorio es un volcado (copy-paste, sin historia de git) de la carpeta `docs/academic/` del repositorio principal [`vigia-intent-analysis`](https://github.com/annatchijova/vigia-intent-analysis), tal como estaba el **5 de noviembre de 2026**. VIGÍA hoy tiene más de 500 módulos Python y una lógica interna que ya avanzó más allá de lo que describen varios de estos documentos. No reflejan necesariamente el estado actual del motor — se publican como material de investigación y referencia teórica, no como documentación técnica vigente.

## Por qué existe este repo separado

El repositorio principal de VIGÍA avanza rápido y su documentación académica interna (en `docs/academic/`) queda desactualizada entre revisiones. En vez de dejar esos ~198 documentos enterrados sin acceso público, se separan acá para poder compartirlos con investigadores — en particular para seguir difundiendo la aplicación de la semiótica de **Charles Sanders Peirce** (y de Eco, Grice y Carnegie) a sistemas de inferencia forense, que es el núcleo teórico de VIGÍA.

Con el tiempo se va a actualizar y ampliar este archivo para que refleje mejor la arquitectura actual de +500 módulos y su razón de ser. Por ahora es una fotografía, no un documento vivo.

## Empezar por acá

- **[VIGIA_RESEARCH_REPORT.md](VIGIA_RESEARCH_REPORT.md)** ([EN](VIGIA_RESEARCH_REPORT_EN.md)) — la investigación extensa sobre por qué VIGIA tiene razón de existir: la crisis del DFIR tradicional, el problema de los EDR como cajas negras, y la propuesta de un motor de inferencia abductiva determinista que separa evidencia de narrativa LLM. Generado originalmente por un swarm de agentes Kimi K2, corregido y verificado contra el repositorio en vivo por Claude — ver cabecera del documento para el detalle de autoría.
- **[ACADEMIC_DOCS_MASTER_INDEX.md](ACADEMIC_DOCS_MASTER_INDEX.md)** — índice maestro de los 192 módulos documentados, organizados por área (`core`, `tools`, `sift`, `forensics`, `inference`, `pipeline`, `security`, `scripts`, `governance`, `specialized`). También disponible en [inglés](ACADEMIC_DOCS_MASTER_INDEX_EN.md), [ruso](ACADEMIC_DOCS_MASTER_INDEX_RU.md) y [chino](ACADEMIC_DOCS_MASTER_INDEX_ZH.md).

## Estructura

```
.
├── VIGIA_RESEARCH_REPORT.md / _EN.md       ← por qué VIGIA debe existir (ES/EN)
├── ACADEMIC_DOCS_MASTER_INDEX.md           ← índice maestro (ES)
│                        _EN.md / _RU.md / _ZH.md   ← mismo índice en inglés/ruso/chino
├── core/            — 38 docs — pipeline central, semiótica, señales, calibración
├── tools/           — 22 docs — CAIE, NLP adversarial, MITRE, patrones, EML
├── sift/            —  9 docs — MFT, prefetch, shellbag, registry, network, browser, memory
├── forensics/       —  5 docs — PDF, PKI, RFC3161, visión, cadena de custodia
├── inference/       —  5 docs — razonamiento abductivo, fingerprint conductual
├── pipeline/        —  4 docs — bundle, report, bridge SIFT, registro de evidencia
├── security/        —  4 docs
├── governance/       —  2 docs
├── specialized/      —  2 docs
├── scripts/          — 10 docs
├── root/             — 13 docs — misceláneos de nivel raíz del corpus original
└── unclassified/     — 78 docs — pendientes de reclasificar dentro del esquema anterior
```

Cada documento cubre su módulo con nota científica sobre la semiótica de Peirce, Eco y Grice, y en varios casos con glosario técnico multilingüe — ver el encabezado de cada archivo para su cobertura de idiomas exacta.

## Licencia

**Apache License 2.0** — ver [LICENSE](LICENSE). Misma licencia que el repositorio principal [`vigia-intent-analysis`](https://github.com/annatchijova/vigia-intent-analysis), porque este archivo es parte de ese mismo proyecto y usar una licencia distinta no tendría sentido.

## Autoría

Mismo régimen de autoría que el proyecto VIGÍA: la arquitectura, las decisiones teóricas y el diseño pertenecen a **Anna Tchijova**; varios documentos fueron redactados por un colectivo de modelos de IA (Kimi K2, Claude, y otros según el documento — ver la cabecera de cada archivo) bajo su dirección y corregidos contra el repositorio en vivo. Ver [`AUTHORS.md`](https://github.com/annatchijova/vigia-intent-analysis/blob/main/AUTHORS.md) del repositorio principal para el detalle completo.

## Repositorio principal

El código, los tests y la documentación técnica vigente viven en [`github.com/annatchijova/vigia-intent-analysis`](https://github.com/annatchijova/vigia-intent-analysis). Este repositorio es solo el archivo de la documentación académica.
