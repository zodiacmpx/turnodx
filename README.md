# TurnoDX

TurnoDX is a lightweight, browser-based shift scheduling tool for operational teams. It generates monthly schedules with weekday and weekend night rotations, rest periods, manual overrides, local persistence, and CSV export.

> TurnoDX is an early-stage project. Generated schedules must be reviewed by a responsible person before operational use and checked against applicable labor rules and local requirements.

## Features

- Monthly calendar generation
- Strict round-robin night-shift allocation
- Weeknight blocks (Monday–Thursday)
- Weekend night blocks (Friday–Sunday)
- Post-night rest periods
- Manual shift editing
- Lockable assignments that survive regeneration
- Local browser storage
- CSV export for spreadsheet use
- No backend, account, or paid service required

## Quick start

1. Clone or download this repository.
2. Open `index.html` in a modern browser.
3. Select a month and year.
4. Choose **Generar con Rotación**.
5. Review and adjust every assignment before use.

No build step or dependency installation is required.

## Shift codes

| Code | Meaning |
| --- | --- |
| `D` | Day shift |
| `T` | Afternoon shift |
| `NS` | Weeknight shift |
| `NF` | Weekend night shift |
| `L` | Rest day |

Left-click a calendar cell to cycle through shift types. Right-click it to lock or unlock the assignment. Locked assignments are preserved when the schedule is regenerated.

## Data and privacy

TurnoDX runs entirely in the browser. Saved schedules use the browser's `localStorage` and are not sent to a server by this project.

The repository contains fictional sample personnel. Before using TurnoDX, replace the sample configuration with appropriate data and follow your organization's privacy and data-handling requirements. Do not commit personal or sensitive operational data to a public repository.

## Current limitations

- Personnel and scheduling rules are currently configured in `index.html`.
- The generator uses randomized day and afternoon allocation.
- It does not guarantee compliance with employment contracts, collective agreements, staffing minimums, fatigue-management policies, or local labor law.
- Automated tests and configurable personnel inputs are planned.

## Roadmap

- Move personnel and rules into an editable configuration interface
- Add deterministic generation and reproducible schedules
- Add automated tests for fairness and rest constraints
- Validate staffing coverage by location and shift
- Improve accessibility and mobile support
- Add import/export for reusable configurations
- Provide English and Spanish interfaces

## Contributing

Issues and pull requests are welcome. When proposing a scheduling change, describe the operational rule, include a small example, and explain the expected result. Please avoid including real employee information in examples, tests, screenshots, or issue reports.

## License

TurnoDX is available under the [MIT License](LICENSE).

---

## Español

TurnoDX es una herramienta liviana de planificación de turnos que funciona directamente en el navegador. Genera calendarios mensuales con rotaciones nocturnas de semana y fin de semana, descansos posteriores, modificaciones manuales, almacenamiento local y exportación CSV.

No requiere servidor ni instalación de dependencias. Abre `index.html`, selecciona el mes y año, genera el calendario y revisa cuidadosamente cada asignación antes de utilizarla.

TurnoDX es un proyecto en etapa inicial y no sustituye la revisión humana ni garantiza por sí solo el cumplimiento de contratos, dotaciones mínimas, políticas internas o legislación laboral. Los ejemplos del repositorio son ficticios; no publiques información personal o sensible.
