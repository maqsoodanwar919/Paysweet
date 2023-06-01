<template> 
   
   <div class="main-card">
    <div class="head_wrap">
          <h1>Payment requests</h1>
          <button class="btn_primary"> <plus /> Create request</button>
      </div>
      <div class="inner_box">
        <div class="table-head">
           <button class="btn_outline_light"><plus /> Add filter</button>
           <div class="search_Wrap">
             <input type="text" class="form-control" placeholder="Search">
             <search />
           </div>
        </div> 
        <div class="table_custom ">
            <table class="table  ">
        <thead>
          <tr>
            <th scope="col">
                <div class="custom-control custom-checkbox">
                  <input type="checkbox" class="custom-control-input" id="customCheck1"  >
                  <label class="custom-control-label" for="customCheck1">Payment ID</label>
              </div> 
            </th>
            <th scope="col">Customer</th>
            <th scope="col">Amount</th>
            <th scope="col">Status</th>
            <th scope="col">Date created</th>
            <th scope="col">Due date</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>
              <div class="custom-control custom-checkbox">
                  <input type="checkbox" class="custom-control-input" id="customCheck1"  >
                  <label class="custom-control-label" for="customCheck1">#2023-00005</label>
              </div>
            </td>
            <td>Jane Smith</td>
            <td>€ 1350</td>
            <td><span class="badge bg-info">Open</span></td>
            <td>31/04/2023</td>
            <td>31/04/2023</td> 
          </tr>
          <tr>
            <td>
              <div class="custom-control custom-checkbox">
                  <input type="checkbox" class="custom-control-input" id="customCheck2">
                  <label class="custom-control-label" for="customCheck2">#2023-00005</label>
              </div>
            </td>
            <td>Jane Smith</td>
            <td>€ 1350</td>
            <td><span class="badge bg-success">Paid</span></td>
            <td>31/04/2023</td>
            <td>31/04/2023</td> 
          </tr>
          <tr>
            <td>
              <div class="custom-control custom-checkbox">
                  <input type="checkbox" class="custom-control-input" id="customCheck2">
                  <label class="custom-control-label" for="customCheck2">#2023-00005</label>
              </div>
            </td>
            <td>Jane Smith</td>
            <td>€ 1350</td>
            <td><span class="badge bg-warning">Overdue</span></td>
            <td >31/04/2023</td>
            <td class="text_warning">31/04/2023</td> 
          </tr>
          <tr>
            <td>
              <div class="custom-control custom-checkbox">
                  <input type="checkbox" class="custom-control-input" id="customCheck2">
                  <label class="custom-control-label" for="customCheck2">#2023-00005</label>
              </div>
            </td>
            <td>Jane Smith</td>
            <td>€ 1350</td>
            <td><span class="badge bg-success">Paid</span></td>
            <td>31/04/2023</td>
            <td>31/04/2023</td> 
          </tr>
          <tr>
            <td>
              <div class="custom-control custom-checkbox">
                  <input type="checkbox" class="custom-control-input" id="customCheck2">
                  <label class="custom-control-label" for="customCheck2">#2023-00005</label>
              </div>
            </td>
            <td>Jane Smith</td>
            <td>€ 1350</td>
            <td><span class="badge bg-success">Paid</span></td>
            <td>31/04/2023</td>
            <td>31/04/2023</td> 
          </tr>
          
        </tbody>
      </table>
        </div>
      </div>
      
   </div>   
      
</template>



<script>   
import plus from '../assets/images/icon/plus.vue';
import search from '../assets/images/icon/search.vue';



export default {
    components: {
        plus,search,
    },
    // ...Other stuff here
}

</script>