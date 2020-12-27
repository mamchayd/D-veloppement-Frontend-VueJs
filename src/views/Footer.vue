<template>
<footer class="footer">
  <div class="content has-text-centered">
   <div class="columns">
  <div class="column">
     <p class="title is-5">Visit Morocco</p>
     <p>
       <span class="icon is-medium is-left">
        <i class="fas fa-phone"></i>
      </span> 06 00 00 00 00</p>
     <p><span class="icon is-medium is-left">
        <i class="fas fa-envelope"></i>
      </span> contact@visit-morocco.com</p>
  </div>
  <div class="column">
    <p class="title is-5">Subscribe to our newsletter</p>
    <div class="control has-icons-left has-icons-right">
      <input class="input is-large" type="email" placeholder="Email">
      <span class="icon is-medium is-left">
        <i class="fas fa-envelope"></i>
      </span>
      <span class="icon is-medium is-right">
        <i class="fas fa-check"></i>
      </span>
    </div>
  </div>
  <div class="column">
    <p class="title is-5">Sitemap</p>
    <nav>
	<ul>
		<li><a href='#profile'>Home</a></li>
		<li><a href='#message'>Best places</a></li>
		<li><a href='#settings'>Destinations</a></li>
		<li ><a href='#message'>Trips</a></li>
		<li><a href='#message'>Blog</a></li>
		<li><a href='#message'>Resources</a></li>
	</ul>
</nav>
  </div>
</div>
  </div>
</footer>
</template>

<script>
export default {
}
</script>

<style>
.footer {
  background-color:#3f3f3f !important ;
}
.footer p {
  color: #fff;
}
.control {
  width: 400px;
  margin: auto;
}
nav ul {
	list-style: none;
	margin: 0;
	padding: 0;
}
nav ul li {
  list-style: none;;
}
nav ul li a {
	display: block;
  padding: 10px 15px;
	color: #fff;
	text-decoration: none;
	-webkit-transition: 0.2s linear;
	-moz-transition: 0.2s linear;
	-ms-transition: 0.2s linear;
	-o-transition: 0.2s linear;
  transition: 0.2s linear;
  text-align: left;
}
nav ul li a:hover {
	background: #f8f8f8;
	color: #515151;
}
nav ul li a .fa {
	width: 16px;
	text-align: center;
	margin-right: 5px;
	float:right;
}
nav ul ul {
	background-color:#ebebeb;
}
nav ul li ul li a {
	background: #f8f8f8;
	border-left: 4px solid transparent;
	padding: 10px 20px;
}
nav ul li ul li a:hover {
	background: #ebebeb;
	border-left: 4px solid #3498db;
}
</style>