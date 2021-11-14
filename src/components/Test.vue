<template>
  <div id="app">
    <div v-if="error">
      {{ error }}
    </div>
    <div v-else>

      <div v-for="website in websites" :key="website.id">
        {{ website.name }}
        {{ website.id }}
        <div v-if="website.mission_statement">
            {{ website.mission_statement.statement }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  name: 'App',
  data () {
    return {
      websites: [],
      error: null
    }
  },
  async mounted () {
    try {
      const response = await axios.get('http://localhost:1337/websites')
      this.websites = response.data
    } catch (error) {
      this.error = error;
    }
  }
}
</script>