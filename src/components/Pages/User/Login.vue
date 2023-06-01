
<template>  
  <div class="body_wrap">
      <div class="dashboard_body mh-100 login_page">  
          <div class="login_form">
           <div class="login_logo"> <login_logo /></div>
           <h4 class="title"> Login</h4>
             <form action="">
              <div class="form-group mb_25">
							<label class="mb_6 f14">Email Address <span class="staric">*</span></label>
							<input type="email" class="form-control" placeholder="Enter name" /> 
            </div>
            <div class="form-group mb_25">
							<label class="mb_6 f14">Password <span class="staric">*</span></label>
							<input type="password" class="form-control" placeholder="Enter name" /> </div>

                 <div class="checkbox_wrap">
										<input type="checkbox" name="iagree_to_be_contacted" id="news-regarding" class="">
										<label for="news-regarding" class="f14">Click to confirm you have read and understand the </label>
									</div>


              <div class="theme_btn_wrap mt_30">
					<button type="button" class="btn theme-btn2"><span>Sign in</span></button> 
				</div>
             </form>
          </div>
      </div>
  </div>  
</template>
 
 
 



 <script>  
 import login_logo from '../../../assets/images/icon/login_logo.vue';
 
  export default{
   name:'Login', 
    components: {
      login_logo  
    },
    // ...Other stuff here 
  }
 </script>
 
 
 
 
 
 
 <style scoped>
  
 </style>
 