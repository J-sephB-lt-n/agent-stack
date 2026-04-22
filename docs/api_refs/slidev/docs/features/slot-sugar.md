---
url: /features/slot-sugar.md
description: |
  A syntax sugar for named slots in layouts.
---

# Slot Sugar for Layouts

Some layouts can provide multiple contributing points using [Vue's named slots](https://vuejs.org/guide/components/slots.html).

For example, in [`two-cols` layout](https://github.com/slidevjs/slidev/blob/main/packages/client/layouts/two-cols.vue), you can have two columns left (`default` slot) and right (`right` slot) side by side.

```md
---
layout: two-cols
---

<template v-slot:default>

# Left

This is shown on the left

</template>
<template v-slot:right>

# Right

This is shown on the right

</template>
```

We also provide a shorthand syntactical sugar `::name::` for slot name. The following works exactly the same as the previous example.

```md
---
layout: two-cols
---

# Left

This is shown on the left

::right::

# Right

This is shown on the right
```

You can also explicitly specify the default slot and provide it in the custom order.

```md
---
layout: two-cols
---

::right::

# Right

This shows on the right

::default::

# Left

This is shown on the left
```

---

