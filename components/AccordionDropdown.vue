<template>
  <div class="accordion">
    <div v-for="(item, index) in items" :key="index" class="accordion-item">
      <div class="accordion-header" @click="toggle(index)">
        <h3>{{ item.title }}</h3>
        <span v-if="activeIndex == index"><img src="/assets/arrow-left.png" alt=""></span>
        <span v-else><img src="/assets/arrow-left.png" alt=""></span>
      </div>
      <transition name="fade">
        <div v-show="activeIndex == index" class="accordion-body">
          <p>{{ item.content }}</p>
        </div>
      </transition>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    items: {
      type: Array,
      required: true,
      default: () => [],
    },
  },
  data() {
    return {
      activeIndex: null,
    }
  },
  methods: {
    toggle(index) {
      this.activeIndex = this.activeIndex === index ? null : index
    },
  },
}
</script>

<style scoped>
.accordion {
  /* border: 1px solid #ccc; */
  border-radius: 5px;
}

/* .accordion-item {
  border-bottom: 1px solid #ccc;
} */

.accordion-header {
  padding: 28px;
    cursor: pointer;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
}

.accordion-header h3 {
  margin: 0;
}

.accordion-body {
  padding: 10px;
  background-color: #fff;
  display: none;
}

.accordion-body p {
  margin: 0;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}
</style>
