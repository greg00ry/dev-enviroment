# dev-environment

Platforma deweloperska: wspólny silnik Operaton (BPMN/DMN) + Postgres jako backend, pod który podpinają się fronty poszczególnych projektów.

## Komponenty

| Katalog | Co to jest | Stack |
|---|---|---|
| [`operaton/`](operaton) | Silnik procesowy BPMN/DMN | Java 21, Spring Boot, Operaton |
| [`postgres/`](postgres) | Baza danych | PostgreSQL 16 |
| [`adminer/`](adminer) | Podgląd/edycja bazy | Adminer |
| [`codeserver/`](codeserver) | VS Code w przeglądarce (z Pythonem) | code-server |
| [`drawio/`](drawio) | Diagramy architektury (C4, BPMN, UML) | draw.io |

## Uruchomienie

Każdy katalog ma własny `compose.yaml` (zarządzane przez Dockge). Lokalnie:

```bash
cd <katalog>
docker compose up -d --build
```

## Status

Projekt na wczesnym etapie, budowany od zera.
