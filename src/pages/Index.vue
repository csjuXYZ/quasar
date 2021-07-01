<template>
  <q-page class="flex flex-center">
    <q-btn @click="$q.notify('My message')" color="primary" label="Show a notification" />
  </q-page>
</template>

<script>
import { defineComponent, ref } from "vue";
export default defineComponent({
  setup() {
    let s = ref(5);
    const inc = () => {
      s.value++;
    };
    return { s, inc };
  },
});
</script>
