# Estructura del repositorio / Repository structure

softwart-docs/
│
├── README.md
├── STRUCTURE.md                          ← este archivo
│
├── manual-tecnico/
│   └── manual-tecnico-v3.docx            ← manual técnico completo
│
├── diagramas/
│   │
│   ├── casos-de-uso/
│   │   ├── 00-general.png
│   │   ├── 01-configuracion.png
│   │   ├── 02-usuarios-acceso.png
│   │   ├── 03-portal-cliente.png
│   │   ├── 04-servicios-marcos.png
│   │   ├── 05-diseno-aprobacion.png
│   │   ├── 06-ventas.png
│   │   ├── 07-medicion-desempeno.png
│   │   └── documentacion/
│   │       └── Documentacion_CasosDeUso_SoftwArt.docx
│   │
│   ├── c4/
│   │   ├── c4-contexto.png
│   │   ├── c4-contenedor.png
│   │   └── c4-componentes.png
│   │
│   ├── clases/
│   │   └── diagrama-clases.png
│   │
│   ├── facilitacion-grafica/
│    	   └── facilitacion-grafica.png
│
│
│
│
├── mhu/
│   ├── MHU_Marqueteria.xlsx              ← visión, épicas y matriz HU completa
│   
│
├── product-backlog/
│   └── product-backlog.xlsx
│
└── story-mapping/
    └── Story_Mapping_SoftwArt.xlsx

## Notas

- Los diagramas de casos de uso se exportan desde [mermaid.live](https://mermaid.live) — el código fuente de cada diagrama está en el manual técnico, sección 11.1.
- Los diagramas C4 y el diagrama de clases corresponden a las secciones 12 y 11.3 del manual técnico respectivamente.
- La MHU contiene tres hojas: **Visión Proyecto**, **Epicas** y **Formato Matriz HU**.
- El product backlog usa codificación jerárquica (`01.1.1`, `01.1.2`...) alineada con la MHU.
