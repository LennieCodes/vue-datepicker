<template>
  <div class="dp-container">
    <input type="text" @click="activateDatePicker" />
    <dp-dropdown date-picker-active="datepickerActive"></dp-dropdown>
  </div>
</template>

<script>
import DatePickerDropdown from '@/components/DatePickerDropdown.vue';

export default {
  data() {
    return {
      datepickerActive: false,
    };
  },
  components: {
    'dp-dropdown': DatePickerDropdown,
  },
  methods: {
    activateDatePicker() {
      this.datepickerActive = !this.datepickerActive;
    }
  },
};
</script>

<style lang="scss" scoped>
  .dp-container {
    position: relative;
  }
</style>
