# Api

Import the runtime to add event listeners or trigger actions

```typescript
import { addRoutingEventListener } from "photon-re";
import type { RoutedEvent } from "photon-re";

addRoutingEventListener("routed", (ev: RoutedEvent): void => {
  console.debug(ev.detail.route);
});
```
