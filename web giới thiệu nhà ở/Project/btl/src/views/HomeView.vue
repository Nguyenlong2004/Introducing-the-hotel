<template>
  <div class="app">
      <img src="@/assets/anh 1.png" width="auto" height="400px" >
      <div class="container">
          <h2 class="section-title center">
            Thuê Văn Phòng Hà Nội - 
            <strong>Theo Tòa</strong>
          </h2>
          <div class="section-description center">
            Cung cấp hơn
            <b>500+</b>
            tòa nhà văn phòng mới. Chúng tôi sẽ giúp Bạn nhanh chóng thuê được văn phòng phù hợp, với giá và các điều kiện thuê tốt nhất.
          </div>
          <div class="header-filter">
            <form action="https://ccboffice.vn/office/" method="GET" class="affix">
					<!-- <div class="loading"><div class="loader"></div></div> -->
						<div class="filter-field">
							<select name="district">
								<option class="hc-select" value="">Quận</option>
																	<option district-id="187" class="hc-select" value="quan-ba-dinh">Quận Ba Đình</option>
																	<option district-id="204" class="hc-select" value="van-phong-cho-thue-quan-bac-tu-liem">Quận Bắc Từ Liêm</option>
																	<option district-id="203" class="hc-select" value="van-phong-cho-thue-quan-cau-giay">Quận Cầu Giấy</option>
																	<option district-id="194" class="hc-select" value="van-phong-quan-dong-da">Quận Đống Đa</option>
																	<option district-id="207" class="hc-select" value="van-phong-cho-thue-quan-ha-dong">Quận Hà Đông</option>
																	<option district-id="193" class="hc-select" value="van-phong-quan-hai-ba-trung">Quận Hai Bà Trưng</option>
																	<option district-id="206" class="hc-select" value="van-phong-cho-thue-quan-hoan-kiem">Quận Hoàn Kiếm</option>
																	<option district-id="381" class="hc-select" value="van-phong-quan-hoang-mai">Quận Hoàng Mai</option>
																	<option district-id="387" class="hc-select" value="van-phong-quan-long-bien">Quận Long Biên</option>
																	<option district-id="195" class="hc-select" value="van-phong-quan-nam-tu-liem">Quận Nam Từ Liêm</option>
																	<option district-id="205" class="hc-select" value="van-phong-quan-tay-ho">Quận Tây Hồ</option>
																	<option district-id="202" class="hc-select" value="van-phong-cho-thue-quan-thanh-xuan">Quận Thanh Xuân</option>
															</select>
							<div class="neighborhood-select">
								<select name="neighborhood"><option class="hc-select" value="">Đường</option></select>
							</div>
						</div>
						<div class="filter-field">
							<div class="min-max">
																<input type="number" min="0" id="price-min" placeholder="Giá từ" value="">
								<input type="number" min="1" id="price-max" placeholder="Đến" value="">
							</div>
							<input type="text" id="amount" name="price" value="" readonly="" style="display:none">
							<!-- <div class="price-range"><span class="range"></span> <span class="ranNumber">$10 - $500</span></div>
							<input type="text" id="amount" name='price' readonly style="display:none">
							<div id="slider-range"></div>					 -->
							<select name="office-class">
								<option class="hc-select" value="">Hạng</option>
																									<option class="hc-select" value="van-phong-hang-a">Hạng A</option>
																	<option class="hc-select" value="van-phong-hang-b">Hạng B</option>
																	<option class="hc-select" value="van-phong-hang-c">Hạng C</option>
																	<option class="hc-select" value="van-phong-hang-d">Hạng D</option>
															</select>
						</div>
						
						
						<div class="filter-field">
							<input type="text" name="keyword" placeholder="Tìm theo tòa nhà" value="">
							<button type="submit" name="submit-filter">Tìm kiếm <svg class="svg-inline--fa fa-search fa-w-16" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="search" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M505 442.7L405.3 343c-4.5-4.5-10.6-7-17-7H372c27.6-35.3 44-79.7 44-128C416 93.1 322.9 0 208 0S0 93.1 0 208s93.1 208 208 208c48.3 0 92.7-16.4 128-44v16.3c0 6.4 2.5 12.5 7 17l99.7 99.7c9.4 9.4 24.6 9.4 33.9 0l28.3-28.3c9.4-9.4 9.4-24.6.1-34zM208 336c-70.7 0-128-57.2-128-128 0-70.7 57.2-128 128-128 70.7 0 128 57.2 128 128 0 70.7-57.2 128-128 128z"></path></svg><!-- <i class="fas fa-search"></i> Font Awesome fontawesome.com --></button>
						</div>
				</form>
          </div>
      </div>
      <section class="office-description">
		<div class="office-section-title">Thông tin chung</div>
		<div class="item-list row">
				<div class="col-sm-6">
		<div class="itemlistitem">
			<div class="row">
				<div class="col-sm-6"><label for="">Vị trí</label></div>
				<div class="col-sm-6">Số 85 Lê Văn Lương, Thanh Xuân, Hà Nội</div>
			</div>
		</div>
		</div>
				<div class="col-sm-6">
		<div class="itemlistitem">
			<div class="row">
				<div class="col-sm-6"><label for="">Chiều cao tầng</label></div>
				<div class="col-sm-6">Gồm 02 tòa nhà cao 28 tầng và 31 tầng</div>
			</div>
		</div>
		</div>
				<div class="col-sm-6">
		<div class="itemlistitem">
			<div class="row">
				<div class="col-sm-6"><label for="">Chiều cao trần</label></div>
				<div class="col-sm-6">2.7m</div>
			</div>
		</div>
		</div>
				<div class="col-sm-6">
		<div class="itemlistitem">
			<div class="row">
				<div class="col-sm-6"><label for="">Diện tích sàn</label></div>
				<div class="col-sm-6">~1000m2</div>
			</div>
		</div>
		</div>
				<div class="col-sm-6">
		<div class="itemlistitem">
			<div class="row">
				<div class="col-sm-6"><label for="">Thang máy</label></div>
				<div class="col-sm-6">Hệ thống thang máy tốc độ cao</div>
			</div>
		</div>
		</div>
				<div class="col-sm-6">
		<div class="itemlistitem">
			<div class="row">
				<div class="col-sm-6"><label for="">Điều hòa</label></div>
				<div class="col-sm-6">Đang cập nhật</div>
			</div>
		</div>
		</div>
				<div class="col-sm-6">
		<div class="itemlistitem">
			<div class="row">
				<div class="col-sm-6"><label for="">Điện dự phòng</label></div>
				<div class="col-sm-6">Đang cập nhật</div>
			</div>
		</div>
		</div>
				<div class="col-sm-6">
		<div class="itemlistitem">
			<div class="row">
				<div class="col-sm-6"><label for="">Giờ làm việc</label></div>
				<div class="col-sm-6">Từ thứ 2 đến thứ 6: 07h30 - 18h00, thứ 7: 07h30 - 13h00</div>
			</div>
		</div>
		</div>
		</div>
	</section>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.app {
  margin: 20px;
  padding: 0px;
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
.section-title {
    font-weight: 400;
    margin: 0 0 30px;
    font-size: 40px;
    color: #848484;
}

.center {
    text-align: center;
}
h2, .h2 {
    font-size: 30px;
}
h1, .h1, h2, .h2, h3, .h3 {
    margin-top: 20px;
    margin-bottom: 10px;
}
h1, h2, h3, h4, h5, h6, .h1, .h2, .h3, .h4, .h5, .h6 {
    font-family: inherit;
    font-weight: 500;
    line-height: 1.1;
    color: inherit;
}
user agent stylesheet
h2 {
    display: block;
    font-size: 1.5em;
    margin-block-start: 0.83em;
    margin-block-end: 0.83em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    font-weight: bold;
}

.section-description {
    max-width: 700px;
    margin: auto;
}
strong {
    color:#ec1d25;
    font-family:'Times New Roman', Times, serif;
}
.header-filter {
    position: relative;
    margin-top: 35px;
    height: 176px;
    margin-bottom: 120px;
}
.header-filter form.affix {
    left: 0;
    right: 0;
    top: 0;
    z-index: 222;
    padding: 5px 20%;
}
.filter-field {
    padding: 0 15px;
}
.filter-field select, .filter-field input {
    border: 1px solid #cacaca;
    background: #fff;
    color: #333;
    font-size: 16px;
    width: 100%;
    padding: 6px 10px;
    margin: 7px 0;
}

input, button, select, textarea {
    font-family: inherit;
    font-size: inherit;
    line-height: inherit;
}
button, select {
    text-transform: none;
}
button, input, optgroup, select, textarea {
    color: inherit;
    font: inherit;
    margin: 0;
}
option {
    font-weight: normal;
    display: block;
    min-height: 1.2em;
    padding: 0px 2px 1px;
}
.col-sm-6 {
  text-align: center;
}
.office-section-title {
    color: #333;
    font-size: 17px;
    font-weight: bold;
    border-left: 3px solid #ec1d25;
    line-height: 1;
    padding-left: 10px;
    margin-top: 40px;
}
 .image , .item-list row{
   display: inline-block;
   width: 100%;
   box-sizing: border-box;
   vertical-align: top; 
   margin-left: 400px;
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
.office-description {
    color: #333;
    font-size: 16px;
    position: relative;
    min-height: 1px;
    padding-left: 15px;
    padding-right: 15px;
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
.itemlistitem {
    margin: 5px 0;
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
.office-description {
    margin-bottom: 20px;
}

.itemlistitem {
    margin-bottom: 10px;
}

.row {
    margin-bottom: 5px;
}

.col-sm-6 {
    width: 50%;
    float: left;
    box-sizing: border-box;
}

.label {
    font-weight: bold;
}

/* Để tạo đường viền giữa các cột */
.col-sm-6:nth-child(even) {
    clear: both;
}

/* Để tạo khoảng cách giữa các cột */
.col-sm-6:nth-child(odd) {
    margin-right: 10px;
}

</style>
