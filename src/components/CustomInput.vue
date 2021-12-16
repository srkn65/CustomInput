
// CustomInput.vue
<template>
    <!-- $listeners -->
    <!-- <input v-on="$listeners" /> -->
    <!-- v-model -->
    <input @input="$emit('input', $event.target.value)" />
</template>
<script>
export default {
    name: 'CustomInput'
}
</script>



