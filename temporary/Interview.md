Introduce yourself

Describe your latest project that uses angular

  

Compare between versions of Angular

|Feature|Angular 18 (2024)|Angular 21 (2025)|Angular 22 (2026)|
|---|---|---|---|
|Support|❌ End of support|✅ LTS|✅ Active|
|Signals|Stable|Mature ecosystem|First-class reactive model|
|Standalone Components|Recommended|Default approach|Standard|
|Control Flow (`@if`, `@for`)|✅ Stable|✅|✅|
|Zoneless|Experimental|Stable|Default for new apps|
|Signal Forms|Experimental|Developer Preview|✅ Stable|
|`resource()` / `httpResource()`|Experimental|Developer Preview|✅ Stable|
|Change Detection|`Default` or `OnPush`|Same|**OnPush by default**|
|Test Runner|Karma/Jasmine|Vitest supported|Vitest is primary|
|SSR/Hydration|Basic hydration|Improved|Incremental hydration by default|


1 câu hỏi về tech của angular (Singal, Standalone component, zoneless)

A Signal is Angular's reactive state management primitive. It stores a value and automatically updates anything that depends on it when the value changes.

A Standalone Component is an Angular component that doesn't need to be declared in an NgModule. Instead, it declares its own dependencies using the imports property, making components more self-contained, reusable, and easier to maintain.
**Before**

```
Component
    ↓
NgModule
    ↓
Application
```

Every component had to belong to an `NgModule`.

**Now**

```
Component
    ↓
imports
    ↓
Application
```

The component manages its own dependencies.

Zoneless is a way to run Angular without `zone.js`. Traditionally, Angular relied on `zone.js` to detect asynchronous operations like HTTP requests, timers, and user events, then ran change detection afterward. With Signals, Angular already knows when state changes and which parts of the UI depend on that state. This allows Angular to update only the affected UI without monitoring every asynchronous task. The result is better performance, a smaller bundle, and more predictable change detection.

### Traditional Angular (with Zone.js)

```
Button Click
      ↓
Zone.js detects the event
      ↓
Angular runs change detection
      ↓
Every affected component is checked
```

Angular automatically knows when something might have changed because `zone.js` patches browser APIs like:

- `setTimeout`
- `Promise`
- HTTP requests
- DOM events

---

### Zoneless Angular

```
Button Click
      ↓
Signal value changes
      ↓
Angular knows exactly what changed
      ↓
Only affected UI updates
```

No `zone.js` is needed.


---

1 bài LeetCode Test

Câu hỏi về Design pattern