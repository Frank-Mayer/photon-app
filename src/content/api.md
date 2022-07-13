# Api

Import the runtime to add custom page logic.

Parameters are filled using url search parameters if given (undefined if not).

```typescript
import { page } from "photon-re";

export class MyPages {
  @page("/")
  public index(q?: string) {
    console.log("q", q);
  }

  @page("/foo/**")
  public foo() {
    // ...
  }
}
```

You can import `dotenv` to check if you are in a production environment.

Development environment is defined by the check: `http:` protocol or `localhost` (or `127.0.0.1`).

```typescript
import { dotenv } from "photon-re";

if (dotenv.production) {
  // production
} else {
  // development
}
```
