<script setup lang="ts">
import { EditorContent, useEditor } from "@tiptap/vue-3";
import StarterKit from "@tiptap/starter-kit";

const editor = useEditor({
  content: "<p>Content here</p>",
  extensions: [StarterKit],
});
</script>

<template>
  <div v-if="editor">
    <EditorContent :editor="editor" />
  </div>
</template>
