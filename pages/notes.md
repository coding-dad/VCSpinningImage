---
title: Hinweise
layout: page
---

Zur Lösung der Aufgabe werden idealerweise folgende Komponenten verwendet

-   [Computed Properties](https://vuejs.org/v2/guide/computed.html#Computed-Properties)
-   [Data & Methods](https://vuejs.org/v2/guide/instance.html#Data-and-Methods)
-   [Event handling](https://vuejs.org/v2/guide/events.html#Listening-to-Events)

## Tipps

Du kanns innerhalb einer Vue Komponente innerhalb von `<script></script>` das Datenobjekt auch folgerndermaßen definieren:

```js
<script>
export default {
	// ...

	data: () => ({
		myName: "Bond, James"
	}),

	// ...
}
</script>
```

## Einordnung der Challenge

Schwierigkeitsgrad
: ==leicht==

Themen
: ==# methods==, ==# computed properties==, ==# event handling==
