<template>
  <header>
    {{ msg }}
  </header>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    msg: String
  }
}
</script>