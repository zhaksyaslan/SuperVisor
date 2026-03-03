# SuperVisor Plugin

SuperVisor is a monitoring and incident-orchestration plugin for web applications and services.

## What It Does

- Monitors HTTP endpoints, queues, and service health in real time
- Tracks latency, errors, and incident signals in one dashboard
- Sends alerts to Slack, Telegram, and webhooks
- Supports automated recovery actions on incident triggers

## Installation

```bash
npm install supervisor-plugin
# or
pnpm add supervisor-plugin
```

## Quick Start

```ts
import { createSupervisor } from 'supervisor-plugin';

const sv = createSupervisor({
  project: 'my-app',
  token: process.env.SUPERVISOR_TOKEN,
});

sv.monitorHttp('/health');
sv.monitorQueue('jobs');
```

## Screenshots

### Dashboard
![SuperVisor dashboard](./assets/dashboard-overview.png)

### Incident Details
![SuperVisor incident details](./assets/incident-details.png)

### Alert Workflows
![SuperVisor alert workflows](./assets/alert-workflows.png)

### Operations Control
![SuperVisor operations control](./assets/ops-control.png)

## Documentation

- [Product Docs](../docs.html)
- [Installation Section](../docs.html#install)
- [Quick Start Section](../docs.html#config)
- [Alerts Section](../docs.html#alerts)
- [Integrations Section](../docs.html#integrations)
- [FAQ Section](../docs.html#faq)

## Legal

- [EULA](./EULA.md)
- [Privacy Policy](./PRIVACY_POLICY.md)
