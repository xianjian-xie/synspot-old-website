<template>
  <!-- <div v-html="/static/index.html">doc page</div> -->
  <div>
    <iframe
      id="serviceFrameSend"
      src="html/index.html"
      display="flex"
      width="100%"
      height="1600"
      frameborder="0"
    ></iframe>
  </div>
</template>

<script>
// import ht from '../static/index.html'
// import 'github-markdown-css/github-markdown.css'
// import 'highlight.js/styles/github.css'

// export default {
//   async asyncData({ params }) {
//     const { default: articleHtml } = await import(
//       `@/assets/md/${params.article}.md`
//     )
//     return { articleHtml }
//   },
//   data() {
//     return {
//       articleHtml: '',
//     }
//   },
// }
// export default {
//   data() {
//     return {
//       docsurl: 'https://en.wikipedia.org/wiki/Main_Page',
//     }
//   },
// }
</script>
