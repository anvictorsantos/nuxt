<template>
  <div>
    <VTooltip>
      <a>Sponsor me</a>

      <template #popper>
        Help me fund
      </template>
    </VTooltip>

    <pre>
      {{ $store.state.user }}
    </pre>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  created() {
    console.log(this.$name('Jon Snow'));
  },
  mounted() {
    console.log(this.$dayjs().format());
  }
}
</script>
