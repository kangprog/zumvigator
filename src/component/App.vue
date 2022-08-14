<template>
  <input type="text" v-model="input" placeholder="Search..."/>
</template>

<script setup>
  import { ref } from "vue";
  let input = ref("");
</script>

<style src="../style/custom_style.css" />
