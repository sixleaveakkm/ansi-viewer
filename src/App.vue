<script setup lang="ts">
import {Codemirror} from "vue-codemirror";

// @ts-ignore
import {ansi} from "@cookshack/codemirror-ansi";
import {oneDark} from "@codemirror/theme-one-dark";

const codemirrorExtensions = [
  ansi(),
  oneDark,
];
</script>

<template>
  <codemirror class="codemirror" :extensions="codemirrorExtensions" autofocus :style="{height: '100vh'}"/>
</template>

<style scoped>
</style>
