<template>
    <div class="dp-dropdown" v-if="datepickerActive">
      <div class="dp-dropdown-header">
        <button class="prev-btn" @click="prevMonth">prev</button>
        <span>March</span>
        <button class="next-btn" @click="nextMonth">next</button>
      </div>
      <div class="dp-dropdown-body">
        <button @click="selectDate">Click me</button>
      </div>
    </div>
</template>

<script>
/*
  What now? Need to setup date somehow? 

  < month >
*/
export default {
  props: {
    datepickerActive: boolean,
  },
  methods: {
    prevMonth() {

    },
    nextMonth() {

    },
    selectDate() {
        
    },
  },
}
</script>

<style lang="scss" scoped>
  .dp-dropdown {
    position: absolute;
    max-width: 400px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    .dp-dropdown-header {
      border-bottom: 1px grey solid;
      .prev-btn {
        float: left;
      }
      .next-btn {
        float: right;
      }
    }
  }
</style>