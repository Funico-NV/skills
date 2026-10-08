# README examples

Use these examples when creating a new README or substantially restructuring one. They demonstrate the intended hierarchy, density, and use of visual emphasis; they are not templates. Verify every name, command, compatibility claim, link, and status against the repository before adapting anything.

## Package or library

````markdown
# Event Client

![Status: stable](https://img.shields.io/badge/status-stable-2ea44f)

Event Client is a TypeScript package for publishing domain events to the internal event gateway. Applications provide their own authentication and transport configuration.

## Install

```bash
npm install @example/event-client
```

## Publish an event

```ts
import { EventClient } from "@example/event-client";

const client = new EventClient({ endpoint: process.env.EVENT_ENDPOINT });

await client.publish({
  type: "order.created",
  payload: { orderId: "order_123" },
});
```

`EVENT_ENDPOINT` must point to an event gateway that the application can reach.

## Compatibility

| Runtime | Supported versions |
| --- | --- |
| Node.js | 22 and later |
````

Why this works:

- The opening paragraph states the package's purpose and boundary.
- The badge communicates status through both text and color.
- Installation leads directly to the smallest useful example.
- The compatibility table provides a genuine mapping rather than decoration.

## Application or service

````markdown
# Invoice Worker

![Status: preview](https://img.shields.io/badge/status-preview-d97706)

Invoice Worker creates invoice PDFs from queued billing events. It processes existing events but does not collect payments or send customer email.

## Run locally

Install dependencies and start the development worker:

```bash
npm install
npm run dev
```

Submit a local test event:

```bash
curl --request POST http://localhost:8787/events \
  --header "content-type: application/json" \
  --data '{"invoiceId":"invoice_123"}'
```

## Configuration

| Variable | Purpose | Required |
| --- | --- | --- |
| `INVOICE_BUCKET` | Stores generated PDF files | Yes |
| `LOG_LEVEL` | Sets application log verbosity | No |

> [!WARNING]
> Replaying a production event can overwrite an existing invoice. Use a test invoice ID during local development.

## Test

```bash
npm test
```
````

Why this works:

- The description names both the responsibility and the boundary.
- Commands follow the normal path from setup to a visible result.
- The configuration table makes required input easy to scan.
- The warning calls out a concrete, consequential risk; it is not decorative.

## Adaptation rules

- Keep only sections supported by the project.
- Prefer one meaningful status badge over a row of decorative badges.
- Preserve readable badge text so color is never the only status signal.
- Add a callout only when separating the content changes how safely or efficiently the reader acts.
- Replace illustrative commands and identifiers with verified project details.
