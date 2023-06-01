<template>
	<div class="body_wrap">
		<div class="dashboard_body mh-100">
			<div class="title_header d-flex mb_50 justify-content-between align-items-center">
				<h1 class="text-left title ">App Users</h1> </div>
			<div class="custom_table user_table">
				<div class="row table_search_filter align-items-center justify-content-between">
					<div class="col-3">
						<div class="form-group mb_25">
							<label class="mb_6 f14">Change Birthday Request</label>
							<select class="form-control custom_select">
								<option>All</option>
							</select>
						</div>
					</div>
					<div class="col-2 text-end ml-auto ">
						<a href="#" class="linke_reest a_over">Reset filters</a>
					</div>
				</div>
				<table class="table mb-0">
					
					<thead class="bg_head border_head">
						<tr>
							 
							<th scope="col" class="f16 lit_clr">ID</th>
							<th scope="col"  class="f16 lit_clr">
								First Name
							</th>
							<th scope="col" class="f16 lit_clr">Last Name</th>
							<th scope="col" class="f16 lit_clr">Mobile Number</th>
							<th scope="col" class="f16 lit_clr"> Birthday</th>
							<th scope="col" class="f16 lit_clr"> Change Birthday Request</th>
							<th scope="col" class="f16 lit_clr"></th>
						</tr>
					</thead>
					<tbody>
						<tr> 
							<td class="f14">1</td>
							<td class="f14">Maryam</td>
							<td class="f14">Shukri</td>
							<td class="f14">+973 12345678</td>
							<td class="f14">15/08/1983</td>
							<td class="f14">-</td>
							<td class="f14"> <div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div> </td>
						</tr>
						<tr> 
							<td class="f14">2</td>
							<td class="f14">Ahmed</td>
							<td class="f14">Mohamed</td>
							<td class="f14">+973 12345678</td>
							<td class="f14">20/02/2001</td>
							<td class="f14">-</td>
							<td class="f14"> <div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div> </td>
						</tr>
						<tr> 
							<td class="f14">3</td>
							<td class="f14">Hasan</td>
							<td class="f14">Maki</td>
							<td class="f14">+973 12345678</td>
							<td class="f14">13/05/1995</td>
							<td class="f14">-</td>
							<td class="f14"> <div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div> </td>
						</tr>
						<tr> 
							<td class="f14">4</td>
							<td class="f14">Dias</td>
							<td class="f14">Maki</td>
							<td class="f14">+973 12345678</td>
							<td class="f14">16/12/1989</td>
							<td class="f14">Yes</td>
							<td class="f14"> <div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div> </td>
						</tr>
						<tr> 
							<td class="f14">5</td>
							<td class="f14">Ekstrom</td>
							<td class="f14">Maki</td>
							<td class="f14">+973 12345678</td>
							<td class="f14">15/08/1983</td>
							<td class="f14">-</td>
							<td class="f14"> <div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div> </td>
						</tr>
						<tr> 
							<td class="f14">6</td>
							<td class="f14">Gustavo</td>
							<td class="f14">Herwitz</td>
							<td class="f14">+973 12345678</td>
							<td class="f14">20/02/2001</td>
							<td class="f14">-</td>
							<td class="f14"> <div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div> </td>
						</tr>
						<tr> 
							<td class="f14">6</td>
							<td class="f14">Cooper</td>
							<td class="f14">Culhane</td>
							<td class="f14">+973 12345678</td>
							<td class="f14">Culhane</td>
							<td class="f14">-</td>
							<td class="f14"> <div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div> </td>
						</tr>
						 
					</tbody>
					<tfoot > 
						<tr>
							<td colspan="6">
								<table class="w-100">
									<tr>
										<td>
											<div class="table_footer d-flex justify-content-between align-items-center table_pd">
												<p class="mb-0"><b>Showing 1 to 7 of 7 results</b></p>
												<div class="pages_wrap d-flex  align-items-center mr-2">
													<div class="select">
														<select name="format" id="format">
															<option value="">1</option>
															<option value="">2</option>
															<option value="">3</option>
															<option value="">4</option>
															<option value="">5</option>
															<option value="">6</option>
															<option value="">7</option>
															<option value="">8</option>
															<option value="">9</option>
															<option value="">10</option>
														</select>
													</div> <span class="f14 ">per page</span> </div>
												<div class="table_pagination">
													<!-- ewew -->
												</div>
											</div>
										</td>
									</tr>
								</table>
							</td>
						</tr>
					</tfoot>
				</table>
			</div>
		</div>
	</div>
</template>
 
 
 



 <script >  
 import Search from '../../../assets/images/icon/search.vue';
 import Edit from '../../../assets/images/icon/edit.vue';
   export default{
   name:'AppUser',
   components: {
    Search,Edit
  },
  }
 </script>
 
 
 
 
 
 
 <style >
  
 </style>
 