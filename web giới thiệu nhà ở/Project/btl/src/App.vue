<template>
  <div id ="app">
    <div class="topbar">
      <div class="container">
      <div class="topbar-info">
        <span>
          <svg class="svg-inline--fa fa-map-marker-alt fa-w-12" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="map-marker-alt" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512" data-fa-i2svg=""><path fill="currentColor" d="M172.268 501.67C26.97 291.031 0 269.413 0 192 0 85.961 85.961 0 192 0s192 85.961 192 192c0 77.413-26.97 99.031-172.268 309.67-9.535 13.774-29.93 13.773-39.464 0zM192 272c44.183 0 80-35.817 80-80s-35.817-80-80-80-80 35.817-80 80 35.817 80 80 80z"></path></svg>
          <!-- <i class="fas fa-map-marker-alt"></i> Font Awesome fontawesome.com -->
          Tầng 11, tòa nhà Việt Á, số 9 phố Duy Tân, Dịch Vọng Hậu, Cầu Giấy, HN
        </span>
        <span>
          <svg class="svg-inline--fa fa-headphones-alt fa-w-16" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="headphones-alt" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M160 288h-16c-35.35 0-64 28.7-64 64.12v63.76c0 35.41 28.65 64.12 64 64.12h16c17.67 0 32-14.36 32-32.06V320.06c0-17.71-14.33-32.06-32-32.06zm208 0h-16c-17.67 0-32 14.35-32 32.06v127.88c0 17.7 14.33 32.06 32 32.06h16c35.35 0 64-28.71 64-64.12v-63.76c0-35.41-28.65-64.12-64-64.12zM256 32C112.91 32 4.57 151.13 0 288v112c0 8.84 7.16 16 16 16h16c8.84 0 16-7.16 16-16V288c0-114.67 93.33-207.8 208-207.82 114.67.02 208 93.15 208 207.82v112c0 8.84 7.16 16 16 16h16c8.84 0 16-7.16 16-16V288C507.43 151.13 399.09 32 256 32z"></path></svg>
          <!-- <i class="fas fa-headphones-alt"></i> Font Awesome fontawesome.com -->
          0342953***
        </span>
        <form role="search" method="get" class="search-form" action="https://ccboffice.vn/">
				<label class="hc-search">
					<input type="search" class="search-field form-control" placeholder="Search..." value="" name="s" title="Search for:">
					<!-- <input type="hidden" name="post_type" value="office" /> -->
					<button type="submit" class="search-submit"><svg class="svg-inline--fa fa-search fa-w-16" aria-hidden="true" focusable="false" data-prefix="fa" data-icon="search" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M505 442.7L405.3 343c-4.5-4.5-10.6-7-17-7H372c27.6-35.3 44-79.7 44-128C416 93.1 322.9 0 208 0S0 93.1 0 208s93.1 208 208 208c48.3 0 92.7-16.4 128-44v16.3c0 6.4 2.5 12.5 7 17l99.7 99.7c9.4 9.4 24.6 9.4 33.9 0l28.3-28.3c9.4-9.4 9.4-24.6.1-34zM208 336c-70.7 0-128-57.2-128-128 0-70.7 57.2-128 128-128 70.7 0 128 57.2 128 128 0 70.7-57.2 128-128 128z"></path></svg><!-- <i class="fa fa-search" aria-hidden="true"></i> Font Awesome fontawesome.com --></button>
				</label>
			</form>
      <div class="favorites"><svg class="svg-inline--fa fa-heart fa-w-16" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="heart" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M462.3 62.6C407.5 15.9 326 24.3 275.7 76.2L256 96.5l-19.7-20.3C186.1 24.3 104.5 15.9 49.7 62.6c-62.8 53.6-66.1 149.8-9.9 207.9l193.5 199.8c12.5 12.9 32.8 12.9 45.3 0l193.5-199.8c56.3-58.1 53-154.3-9.8-207.9z"></path></svg>
      <!-- <i class="fas fa-heart"></i> Font Awesome fontawesome.com -->
       <a href="/favorite">Favorite: </a>
       <span>0</span>
      </div>
      </div> 
      </div>
    </div>
    <header id="masthead" class="site-header" role="banner">
		<div class="hc-header">
			<div class="container">
				<div class="header-menu-section">
					<div class="site-header-inner">
						<div class="site-branding">
							<div class="site-title">
                  <ul>
                    <img class="img" src="https://ccboffice.vn/wp-content/uploads/2021/07/CCB-logo-2021-goc-e1626080950792.png" alt="CCB">
                    <li><router-link to='/'>Trang chủ</router-link></li>
                    <li><router-link to='/product-page'>Văn phòng cho thuê</router-link></li>
                    <li><router-link to="/news-page">Tin tức </router-link></li>
                    <li><router-link to="/contact-page">Liên hệ</router-link></li>
                 </ul>
							</div>
						</div>
					</div>
						</div>
	
			<!-- End sub menu -->
					</div><!-- .container -->
			</div></header>
            <router-view/>
            <FooterPage/>
  </div>
</template>
<script>
import FooterPage from '@/components/FooterPage.vue'; 

export default {
  components: {
    FooterPage,
  },
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.img {
  margin-right: 75px;
}
.site-title li {
  display: inline-block;
  margin-right: 20px;
}
.site-title {
  background-image:url('');
  background-size: cover;
  background-attachment: fixed;
  background-repeat: no-repeat;
  display: flex;
 justify-content: center;
 align-items: center;


}
.topbar {
    background-color: #880005;
    color: #fff;
    font-size: 16px;
    padding: 7px 0;
}
.container {
    padding-bottom: 0;
    position: relative;
}
.container {
    margin-right: auto;
    margin-left: auto;
    padding-left: 15px;
    padding-right: 15px;
}
.container {
    padding: 0 15px 15px 15px;
}
* {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
}
user agent stylesheet
div {
    display: block;
}
body {
    word-wrap: break-word;
    font-family: 'Roboto';
    font-size: 16px;
}
body {
    font-family: 'Raleway', sans-serif;
    font-size: 14px;
    line-height: 1.428571429;
    color: #333333;
    background-color: #fff;
}
.topbar-info {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
}
.topbar-info span {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
}
svg:not(:root).svg-inline--fa {
    overflow: visible;
}
.svg-inline--fa.fa-w-12 {
    width: 0.75em;
}
.topbar-info span svg {
    background: #e51d2d;
    border-radius: 50%;
    width: 27px!important;
    height: 27px;
    padding: 7px;
    margin-right: 7px;
}
svg:not(:root) {
    overflow: hidden;
}
.svg-inline--fa {
    display: inline-block;
    font-size: inherit;
    height: 1em;
    overflow: visible;
    vertical-align: -0.125em;
}
.topbar-info span+span {
    margin-left: 15px;
}
.search-form {
    margin-left: 60px;
}
form {
    display: block;
    margin-top: 0em;
}
.hc-search {
    position: relative;
    margin: 0;
    display: block;
}

label {
    display: inline-block;
    max-width: 100%;
    margin-bottom: 5px;
    font-weight: bold;
}
label {
    cursor: default;
}
.hc-search input[type="search"] {
    color: #616161;
    font-family: "Roboto";
    font-size: 13px;
    font-style: italic;
    border-radius: 0;
    font-weight: normal;
    height: 26px;
    max-width: 100%;
    width: 190px;
}
input[type="search"] {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
}
input[type="search"] {
    -moz-box-sizing: content-box;
    -webkit-box-sizing: content-box;
    box-sizing: content-box;
}
.form-control {
    display: block;
    width: 100%;
    height: 34px;
    padding: 6px 12px;
    font-size: 14px;
    line-height: 1.428571429;
    color: #555555;
    background-color: #fff;
    background-image: none;
    border: 1px solid #ccc;
    border-radius: 4px;
    -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,0.075);
    box-shadow: inset 0 1px 1px rgba(0,0,0,0.075);
    -webkit-transition: border-color ease-in-out 0.15s,box-shadow ease-in-out 0.15s;
    -o-transition: border-color ease-in-out 0.15s,box-shadow ease-in-out 0.15s;
    transition: border-color ease-in-out 0.15s,box-shadow ease-in-out 0.15s;
}
input, button, select, textarea {
    font-family: inherit;
    font-size: inherit;
    line-height: inherit;
}
input {
    line-height: normal;
}
button, input, optgroup, select, textarea {
    color: inherit;
    font: inherit;
    margin: 0;
}
input[type="search" i] {
    appearance: auto;
    box-sizing: border-box;
    writing-mode: horizontal-tb !important;
    padding-block: 1px;
    padding-inline: 2px;
}
.search-submit {
    position: absolute;
    top: 0;
    right: 0;
    height: 100%;
    border: 0;
    background: transparent;
}

input, button, select, textarea {
    font-family: inherit;
    font-size: inherit;
    line-height: inherit;
}
button, html input[type="button"], input[type="reset"], input[type="submit"] {
    cursor: pointer;
}
button, select {
    text-transform: none;
}
button {
    overflow: visible;
}
button, input, optgroup, select, textarea {
    color: inherit;
    font: inherit;
    margin: 0;
}
.favorites {
    padding-top: 4px;
    padding-left: 54px;
    float: right;
}
.favorites a {
    color: #fff;
}

a, a:hover {
    text-decoration: none;
    -webkit-transition: .3s all;
    -o-transition: .3s all;
    transition: .3s all;
    cursor: pointer;
}
a {
    color: #eb2629;
}
a {
    color: #b75833;
    text-decoration: none;
}
a {
    background-color: transparent;
}
.favorites span {
    display: inline-block;
    color: #ec1b23;
    font-size: 15px;
    font-weight: bold;
    background: #fff;
    border-radius: 5px;
    padding: 1px 6px;
    line-height: 1;
}
.site-header {
    left: 0;
    top: 41px;
    width: 100%;
    background: #efefef;
    padding: 15px 0;
    z-index: 9999999;
}
header {
    display: block;
}
.header-menu-section {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
}
.site-title {
    margin: 0;
}
.site-navigation {
    float: right;
    width: 100%;
    position: absolute;
    padding: 0 15px;
    right: 0;
    top: 13px;
    background: #efefef;
    z-index: 1;
}
.site-navigation {
    width: 70px;
}
.site-navigation {
    float: right;
    width: 80%;
    max-width: 576px;
}
.navbar {
    min-height: auto;
}

.navbar-default {
    background-color: transparent;
    border-color: transparent;
}
.navbar {
    position: relative;
    min-height: 50px;
    margin-bottom: 0;
    border: 0;
}
.navbar-default .navbar-toggle {
  width: 100%;
  padding: 10px 10%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: relative;
  border-color: #ddd;
}
.navbar-toggle {
    position: relative;
    float: right;
    margin-right: 15px;
    padding: 9px 10px;
    margin-top: 8px;
    margin-bottom: 8px;
    background-color: transparent;
    background-image: none;
    border: 1px solid transparent;
    border-radius: 4px;
}
header {
      padding: 15px 0;
      text-align: center;
    }

    nav ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
      display: inline-block;
    }

    nav li {
      display: inline-block;
      margin-right: 20px;
    }
.collapse {
    display: none;
    visibility: hidden;
}
ul, ol {
    margin-top: 0;
    margin-bottom: 10px;
}

ol, ul {
    box-sizing: border-box;
}
ul {
    display: block;
    list-style-type: disc;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    padding-inline-start: 40px;
}
.nav>li {
    position: relative;
    display: block;
}
li {
    display: list-item;
    text-align: -webkit-match-parent;
}
.header-submenu {
    position: absolute;
    background: #FDFFF1;
    -webkit-box-shadow: 0px 5px 7px -3px rgba(92,92,92,.75);
    box-shadow: 0px 5px 7px -3px rgba(92,92,92,.75);
    width: 100%;
    left: 0;
    top: 65px;
    border-top: 8px solid #ED1D25;
    padding: 40px 50px;
    display: none;
    z-index: 1;
}
.row {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    display: -moz-flex;
    display: -ms-flex;
    display: -webkit-flex;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    justify-content: flex-start;
    -webkit-box-pack: start;
    -ms-flex-pack: start;
}

.row {
    margin-left: -15px;
    margin-right: -15px;
}
.header-submenu label {
    color: #333;
    font-size: 16px;
    font-weight: bold;
    text-transform: uppercase;
    margin: 0 0 10px;
}
.header-submenu ul {
    padding: 0 0 0 16px;
    margin: 0;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    display: -moz-flex;
    display: -ms-flex;
    display: -webkit-flex;
    -webkit-flex-wrap: wrap;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    -webkit-justify-content: flex-start;
    justify-content: flex-start;
    -webkit-box-pack: start;
    -ms-flex-pack: start;
}
.header-submenu ul li {
    width: 50%;
    margin: 7px 0;
}
</style>
