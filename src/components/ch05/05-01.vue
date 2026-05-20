<template>
  <div>
    <h1>App.vue</h1>
    <p>Count: {{ counter }}</p>
    <p>Double Count: {{ doubleCount }}</p>
    <p>Double Plus One: {{ doublePlusOne }}</p>
    <button @click="increment">Increment</button>
    <button @click="randomizeCounter">Randomize</button>
  </div>
</template>

<script>
import { useStore } from "../../store/index.ts";
export default {
  data() {
    return {
      counter: useStore(),
    };
  },
  computed:{
    doubleCount(){
        return this.counter.doubleCount
    },
    doublePlusOne(){
        return this.counter.doublePlusOne
    }
  },
  methods:{
    increment(){
        this.counter.increment();
    },
    randomizeCounter(){
        this.counter.randomizeCounter();
    }
  }
};
</script>
