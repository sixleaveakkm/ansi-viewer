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
  <codemirror :extensions="codemirrorExtensions" autofocus/>
</template>

<style scoped></style>
