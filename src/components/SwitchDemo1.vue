<demo>基础用法</demo>
<desc>按钮的基础用法</desc>

<template>
  <Switch v-model:value="bool" />
</template>

<script lang="ts">
import { ref } from 'vue';

import Switch from '../lib/Switch.vue';
// 使用时改为以下引入
// import { Switch } from '@xmxshr/mui-vue';

export default {
  components: {
    Switch,
  },
  setup() {
    // 设置初始值
    const bool = ref(false);
    return {
      bool,
    };
  },
};
</script>