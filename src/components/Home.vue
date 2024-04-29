<template>
  <h1>home section</h1>
</template>

<script>
export default {
  unmounted() {
    console.log("unmount")
  },
  activated() {
    console.log("active")
  },
  deactivated() {
    console.log("idle")

  }
}

</script>

