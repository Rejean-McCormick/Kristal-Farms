# Kristal Farms documentation

This documentation covers the **Kristal Farms infrastructure project** and the application/data system used to explain, research and evaluate it.

## Read in this order

### Project

1. [Project state](00-control/PROJECT_STATE.md)
2. [Kristal Wink / éolienne autonome — FR](10-core/KRISTAL_WINK_ARCHITECTURE_FR.md)
3. [Kristals opératoires et hors ligne — FR](10-core/KRISTALS_OFFLINE_ET_PROCEDURES_FR.md)
4. [Gouvernance collective et Assemblée des fondateurs — FR](00-control/KRISTAL_GOUVERNANCE_COLLECTIVE_FR.md)
5. [Strategic principles](00-control/STRATEGIC_PRINCIPLES.md)
6. [Project reference architecture — English](10-core/Kristal_Farms_Project_Reference_Architecture_EN.md) or [architecture de référence du projet — français](10-core/Architecture_de_reference_du_projet_Kristal_Farms_FR.md)
7. [Deployment strategy — English](10-core/deployment/DEPLOYMENT_STRATEGY_EN.md) or [stratégie de déploiement — français](10-core/deployment/STRATEGIE_DE_DEPLOIEMENT_FR.md)
8. [Corridor dossier strategy](00-control/CORRIDOR_DOSSIER_STRATEGY.md)
9. [Responsible international tenant governance](00-control/INTERNATIONAL_TENANT_GOVERNANCE.md)
10. [Plan de mobilisation internationale — français](10-core/strategy/PLAN_MOBILISATION_INTERNATIONALE_KRISTAL_FARMS_FR.md)
11. [Tenant-controlled encrypted environment — English](10-core/tenancy/BLACK_BOX_TENANCY_MODEL_EN.md) or [environnement chiffré sous contrôle du locataire — français](10-core/tenancy/MODELE_LOCATION_BLACK_BOX_FR.md)

### Application and data

1. [Application product vision](product/vision.md)
2. [Software & data platform architecture](architecture/overview.md)
3. [Information architecture](architecture/information-architecture.md)
4. [Kristal Farms domain principles](domain/kristal-farms-principles.md)
5. [Data model](data/data-model.md)
6. [Evidence model](data/evidence-model.md)
7. [Map observatory interaction](frontend/map-observatory-interaction.md)
8. [Layer catalog](frontend/layer-catalog.md)
9. [API overview](api/overview.md)
10. [Implementation plan](roadmap/implementation-plan.md)

### Mine infrastructure reuse and storage

1. [Mine reuse screening method](30-site-screening/mine-reuse/MINE_REUSE_SCREENING_METHOD.md)
2. [Underground compute / mine infrastructure reuse](30-site-screening/mine-reuse/UNDERGROUND_COMPUTE_REUSE.md)
3. [Mine-pit reservoir and pumped-storage research](30-site-screening/mine-reuse/MINE_RESERVOIR_PUMPED_STORAGE.md)
4. [Northern mine-reuse inventory](50-research/mines/NORTHERN_MINE_REUSE_INVENTORY.md)

### International tenancy and mobilization

1. [Plan de mobilisation internationale — français](10-core/strategy/PLAN_MOBILISATION_INTERNATIONALE_KRISTAL_FARMS_FR.md)
2. [Responsible international tenant governance](00-control/INTERNATIONAL_TENANT_GOVERNANCE.md)
3. [Tenant confidentiality boundary](security/TENANT_CONFIDENTIALITY_BOUNDARY.md)
4. [Tenant due-diligence runbook](operations/TENANT_DUE_DILIGENCE_RUNBOOK.md)
5. [International tenant landscape](50-research/commercial/INTERNATIONAL_TENANT_LANDSCAPE.md)

## Documentation authority

The active authority order is defined in [Document Authority](00-control/DOCUMENT_AUTHORITY.md). In short:

- current project-control documents govern intent and interpretation;
- current project reference architecture governs the physical/commercial model;
- source evidence governs factual claims within its actual scope;
- assumptions remain assumptions;
- archived material never silently overrides active state.

## Documentation philosophy

The repository separates three kinds of active documentation:

- **Normative:** rules the project data/software must obey.
- **Descriptive:** how the current project/application implementation works.
- **Decision records:** why a durable technical choice was made.

Normative documents use terms such as **MUST**, **MUST NOT**, **SHOULD**, and **MAY** intentionally.

## Machine-readable contracts

The `contracts/` directory contains schemas and policy files intended to be consumed by code, tests, CI and coding agents. Human documentation and machine contracts must remain consistent.

## Long-horizon material

Optional human-infrastructure, learning and education concepts are isolated under [Long-Horizon Concepts](70-long-horizon/README.md). They are not prerequisites or commitments for the first energy/compute deployment.

## Owner-directed concept update (2026-10-12)

The **offline-first Kristal Wink** option is documented above and in [proposed ADR-0024](adr/0024-offline-first-kristal-wink-direction.md). Connected fibre tenancy remains supported, but continuous high-capacity fibre is no longer a universal dependency in the project vision. Earlier site economics and evidence claims were not recalculated for this new scenario.
