<template>
  <div class="app-container">
    <span>用户管理</span>
    <el-button icon="el-icon-question" type="primary" @click.prevent.stop="guide">{{ $t('guide.button') }}</el-button>
  </div>
</template>

<script>

export default {
  name: 'UserManager',
  data() {
    return {
      driver: null
    }
  },
  mounted() {
    // this.driver = new Driver()
  },
  methods: {
    guide() {
      // this.driver.defineSteps(steps)
      this.driver.start()
    }
  }
}
</script>
