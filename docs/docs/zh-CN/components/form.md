::: demo

<template>
  <lay-input v-model="data"></lay-input>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {

    const data = ref("内容");

    return {
      data
    }
  }
}
</script>

:::

::: demo

<template>
  <lay-input placeholder="请输入密码"></lay-input>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {

    return {

    }
  }
}
</script>

:::

::: demo

<template>
  <lay-textarea placeholder="请输入密码"></lay-textarea>
  <br>
  <lay-textarea placeholder="请输入密码" v-model="data"></lay-textarea>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {

    const data = ref("内容");

    return {
      data
    }
  }
}
</script>

:::

::: demo

<template>
  <lay-switch v-model="active"></lay-switch>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {

    const active = ref(true);

    return {
        active
    }
  }
}
</script>

:::

::: demo

<template>
  <lay-switch v-model="active" disabled></lay-switch>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {

    const active = ref(true);

    return {
        active
    }
  }
}
</script>

:::