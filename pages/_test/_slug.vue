<template>
  <div>
    <h1>{{ this.sluga }}</h1>
    <p>Path: {{ $route.path }}</p>
  </div>
</template>
<script>
export default {
  asyncData({ params }) {
    console.log(params)
    const sluga = params.sluga
    return { sluga }
  },
}
</script>
