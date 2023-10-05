<script setup>
import { ref , computed} from 'vue'
import store from '../store';

const test = computed(() => store.state.test01)

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
 <h1 class="bg-purple-500" >{{ test }}</h1>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
