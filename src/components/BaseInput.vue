<template>
<div>
  <p>Base Input</p>
  <input type="text" :value="modelValue.value" @input="writeValue($event.target.value)" />
</div>

</template>
<script setup>
const emit = defineEmits(['update:modelValue', 'value-change'])
defineProps({
  modelValue: {
    type: Object,
    default: ""
  }
})
function writeValue(val) {
  emit('update:modelValue', {
    value: val,
    code: 12
  })
}
</script>