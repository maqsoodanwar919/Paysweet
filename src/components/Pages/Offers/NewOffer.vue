<template>
	<div class="body_wrap">
		<div class="dashboard_body mh-100">
			<div class="title_header d-flex mb_50 justify-content-between align-items-center">
        <h1 class="text-left title ">New Offer</h1> 
      </div>
     <form class="" action="">
		<fieldset class="fieldset bg_none">
			<div class="fieldset_title">
			  <h6>Offer Status</h6>
			</div>
			<div class="form-group mb_25">
			  <label class="mb_6 f14">Status</label>
			  <select class="form-control custom_select">
				<option>Active</option>
			  </select>
			</div> 
		  </fieldset>



		  <fieldset class="fieldset bg_none">
			<div class="fieldset_title">
			  <h6>Main Information</h6>
			</div>
			<div class="form-group mb_25">
                  <label class="mb_6 f14">Offer Code*</label>
                 <input type="text" class="form-control"  placeholder="Offer Code"/>
            </div>
			<div class="form-group mb_25">
                  <label class="mb_6 f14">Restaurant Name*</label>
                 <input type="text" class="form-control"  placeholder="Al Rifai Roastery"/>
            </div>
			<div class="form-group mb_25">
                  <label class="mb_6 f14">Description</label>
                 <input type="text" class="form-control"  placeholder="e.g. 25% off on all items"/>
            </div>
			<div class="row">
				<div class="col-md-6">
					<div class="form-group mb_25 date_wrap">
                  <label class="mb_6 f14">Expiry Date (Optional)</label>
                 <input type="date" class="form-control text_up"  placeholder="DD/MM/YYYY"/>
            </div>
				</div>
				<div class="col-md-6">
					<div class="form-group mb_25 date_wrap">
                  <label class="mb_6 f14">Expiry Date (Optional)</label>
                 <input type="date" class="form-control text_up"  placeholder="DD/MM/YYYY"/>
            </div>
				</div>
			</div>
			<div class=" form-group mb_25">
				  <label class="mb_6 f14">Logo (min 500 x 500)</label>
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
		  </fieldset>

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
 import UploadIcon from '../../../assets/images/icon/UploadIcon.vue';
  export default {
	name:'NewOffer ',
	components: {UploadIcon  },
  }
</script>

 
 
 
 
 
 
 
 