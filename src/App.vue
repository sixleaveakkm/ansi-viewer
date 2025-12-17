<script setup lang="ts">
import {Codemirror} from "vue-codemirror";

// @ts-ignore
import {ansi} from "@cookshack/codemirror-ansi";
import {materialDark} from "@fsegurai/codemirror-theme-material-dark";
import { EditorView } from "@codemirror/view";


const codemirrorExtensions = [
  ansi(),
  materialDark,
  EditorView.lineWrapping,
];
</script>

<template>
  <codemirror class="codemirror" :extensions="codemirrorExtensions" autofocus :style="{height: '100vh', fontSize: '16px'}"/>
</template>

<style>
.cm-specialChar {
  display: none;
}
</style>
