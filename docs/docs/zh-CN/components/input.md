::: demo

<template>
  <lay-input v-model="data1"></lay-input>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {

    const data1 = ref("内容");

    return {
      data1
    }
  }
}
</script>

:::

::: demo

<template>
  <lay-input placeholder="提示信息"></lay-input>
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
  <lay-input v-model="data2" @input="input"></lay-input>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {

    const data2 = ref("Input 事件");
    const input = function( val ) {
        console.log("当前值:" + val)
    }

    return {
      data2,
      input
    }
  }
}
</script>

:::


::: demo

<template>
  <lay-input placeholder="禁止输入" :disabled="disabled"></lay-input>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {

    const disabled = ref(true)

    return {
        disabled
    }
  }
}
</script>

:::


| Name   | Description | Accepted Values  |
| -------- | ---- | ----------------------- | 
| name       | 原始属性 name | --  | 
| placeholder      | 提示信息 | --   | 
| disabled      | 禁用 | `true` `false`   |
| v-model     | 值 | --  | 
| input   | 原生 input 事件 | val : 当前值  | 