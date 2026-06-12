# @meraki/plans

Gemeinsame Lizenz-Plan-Definitionen für **Meraki CMS** und **Meraki License Server** — die einzige Quelle der Wahrheit für `PLAN_DEFINITIONS` und `PLAN_MODULES`.

## Verwendung

Als Git-Dependency in `package.json`:

```json
"dependencies": {
    "@meraki/plans": "github:stb-srv/meraki-plans"
}
```

CommonJS (meraki-cms):

```js
const { PLAN_DEFINITIONS, PLAN_MODULES } = require('@meraki/plans');
```

ESM (meraki-licens):

```js
import { PLAN_DEFINITIONS, PLAN_MODULES } from '@meraki/plans';
```

## Regeln

- Plan-Definitionen **nur hier** bearbeiten — nie in den konsumierenden Projekten duplizieren.
- Nach Änderungen in den Konsumenten `npm update @meraki/plans` ausführen, damit die neue Version gezogen wird.
- Modul-Namen immer über die `PLAN_MODULES`-Konstanten referenzieren, nicht als String-Literale.
