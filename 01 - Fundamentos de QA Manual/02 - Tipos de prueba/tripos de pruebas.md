Aquí tienes un diagrama que organiza la información sobre los tipos de pruebas de software:

```
┌───────────────────────────────────────────────────────────────────────────────┐
│                            PRUEBAS DE SOFTWARE                                │
└───────────────────────────────────────────────────────────────────────────────┘
                                      │
                      ┌───────────────┴──────────────────┐
                      │                                  │
           ┌──────────▼───────────┐            ┌─────────▼─────────┐
           │  PRUEBAS ESTÁTICAS   │            │ PRUEBAS DINÁMICAS │
           │ (Sin ejecutar código)│            │(Ejecutando código)│
           └──────────┬───────────┘            └─────────┬─────────┘
                      │                                  │
           ┌──────────┴──────────┐            ┌──────────┴────────────────────┐
           │ Análisis Estático   │            │ Se clasifican en:             │
           │ (Revisión de código,│            │ 1. Según su objetivo          │
           │ documentación, etc.)│            │ 2. Según conocimiento interno │
           └─────────────────────┘            └──────────┬────────────────────┘
                                                         │
                            ┌────────────────────────────┴───────────────────────────────┐
                            │                                                            │
                ┌───────────▼────────────┐                                 ┌─────────────▼─────────────┐
                │ PRUEBAS FUNCIONALES    │                                 │ PRUEBAS NO FUNCIONALES    │
                │ (Verifican requisitos) │                                 │ (Evalúan atributos)       │
                └───────────┬────────────┘                                 └─────────────┬─────────────┘
                            │                                                            │
        ┌───────────────────┴─────────────────────────────┐                   ┌──────────┴─────────────┐
        │                   │              │              │                   │                        │
┌───────▼───────┐   ┌───────▼────────┐ ┌───▼─────────┐ ┌─▼─────────────┐   ┌─▼─────────────┐   ┌─────▼─────┐
│ Unitarias     │   │ Integración     │ │ Sistema     │ │ Aceptación    │   │ Rendimiento   │   │ Seguridad │
│ (Unidades     │   │ (Interacción    │ │ (Software   │ │ (Usuario final│   │ (Velocidad,   │   │ (Protección│
│ individuales) │   │ entre módulos)  │ │ completo)   │ │ valida)       │   │  estabilidad) │   │ contra    │
└───────────────┘   └─────────────────┘ └─────────────┘ └───────────────┘   └──────────────┘   │ ataques)  │
                                                                                              └───────────┘

    Técnicas funcionales:
    ┌─────────────┬─────────────┬──────────────┐
    │ Caja Negra  │ Caja Blanca │ Caja Gris    │
    │ (Sin        │ (Con        │ (Combinación │
    │ conocimiento│ conocimiento│ de ambas)    │
    │ interno)    │ interno)    │              │
    └─────────────┴─────────────┴──────────────┘

┌──────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                      │
│  ┌────────────────────────┐  ┌───────────────┐  ┌───────────────┐  ┌───────────────┐ │
│  │ Pruebas de Regresión   │  │ Pruebas de    │  │ Pruebas Smoke │  │ Pruebas de    │ │
│  │ (Verificar cambios)    │  │ Compatibilidad│  │ (Básica       │  │ Usabilidad    │ │
│  └────────────────────────┘  │ (Entornos     │  │ funcionalidad)│  │ (Facilidad    │ │
│                              │ diferentes)   │  │               │  │ de uso)       │ │
│                              └───────────────┘  └───────────────┘  └───────────────┘ │
│                                                                                      │
└──────────────────────────────────────────────────────────────────────────────────────┘
```

### Notas:
1. **Pruebas Estáticas**: Solo incluyen análisis estático (revisión de código/documentación).
2. **Pruebas Dinámicas**:
   - **Funcionales**: Se dividen por objetivo (Unitarias, Integración, Sistema, Aceptación). Se pueden aplicar técnicas de Caja Negra, Blanca o Gris.
   - **No Funcionales**: Rendimiento, Seguridad, Usabilidad, etc.
3. **Otros tipos comunes**: Pruebas de Regresión, Compatibilidad, Smoke, Usabilidad, etc. Pueden ser funcionales o no funcionales según el contexto.
4. **Relaciones**:
   - Las pruebas Unitarias/Integración/Sistema/Aceptación suelen ser funcionales.
   - Las pruebas Smoke y Regresión pueden aplicarse a ambos grupos.

¿Te gustaría profundizar