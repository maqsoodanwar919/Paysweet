<template>
	<div class="body_wrap">
	  <div class="dashboard_body mh-100">
		<div class="title_header d-flex mb_50 justify-content-between align-items-center">
		  <h1 class="text-left title">Edit <span class="lit_font">Calexico</span>
		  </h1>
		  <div class="btn_wrap d-flex">
			<button type="button" class="btn theme-btn2 w185 mr_10">
			  <span>New Coverage</span>
			</button>
			<button type="button" class="btn theme-red">Delete</button>
		  </div>
		</div>
		<form action="">
		  <fieldset class="fieldset">
			<div class="fieldset_title">
			  <h6>Restaurant Status</h6>
			</div>
			<div class="form-group mb_25">
			  <label class="mb_6 f14">Status</label>
			  <select class="form-control custom_select">
				<option>Active</option>
			  </select>
			</div>
			<div class="checkbox_wrap form-group">
			  <input type="checkbox" name="New-in-town" id="New_in_town" class="">
			  <label for="New_in_town" class="f14">New in town <span class="text_lt">(a ‘NEW’ sticker will be added to the restaurant & will disappear after 6 months)</span>
			  </label>
			</div>
		  </fieldset>
		  <fieldset class="fieldset">
			<div class="fieldset_title">
			  <h6>Cuisines & Occassions</h6>
			</div>
			<div class="form-group mb_25 custom_multiselect lt_bg ">
			  <label class="mb_6 f14">Cuisines</label>
			  <Multiselect :class="{'custom_select': true, 'form-control':true } " v-model="value" mode="tags" placeholder="Select Cuisines" :options="Cuisines" />
			</div>
			<div class="form-group mb_25 custom_multiselect lt_bg ">
			  <label class="mb_6 f14">Occassions</label>
			  <Multiselect :class="{'custom_select': true, 'form-control':true } " v-model="value" mode="tags" placeholder="Select Occassions" :options="Occassions" />
			</div>
		  </fieldset>
		  <fieldset class="fieldset tabs_fieldset p20_30 overflow">
			<nav>
			  <div class="nav nav-tabs" id="nav-tab" role="tablist">
				<button class="nav-link active" id="nav-english-tab" data-bs-toggle="tab" data-bs-target="#nav-english" type="button" role="tab" aria-controls="nav-english" aria-selected="true">English</button>
				<button class="nav-link" id="nav-arabic-tab" data-bs-toggle="tab" data-bs-target="#nav-arabic" type="button" role="tab" aria-controls="nav-arabic" aria-selected="false">arabic</button>
			  </div>
			</nav>
			<div class="tab-content mt_55" id="nav-tabContent">
			  <div class="tab-pane fade show active" id="nav-english" role="tabpanel" aria-labelledby="nav-english-tab">
				<fieldset class="fieldset p30_20 mb-0">
				  <div class="fieldset_title bg-white">
					<h6>Main Information</h6>
				  </div>
				  <div class="form-group mb_25">
					<label class="mb_6 f14">Name*</label>
					<input type="text" class="form-control" placeholder="Enter name" />
				  </div>
				  <div class="form-group mb_25">
					<label class="mb_6 f14">Average Prices (BHD)*</label>
					<input type="text" class="form-control" placeholder="Enter name" />
				  </div>
				  <div class="form-group mb_25">
					<label class="mb_6 f14">Additional Prices Text (optional)</label>
					<input type="text" class="form-control" placeholder="e.g. Inclusive of VAT and service charges if there’s any" />
				  </div>
				  <div class="form-group mb_25">
					<label class="mb_6 f14">Instagram Handle (optional)</label>
					<input type="text" class="form-control" placeholder="e.g. Inclusive of VAT and service charges if there’s any" />
				  </div>
				  <div class="form-group mb_25">
					<label class="mb_6 f14">Phone Number (optional)</label>
					<div class="d-flex">
					  <select class="form-control custom_select w130 mr_10">
						<option>+973</option>
					  </select>
					  <input type="text" class="form-control" placeholder="e.g. Inclusive of VAT and service charges if there’s any" />
					</div>
				  </div>
				  <div class="form-group mb_25">
					<label class="mb_6 f14">About the restuarant*</label>
					<textarea class="form-control h80" placeholder="Description of the restaurant"></textarea>
				  </div>
				  <div class="form-group mb_25">
					<label class="mb_6 f14">Meat & Poultry Sources</label>
					<input type="text" class="form-control" placeholder="enter where the meat & chicken is from" />
				  </div>
				</fieldset>
			  </div>
			  <div class="tab-pane fade" id="nav-arabic" role="tabpanel" aria-labelledby="nav-arabic-tab">arabic</div>
			</div>
		  </fieldset>
		  <fieldset class="fieldset p20_30">
			<div class="fieldset_title">
			  <h6>Location & Food Trucks</h6>
			</div>
			<div class="tabs_fieldset  mt_60 p30_20">
			  <div class="fieldset_title">
				<h6>Location/Branch</h6>
			  </div>
			  <div class="add_branch_wraper">
				<div class="row pt-2">
				  <div class="col-3">
					<div class="form-group mb_25">
					  <label class="mb_6 f14">Location/Branch Name </label>
					  <input type="text" class="form-control" placeholder="Enter Branch Name" />
					</div>
				  </div>
				  <div class="col-9">
					<div class="form-group mb_25">
					  <label class="mb_6 f14">Location URL*</label>
					  <input type="text" class="form-control" placeholder="Enter google maps link here" />
					</div>
				  </div>
				</div>
			  </div>
			  <div class="btn_wrap d-flex">
				<button type="button" class="btn theme-btn2 w185 add_btn">
				  <span>
					<Cross class="mr_10" />Add Branch
				  </span>
				</button>
			  </div>
			</div>
			<div class="tabs_fieldset  mt_50 p30_20">
			  <div class="fieldset_title">
				<h6>Food Trucks</h6>
			  </div>
			  <div class="add_Food_wraper pt-2">
				<div class="row">
				  <div class="col-3">
					<div class="form-group mb_25">
					  <label class="mb_6 f14">Location Name </label>
					  <input type="text" class="form-control" placeholder="Enter Branch Name" />
					</div>
				  </div>
				  <div class="col-9">
					<div class="form-group mb_25">
					  <label class="mb_6 f14">Location URL</label>
					  <input type="text" class="form-control" placeholder="Enter google maps link here" />
					</div>
				  </div>
				  <div class="col-3">
					<div class="form-group mb_25">
					  <label class="mb_6 f14">Location Name </label>
					  <input type="text" class="form-control" placeholder="Enter Branch Name" />
					</div>
				  </div>
				  <div class="col-9">
					<div class="form-group mb_25">
					  <label class="mb_6 f14">Location URL</label>
					  <input type="text" class="form-control" placeholder="Enter google maps link here" />
					</div>
				  </div>
				</div>
			  </div>
			  <div class="btn_wrap d-flex">
				<button type="button" class="btn theme-btn2 w210 add_btn">
				  <span>
					<Cross class="mr_10" />Add Food Truck
				  </span>
				</button>
			  </div>
			</div>
		  </fieldset>
		  <fieldset class="fieldset p20_30">
			<div class="fieldset_title">
			  <h6>Timing, Amenities, & Delivery</h6>
			</div>
			<div class="tabs_fieldset  mt_60 p30_20">
			  <div class="fieldset_title bg-white">
				<h6>Timing</h6>
			  </div>
			  <div class="timing_wrap mb_20 ml-15">
				<div class="form-group">
				  <div class="checkbox_wrap">
					<input type="checkbox" name="days" id="Sunday" class="">
					<label for="Sunday" class="f14">Sunday</label>
				  </div>
				</div>
				<div class="hour_mintus_wrap">
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				  <div class="hour_to f14">to</div>
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				</div>
			  </div>
			  <div class="timing_wrap mb_20 ml-15">
				<div class="form-group">
				  <div class="checkbox_wrap">
					<input type="checkbox" name="days" id="Monday" class="">
					<label for="Monday" class="f14">Monday</label>
				  </div>
				</div>
				<div class="hour_mintus_wrap">
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				  <div class="hour_to f14">to</div>
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				</div>
			  </div>
			  <div class="timing_wrap mb_20 ml-15">
				<div class="form-group">
				  <div class="checkbox_wrap">
					<input type="checkbox" name="days" id="Tuesday" class="">
					<label for="Tuesday" class="f14">Tuesday</label>
				  </div>
				</div>
				<div class="hour_mintus_wrap">
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				  <div class="hour_to f14">to</div>
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				</div>
			  </div>
			  <div class="timing_wrap mb_20 ml-15">
				<div class="form-group">
				  <div class="checkbox_wrap">
					<input type="checkbox" name="days" id="Wednesday" class="">
					<label for="Wednesday" class="f14">Wednesday</label>
				  </div>
				</div>
				<div class="hour_mintus_wrap">
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				  <div class="hour_to f14">to</div>
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				</div>
			  </div>
			  <div class="timing_wrap mb_20 ml-15">
				<div class="form-group">
				  <div class="checkbox_wrap">
					<input type="checkbox" name="days" id="Thursday" class="">
					<label for="Thursday" class="f14">Thursday</label>
				  </div>
				</div>
				<div class="hour_mintus_wrap">
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				  <div class="hour_to f14">to</div>
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				</div>
			  </div>
			  <div class="timing_wrap mb_20 ml-15">
				<div class="form-group">
				  <div class="checkbox_wrap">
					<input type="checkbox" name="days" id="Friday" class="">
					<label for="Friday" class="f14">Friday</label>
				  </div>
				</div>
				<div class="hour_mintus_wrap">
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				  <div class="hour_to f14">to</div>
				  <div class="form-group AccessTime_wrap">
					<input type="time" class="form-control tw_187" name="days" id="" placeholder="HH:MM">
				  </div>
				</div>
			  </div>
			</div>
			<div class="tabs_fieldset  mt_40 p30_20">
			  <div class="fieldset_title bg-white Amenities_wraper">
				<h6>Amenities</h6>
			  </div>
			  <div class="row  pt-2 pl-15">
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Free_Wifi" class="">
					  <label for="Free_Wifi" class="f14">Free Wifi</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Indoor_Seating" class="">
					  <label for="Indoor_Seating" class="f14">Indoor Seating</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Complimentary_Food" class="">
					  <label for="Complimentary_Food" class="f14">Complimentary Food</label>
					</div>
				  </div>
				</div>
			  </div>
			  <div class="row  pt-2 pl-15">
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Reservations" class="">
					  <label for="Reservations" class="f14">Reservations</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Disabled_Parking" class="">
					  <label for="Disabled_Parking" class="f14">Disabled Parking</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Bottomless_Drinks" class="">
					  <label for="Bottomless_Drinks" class="f14">Bottomless Drinks</label>
					</div>
				  </div>
				</div>
			  </div>
			  <div class="row  pt-2 pl-15">
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Parking_Available" class="">
					  <label for="Parking_Available" class="f14">Parking Available</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Smoking_Area" class="">
					  <label for="Smoking_Area" class="f14">Smoking Area</label>
					</div>
				  </div>
				</div>
			  </div>
			  <div class="row  pt-2 pl-15">
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Outdoor_Seating" class="">
					  <label for="Outdoor_Seating" class="f14">Outdoor Seating</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Delivery" class="">
					  <label for="Delivery" class="f14">Delivery</label>
					</div>
				  </div>
				</div>
			  </div>
			</div>
			<div class="tabs_fieldset  mt_40 p30_20">
			  <div class="fieldset_title bg-white Amenities_wraper">
				<h6>Delivery Options</h6>
			  </div>
			  <div class="row  pt-2 pl-15">
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Talabat" class="">
					  <label for="Talabat" class="f14">Talabat</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Careem_Now" class="">
					  <label for="Careem_Now" class="f14">Careem Now</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Uber_Eats" class="">
					  <label for="Uber_Eats" class="f14">Uber Eats</label>
					</div>
				  </div>
				</div>
			  </div>
			  <div class="row  pt-2 pl-15">
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="You_Delivery" class="">
					  <label for="You_Delivery" class="f14">YOU Delivery</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Ahlan" class="">
					  <label for="Ahlan" class="f14">Ahlan</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Zomato" class="">
					  <label for="Zomato" class="f14">Zomato</label>
					</div>
				  </div>
				</div>
			  </div>
			  <div class="row  pt-2 pl-15">
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Jahez" class="">
					  <label for="Jahez" class="f14">Jahez</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Deliveroo" class="">
					  <label for="Deliveroo" class="f14">Deliveroo</label>
					</div>
				  </div>
				</div>
				<div class="col-md-3">
				  <div class="form-group">
					<div class="checkbox_wrap">
					  <input type="checkbox" name="Amenities" id="Hunger Station" class="">
					  <label for="Hunger Station" class="f14">Hunger Station</label>
					</div>
				  </div>
				</div>
			  </div>
			</div>
		  </fieldset>
		  <fieldset class="fieldset p20_30  ">
			<div class="fieldset_title">
			  <h6>Menus</h6>
			</div>
			<div class="menu_inner  ">
			  <div class="upload_file_repeat">
				<div class="form-group mb_25">
				  <label class="mb_6 f14">Menu Name</label>
				  <input type="text" class="form-control" placeholder="e.g. Food Menu" />
				</div>
				<div class="form-group mb_25">
				  <label class="mb_6 f14">Menu Link</label>
				  <input type="text" class="form-control" placeholder="Enter URL" />
				</div>
				<div class=" form-group mb_25">
				  <label class="mb_6 f14">Images</label>
				  <div class="fileupload mt-0">
					<div class="fileupload-inner">
					  <UploadIcon />
					  <p class="f14">Drag and drop files here</p>
					  <div class="btn-file ">
						<span class="f14">Browse</span>
						<input class="btn-file" type="file">
					  </div>
					</div>
				  </div>
				</div>
				<div class="btn_wrap d-flex">
				  <button type="button" class="btn theme-btn2 w210 add_btn">
					<span>
					  <Cross class="mr_10" />Add Image
					</span>
				  </button>
				</div>
				<hr class="line">
				<!-- <div class="btn_wrap d-flex"><button type="button" class="btn theme-btn2 w210 add_btn"><span><Cross class="mr_10"/>Add New Menu</span></button></div> -->
			  </div>
			  <div class="btn_wrap d-flex">
				<button type="button" class="btn theme-btn-white w210">
				  <span>
					<Cross class="mr_10" /> Add New Menu
				  </span>
				</button>
			  </div>
			</div>
		  </fieldset>
		  <fieldset class="fieldset p20_30  ">
			<div class="fieldset_title">
			  <h6>Photos</h6>
			</div>
			<div class="menu_inner  ">
			  <div class="Images_file_repeat">
				<div class=" form-group mb_25">
				  <label class="mb_6 f14">Image1</label>
				  <div class="fileupload mt-0">
					<div class="fileupload-inner">
					  <UploadIcon />
					  <p class="f14">Drag and drop files here</p>
					  <div class="btn-file ">
						<span class="f14">Browse</span>
						<input class="btn-file" type="file">
					  </div>
					</div>
				  </div>
				</div>
				<div class="form-group mb_25">
				  <label class="mb_6 f14">Caption/Item Name (English)</label>
				  <input type="text" class="form-control" placeholder="Enter caption here" />
				</div>
				<div class="form-group mb_25">
				  <label class="mb_6 f14">Caption/Item Name (Arabic)</label>
				  <input type="text" class="form-control" placeholder="Enter caption here" />
				</div>
				<div class="form-group mb_25">
				  <label class="mb_6 f14">Price (BHD)</label>
				  <input type="text" class="form-control" placeholder="enter price of item" />
				</div>
				<div class="form-group mb_25 custom_multiselect lt_bg ">
				  <label class="mb_6 f14">Cuisines</label>
				  <Multiselect :class="{'custom_select': true, 'form-control':true } " v-model="value" mode="tags" placeholder="Select Cuisines" :options="CuisinesPhoto" />
				</div>
				<div class="form-group mb_25 custom_multiselect lt_bg ">
				  <label class="mb_6 f14">Occassions</label>
				  <Multiselect :class="{'custom_select': true, 'form-control':true } " v-model="value" mode="tags" placeholder="Select Occassions" :options="OccassionsPhoto" />
				</div>
				<div class="btn_wrap d-flex btn_red">
				  <button type="button" class="btn theme-btn-white w210">
					<span>
					  <remove class="mr_10" />Remove Item
					</span>
				  </button>
				</div>
				<hr class="line">
			  </div>
			  <div class="btn_wrap d-flex">
				<button type="button" class="btn theme-btn2 w210">
				  <span>
					<Cross class="mr_10" /> Add Image
				  </span>
				</button>
			  </div>
			</div>
		  </fieldset>
		  <fieldset class="fieldset p20_30  ">
			<div class="fieldset_title">
			  <h6>Shukri’s Favourties</h6>
			</div>
			<div class="menu_inner  ">
			  <div class="shukri_favourties_repeat">
				<div class="form-group mb_25">
				  <label class="mb_6 f14">Item Name (English)</label>
				  <input type="text" class="form-control" placeholder="e.g. Tikka Lumee" />
				</div>
				<div class="form-group mb_25">
				  <label class="mb_6 f14">Item Name (Arabic)</label>
				  <input type="text" class="form-control" placeholder="e.g. Tikka Lumee" />
				</div>
				<div class=" form-group mb_25">
				  <label class="mb_6 f14">Image</label>
				  <div class="fileupload mt-0 border_dots">
					<div class="fileupload-inner">
					  <UploadIcon />
					  <p class="f14">Drag and drop files here</p>
					  <div class="btn-file ">
						<span class="f14">Browse</span>
						<input class="btn-file" type="file">
					  </div>
					</div>
				  </div>
				</div>
				<div class="form-group mb_25">
				  <label class="mb_6 f14">Price (BHD)</label>
				  <input type="text" class="form-control" placeholder="enter price of item" />
				</div>
				<div class="btn_wrap d-flex btn_red">
				  <button type="button" class="btn theme-btn-white w210">
					<span>
					  <remove class="mr_10" />Remove Item
					</span>
				  </button>
				</div>
				<hr class="line">
			  </div>
			  <div class="btn_wrap d-flex">
				<button type="button" class="btn theme-btn2 w210">
				  <span>
					<Cross class="mr_10" /> Add Image
				  </span>
				</button>
			  </div>
			</div>
		  </fieldset>
		  <div class="theme_btn_wrap mt_30">
			<button type="button" class="btn theme-btn2 mr_10">
			  <span>Save</span>
			</button>
			<button type="button" class="btn theme-btn-white">
			  <span>Cancel</span>
			</button>
		  </div>
		</form>
	  </div>
	</div>
  </template>
 
 
 



  
 
 
 <script>
 import Multiselect from '@vueform/multiselect'
 import Cross from '../../../../assets/images/icon/cross.vue';
 import AccessTime from '../../../../assets/images/icon/accesstime.vue';
 import UploadIcon from '../../../../assets/images/icon/UploadIcon.vue';
 import remove from '../../../../assets/images/icon/remove.vue';
 export default {
  name:'RestaurantsEdit',
   components: { Multiselect, Cross, AccessTime, UploadIcon,remove },
   data() {
     return {
		Cuisines: [],
		Occassions: [],
		CuisinesPhoto: [],
		OccassionsPhoto: [],
       Cuisines: ['Mexican', 'Tacos'],
	   Occassions: ['Tourist Spot', 'Lunch & Dinner' , 'Friends Gathering' , 'Celebrations'],
	   CuisinesPhoto: ['Mexican', 'Tacos'],
	   OccassionsPhoto: ['Tourist Spot', 'Lunch & Dinner' , 'Friends Gathering' , 'Celebrations']
     }
   }
 }
</script>

<style src="@vueform/multiselect/themes/default.css"></style>
 