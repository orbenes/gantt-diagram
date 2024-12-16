# Proceso de Viaje del Cliente de NOMII - Diagrama de Gantt

```mermaid
gantt
    title Proceso de Viaje del Cliente de NOMII - Línea de Tiempo
    dateFormat  YYYY-MM-DD
    excludes weekends

    %% Inicio: Pool de Médicos
    section Inicio
    Pool de Médicos :a1, 2024-01-01, 1d

    %% Fase LATAM
    section Fase LATAM
    Pago Inicial (2/3 de 21.900 €) :a2, after a1, 1d
    Opciones de Financiamiento      :a3, after a2, 3d
    Preparación de Documentos y Alemán :a4, after a3, 180d
    Traducciones y DHL             :a5, 2024-07-05, 1d
    Solicitud de Visa (Chancenkarte):a6, after a5, 30d
    Costos de Vuelo y Seguro        :a7, after a6, 1d

    %% Fase Alemania
    section Fase Alemania
    Pago 1/3 (7.300 €)              :b1, after a7, 1d
    Financiamiento ApoBank          :b2, after b1, 3d
    PA Insertion (Trabajo parcial)   :b3, after b2, 90d
    Preparación FSP                  :b4, after b3, 150d
    Pago FSP Gebühr (350 €)          :b5, after b4, 1d
    FSP genehmigen                   :b6, after b5, 1d
    BE Personalvermittlung Fee (4.650 €) :b7, after b6, 1d
    Permiso Profesional              :b8, after b7, 30d
    Trabajo en Geriatría/Familiares  :b9, after b8, 365d
    Ingresos por Telemedicina        :b10, after b9, 365d
    Creación de KP con Apoyo NOMII    :b11, after b9, 180d
    Preparación KP y Pago            :b12, after b11, 120d
    KP aprobado => Approbation       :b13, after b12, 1d
    Fee de Personalvermittlung para Approbation (5.200 €) :b14, after b13, 1d
    Hochbedarfsfachstelle 1, 2, 3     :b15, after b14, 30d

    %% Ingresos por Alquiler (solo 3 médicos)
    section Ingresos por Alquiler
    Ingresos Alquiler Médico 1 (150-200 €/Mes) :m1, after b3, 365d
    Ingresos Alquiler Médico 2 (150-200 €/Mes) :m2, after b3, 365d
    Ingresos Alquiler Médico 3 (150-200 €/Mes) :m3, after b3, 365d

    %% Ingresos por Apertura de Cuenta Bancaria y Seguro
    Ingresos Apertura Cuenta Bancaria y Seguro (~300 €) :m4, after b9, 1d

    %% Otros Gastos
    Otros Gastos (Variables) :c1, after b12, 365d

    %% Meilensteine (Hitos)
    milestone Entrega Visa, 2024-10-01, 0
    milestone Inicio Trabajo como Médico, 2025-05-04, 0
    milestone Approbation obtenida, 2026-03-01, 0

    %% Estilos personalizados usando 'style'
    style a1 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style a2 fill:#2ecc71,stroke:#333,stroke-width:1px, color:#ffffff
    style a3 fill:#e67e22,stroke:#333,stroke-width:1px, color:#ffffff
    style a4 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style a5 fill:#e74c3c,stroke:#333,stroke-width:1px, color:#ffffff
    style a6 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style a7 fill:#e74c3c,stroke:#333,stroke-width:1px, color:#ffffff
    style b1 fill:#2ecc71,stroke:#333,stroke-width:1px, color:#ffffff
    style b2 fill:#e67e22,stroke:#333,stroke-width:1px, color:#ffffff
    style b3 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style b4 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style b5 fill:#e74c3c,stroke:#333,stroke-width:1px, color:#ffffff
    style b6 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style b7 fill:#2ecc71,stroke:#333,stroke-width:1px, color:#ffffff
    style b8 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style b9 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style b10 fill:#2ecc71,stroke:#333,stroke-width:1px, color:#ffffff
    style b11 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style b12 fill:#e74c3c,stroke:#333,stroke-width:1px, color:#ffffff
    style b13 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style b14 fill:#2ecc71,stroke:#333,stroke-width:1px, color:#ffffff
    style b15 fill:#1f77b4,stroke:#333,stroke-width:1px, color:#ffffff
    style m1 fill:#2ecc71,stroke:#333,stroke-width:1px, color:#ffffff
    style m2 fill:#2ecc71,stroke:#333,stroke-width:1px, color:#ffffff
    style m3 fill:#2ecc71,stroke:#333,stroke-width:1px, color:#ffffff
    style m4 fill:#2ecc71,stroke:#333,stroke-width:1px, color:#ffffff
    style c1 fill:#e74c3c,stroke:#333,stroke-width:1px, color:#ffffff
