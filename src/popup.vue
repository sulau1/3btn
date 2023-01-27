<template>
  <div class="popup">
    <div class="popup_head">
      <span>PopupName</span>
      <span class="close_button">&#10008;</span>
    </div>
    <div class="popup_content">
      <slot></slot>
    </div>
    <div class="popup_bottom">
      <button></button>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: "popup",
  props: {},
  data() {
    return {
      IsPopUpVisible: false,
    };
  },
  methods: {
    ShowPopup() {
      this.IsPopUpVisible = true;
    },
  },
};
</script>

<style></style>
