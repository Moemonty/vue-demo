<script setup>
import { ref, onMounted } from 'vue'

defineProps({
  msg: {
    type: String,
    required: true
  },
  count: {
    type: Number,
    required: false,
  }
})

const count = ref(0)

function increment() {
  count.value++
}

// lifecycle hooks
onMounted(() => {
  console.log(`Hello Cornell University. The count is: ${count.value}.`)
})

</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      Hello, Cornell University Library Applications Development and Team!
    </h3>
    <button @click="increment">
      Clicks: {{ count }}
    </button>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
