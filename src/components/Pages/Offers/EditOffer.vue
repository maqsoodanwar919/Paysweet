<template>
	<div class="body_wrap">
		<div class="dashboard_body mh-100">
			<div class="title_header d-flex mb_50 justify-content-between align-items-center">
        <h1 class="text-left title ">Edit Cuisine</h1> 
		<button type="button" class="btn theme-red">Delete</button>
      </div>
     <form class="" action="">
		  
			<div class="form-group mb_25">
				<label class="mb_6 f14">Cuisine Name (English)*</label>
				<input type="text" class="form-control"  placeholder="American"/>
             </div>

			 <div class="form-group mb_25">
				<label class="mb_6 f14">Cuisine Name (Arabic)*</label>
				<input type="text" class="form-control"  placeholder="امريكي"/>
             </div>

			 <div class=" form-group mb_25">
				  <label class="mb_6 f14">Main Image* (min 500 x 500)</label>
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
				<div class="form-group mb_25 custom_multiselect   ">
				  <label class="mb_6 f14">Restaurants</label>
				  <Multiselect :class="{'custom_select': true, 'form-control':true } " v-model="value" mode="tags" placeholder="Select Cuisines" :options="RestaurantsOption" />
					<span></span>
				</div>

		 

        <!-- theme_btn_wrap -->
       <div class="theme_btn_wrap mt_50">
        <button type="button" class="btn theme-btn2 mr_10"><span>Save</span></button>
        <button type="button" class="btn theme-btn-white"><span>Cancel</span></button> 
       </div>
      </form>
	 
		</div>
	</div> 
</template>
 
 
 


<script> 
 import Multiselect from '@vueform/multiselect'
 import UploadIcon from '../../../assets/images/icon/UploadIcon.vue';
  export default {
	name:'EditOffer ',
	components: {UploadIcon ,Multiselect },

	data() {
     return {
		Restaurants: [], 
		RestaurantsOption: ['Papa Johns', 'Nandos' , 'Fuddruckers' , 'Texas Chicken','KFC','Five Guys Burger & Fries','Blaze','Costa Coffee','Cheezo','Frankie’s','Burgers & Shakes','Jasmi’s','Texas Roadhouse']
     }
   }
  }
</script>

 
 
 
 
 
 
 
 