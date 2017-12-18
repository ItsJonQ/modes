# Modes 🔲

Modes is a modular design system for CSS.

<img src="https://github.com/ItsJonQ/modes/blob/master/images/logo.png?raw=true" width="300" />

(WIP)

## Modes…

* Draws inspiration from many CSS frameworks and architecture ideologies
* Recognizes that implementation is situational

---

Need to write notes on…

* Naming conventions
* Frameworks
* Integration
* Testing

---

## Naming conventions

* BEM convention
* ITCSS prefixes
* camelCase


### Structure

`prefix-NameOfObject-additionalPropery`


### Prefixes

Below are prefixes for this system. They're composed of the naming conventions from ITCSS, with some additional prefixes.

| Prefix | Example | Description |
| --- | --- | --- |
| `c-` | `c-Card` | Component. Visible pieces of UI. |
| `o-` | `o-Grid` | Object. Invisible pieces of UI. Typically layout-based. |
| `u-` | `u-mrg-auto` | Utility. Used for adjustment. |
| `t-` | `t-black` | Theme. Used for aesthetic styling. |
| `tx-` | `tx-13` | Text. Text styles. |
| `v-` | `v-CardWrapper` | View. Larger scoped chunks of UI. |
| `s-` | `s-HomePage` | Section. Larger scoped chunks of UI. |


* BEM establishes relationships between objects (and children)
* ITCSS prefixes establishes "types"
* camelCase: CaptializeCamelCase for components. Regular camelCase for non-components.


Examples:

Card component
```scss
.c-Card {
  &__block {
    ...
  }
}
```

Page component
```scss
.c-Page {
  ...
}
```

Card component, with a Page
```scss
.c-Page {
  &__Card {
    ...
  }
}
```


Object:
```scss
.o-Grid {
}
```
