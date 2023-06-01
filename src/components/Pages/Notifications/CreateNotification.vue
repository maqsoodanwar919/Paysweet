

<template> 
<div class="body_wrap">
		<div class="dashboard_body mh-100">
			<div class="title_header d-flex mb_50 justify-content-between align-items-center">
        <h1 class="text-left title ">Create New Notification</h1>
      <button type="button" class="btn theme-red">Delete</button>
      </div>
     <form class="" action="">
        <div class="row">
          <div class="col-md-11">
            <div class="form-group mb_25">
                  <label class="mb_6 f14">Title*</label>
                 <input type="text" class="form-control"  placeholder="Enter name"/>
            </div>
            <div class="form-group mb_25">
                  <label class="mb_6 f14">Message*</label>
                 <textarea class="form-control h80" placeholder="Description of the restaurant"></textarea>
            </div> 
            </div>  
            <label class="f14 mb_20">This notifications links to</label>
           <div class="row  ">
            <div class="col-md-3">
              <div class="form-group mb_25"> 
                  <div class="input_wrap">
                <input type="radio" class="" name="notifications-links" id="General_App" >
                <label class="label-text f14" for="General_App"><span>General App</span></label>
              </div>
            </div>
            </div>
            <div class="col-md-3">
              <div class="form-group mb_25"> 
                  <div class="input_wrap">
                <input type="radio" class="" name="notifications-links" id="Offers_Section" >
                <label class="label-text f14" for="Offers_Section"><span>Offers Section</span></label>
              </div>
            </div>
            </div>
           </div>
           <div class="row  ">
            <div class="col-md-3">
              <div class="form-group mb_25"> 
                  <div class="input_wrap">
                <input type="radio" class="" name="notifications-links" id="Restaurant" >
                <label class="label-text f14" for="Restaurant"><span>Restaurant</span></label>
              </div>
            </div>
            </div>
            <div class="col-md-3">
              <div class="form-group mb_25"> 
                  <div class="input_wrap">
                <input type="radio" class="" name="notifications-links" id="Collaboration_Item" >
                <label class="label-text f14" for="Collaboration_Item"><span>Collaboration Item</span></label>
              </div>
            </div>
            </div>
          </div>
          <div class="row  ">
            <div class="col-md-3">
              <div class="form-group mb_25"> 
                  <div class="input_wrap">
                <input type="radio" class="" name="notifications-links" id="cco" >
                <label class="label-text f14" for="cco"><span>Cuisine/Category/Occassion</span></label>
              </div>
            </div>
            </div>
            <div class="col-md-3">
              <div class="form-group mb_25"> 
                  <div class="input_wrap">
                <input type="radio" class="" name="notifications-links" id="Surprise" >
                <label class="label-text f14" for="Surprise"><span>‘Surprise Me’ Section</span></label>
              </div>
            </div>
            </div>
            </div>
            <div class="col-md-11">
            <div class="form-group mb_25">
              <label class="mb_6 f14">Status</label>
              <select class="form-control custom_select">
                <option>Draft</option>
              </select>
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
  export default{
   name:'CreateNotification',
    
  }
 </script>
 
 
 
 
 
 
 <style scoped>
  
 </style>
 