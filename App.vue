<template>
  <view class="container">
    <web-view :source="{uri:'https://www.google.com/'}" 
      :style="{marginTop: 20}" 
      :originWhitelist="['*']"
      javaScriptEnabled
      domStorageEnabled
      allowFileAccessFromFileURLs
      startInLoadingState
      mixedContentMode="compatibility"
      />
  </view>
</template>

<style>
.container {
  background-color: #fff;
  flex: 1;
}
.text-color-primary {
  color: blue;
}
</style>

<script>
import { WebView } from "react-native-webview";

export default {
  components: {
    "web-view": WebView
  }
}
</script>
