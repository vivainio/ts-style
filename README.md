
# Classes and interfaces

- Prefer interfaces
- Use classes only when your objects are participating in Dependency Injection.
- Do not mark public elements in classes as "public". It's default.

# Module pattern

Use "static class" instead of freestanding function to collect functionality (to make it cleaner where utility is coming from)

```typescript

// static
export class FooUtil {
  static bar() {
    // ...
  }
}
```

# Lifecycle

- OnPush change detection everywhere
- Do almost nothing in constructor
- Register observers in ngOnInit
- Avoid ngOnChanges when you can

# Misc

- Prefer promises to RxJS observables
- Prefer "then" to async/await for now (because async/await does not give perfect source maps)
- When using observables do NOT store subscriptions anywhere. Use automatic disposers


```



