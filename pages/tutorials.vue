<template>
  <!-- <div v-html="/static/index.html">doc page</div> -->
  <div>
    <iframe
      id="serviceFrameSend"
      src="notebook/Sponsor_User_Guide.html"
      display="flex"
      width="100%"
      height="1600"
      frameborder="0"
    ></iframe>
    <!-- <iframe
      id="serviceFrameSend"
      src="https://nbviewer.org/github/xianjian-xie/package/blob/main/Assistor_User_Guide.ipynb"
      display="flex"
      width="100%"
      height="1600"
      frameborder="0"
    ></iframe> -->
    <!-- 调整黄金框大小 -->
    <!-- <div
      style="
        border: 2px solid #d5cc5a;
        overflow: hidden;
        margin: 15px auto;
        max-width: 1575px;
      "
    > -->
    <!-- 网页大小调整 -->
    <!-- <div style="overflow: hidden; margin: 15px auto; max-width: 1575px">
      
      <iframe
        scrolling="no"
        src="https://nbviewer.org/github/xianjian-xie/package/blob/main/Sponsor_User_Guide.ipynb"
        style="
          border: 0px none;
          margin-left: -6px;
          height: 8600px;
          margin-top: -86px;
          width: 1250px;
        "
      >
      </iframe>
    </div> -->
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
