// Form.vue
<template>
<form>
  <p style="color: green">
    {{ model }}
  </p>
     <!-- $listeners -->

    <!-- <custom-input @input="model = $event.target.value"/> -->

     <!-- v-model -->
    <custom-input v-model="model"/>
</form>
</template>

<script>
import CustomInput from './CustomInput.vue'
export default {
  components: { CustomInput },
  name: 'Form',
  data() {
    return {
      model: ''
    }
  }
}
</script>