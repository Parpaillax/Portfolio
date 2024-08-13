<template>
  <div>
    <RouterView />
<!--    <index></index>-->
  </div>
</template>
<script>
import Index from "~/pages/index.vue";
import {defineComponent} from "vue";

export default defineComponent({
  components: {Index}
})
</script>