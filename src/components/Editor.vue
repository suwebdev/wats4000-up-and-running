<template>
  <div class="editor">
    <textarea :value="input" @input="update"></textarea>
    <div v-html="compiledMarkdown"></div>
  </div>
</template>

<script>
export default {
  name: 'editor',
  data () {
    return {
      input: '# hello world'
    }
  },
  computed: {
    compiledMarkdown: function () {
      return marked(this.input, { sanitize: true })
    }
  },
  methods: {
    update: _.debounce(function (e) {
      this.input = e.target.value
    }, 300)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.editor {
  margin: 0;
  height: 100%;
}

textarea, .editor div {
  display: inline-block;
  width: 49%;
  height: 75vh;
  vertical-align: top;
  box-sizing: border-box;
  padding: 0 20px;
  text-align: left;
}

textarea {
  border: none;
  border-right: 1px solid #ccc;
  resize: none;
  outline: none;
  background-color: #f6f6f6;
  font-size: 14px;
  font-family: 'Monaco', courier, monospace;
  padding: 20px;
}

code {
  color: #f66;
}
</style>
