<template>
  <div class="hello">
    <h1>"Welcome to Kuehar's page!!"</h1>
    <h2>Links</h2>
    <ul class="nav">
      <li>
        <a href="https://github.com/Kuehar"><ion-icon name="logo-github" class="ion-social-github"></ion-icon></a>
      </li>
      <li>
          <a href="https://www.linkedin.com/in/uehara-ken-aa89b7152"><ion-icon name="logo-linkedin" class="ion-social-linkedin"></ion-icon></a>
      </li>
      <li>
        <a href="https://twitter.com/KueharX"><ion-icon name="logo-twitter" class="ion-social-twitter"></ion-icon></a>
      </li>
      <li>
        <a href="https://qiita.com/KueharX"><ion-icon name="reader-outline" class="ion-social-qiita"></ion-icon></a>
      </li>
      <br>
    </ul>
    <h2>This page was made using </h2>
    <h2 class = "vue">Vue.js<a href="#"><ion-icon name="logo-vue" class="ion-social-vue"></ion-icon></a></h2>
    <h2>and</h2>
    <h2 class="azure">Microsoft Azure
      <a href="#"><ion-icon name="logo-windows" class="ion-social-windows"></ion-icon></a></h2>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

h1, h2 {
  font-weight: normal;
  }

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: rgb(8, 8, 8);
}
.vue{
  transition:3.0s;
  color:#0A6F30;
}
.azure{
  color:#00008B;
}

.ion-social-github,
.ion-social-vue,
.ion-social-linkedin,
.ion-social-qiita,
.ion-social-twitter,
.ion-social-windows{
  transition:color 0.2s;
  color:#888;
}

.ion-social-github:hover{
  color:#020303;
}

.ion-social-vue:hover{
  color:#0A6F30;
}

.ion-social-linkedin:hover{
  color:#00008B;
}

.ion-social-qiita:hover{
  color:#0A6F30;
}

.ion-social-twitter:hover{
  color:#55acee;
}

.ion-social-windows:hover{
  color:#00008B;
}

.social-links{
  list-style: none;
  float: right;
}

.nav li a:link,
.nav li a:visited,
.li a:link,
.li a:visited{
  text-decoration: none;
  border:0;
  color:#888;
  transition: 0.2s;
}

.li a:link,
.li a:visited{
  font-size:160%;
}

.page-container {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
}
</style>
