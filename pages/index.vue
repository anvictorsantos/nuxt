<template>
  <div>
    <pre>
      {{ $config }}
    </pre>

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
  
  asyncData({ $config }) {
    console.log($config);
  },

  created() {
    console.log(this.$config.facebook_api_key);
    console.log(this.$name('Jon Snow'));
  },

  mounted() {
    console.log(this.$dayjs().format());
  }
}
</script>
