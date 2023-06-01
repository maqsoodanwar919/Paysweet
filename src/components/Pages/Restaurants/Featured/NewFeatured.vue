<template>
	<div class="body_wrap">
		<div class="dashboard_body mh-100">
			<div class="title_header d-flex mb_50 justify-content-between align-items-center">
				<h1 class="text-left title ">New Featured List</h1> 
			</div>
			<form class="" action="">
				<div class="row">
					<div class="col-md-11">
						<div class="form-group mb_25">
							<label class="mb_6 f14">Status</label>
							<select class="form-control custom_select">
								<option>Draft</option>
							</select>
						</div> 
					<div class="form-group mb_25">
							<label class="mb_6 f14">List Title (English)*</label>
							<input type="text" class="form-control" placeholder="e.g. The Golden List" /> 
					</div>
					<div class="form-group mb_25">
							<label class="mb_6 f14">List Title (Arabic)*</label>
							<input type="text" class="form-control" placeholder="e.g. The Golden List" /> 
					</div> 

					 
						<div class="form-group mb_25 custom_multiselect ">
							<label class="mb_6 f14">Restaurants</label>
							<Multiselect
							:class="{'custom_select': true, 'form-control':true } "
							v-model="value"
							mode="tags"
							placeholder="Select Restaurant"
							:options="options"
							/> 
						</div>
				  
				 
				</div>
				</div>
				<!-- theme_btn_wrap -->
				<div class="theme_btn_wrap mt_30">
					<button type="button" class="btn theme-btn2 mr_10"><span>Save</span></button>
					<button type="button" class="btn theme-btn-white"><span>Cancel</span></button>
				</div>
			</form>
		</div>
	</div>
</template>
 
 
 


<script>
  import Multiselect from '@vueform/multiselect'

  export default {
    components: { Multiselect },
    data() {
      return {
        value: [],
        options: ['Papa Johns', 'Nandos', 'Fuddruckers','Texas Chicken' ,'KFC' , 'Five Guys Burger & Fries']
      }
    }
  }
</script>

<style src="@vueform/multiselect/themes/default.css"></style>
 
 
 
 
 
 
 