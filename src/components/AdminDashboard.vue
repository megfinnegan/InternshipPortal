<template>
  <section>
    <div class="min-h-screen"> 
      <div class="grid grid-cols-5 grid-rows-2 gap-3 p-5">
        <div class="col-start-1 bg-gray-100 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">15 Total Listings</div> 
        <div class="col-start-2 col-span-4 row-start-1 row-end-3 bg-gray-100 text-gray-500 text-lg font-bold text-center p-10 pb-20 rounded-lg">Positions Density</div>
        <div class="relative col-start-2 col-span-4 row-start-3 row-end-6 bg-gray-100 text-gray-500 text-lg font-bold text-center py-0 px-10 rounded-lg">
            
            <div class="min-h-screen flex items-center">
              <div class="flex overflow-x-scroll">
                <div class="flex flex-nowrap">
                  <div class="inline-block px-3">
                    <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                  <div class="inline-block px-3">
                    <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                  <div class="inline-block px-3">
                    <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                  <div class="inline-block px-3">
                    <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                  <div class="inline-block px-3">
                    <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                  <div class="inline-block px-3">
                   <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                  <div class="inline-block px-3">
                    <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                  <div class="inline-block px-3">
                    <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                  <div class="inline-block px-3">
                    <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                  <div class="inline-block px-3">                  
                    <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                  <div class="inline-block px-3">
                    <div class="bg-gray-400 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Pending Listings</div>
                  </div>
                </div>
              </div>
            </div> 
        </div>
        <div class="col-start-1 row-start-2 bg-gray-100 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Most Viewed Company</div>
        <div class="col-start-1 row-start-3 bg-gray-100 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">Software Engineer: Most Viewed Position</div>
        <div class="col-start-1 row-start-4 bg-gray-100 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">20 Total Monthly Visits</div>
        <div class="col-start-1 row-start-5 bg-gray-100 text-gray-500 text-lg font-bold text-center p-10 rounded-lg">5 Pending Contact Requests</div>
        
      </div>
    </div>
  </section>
</template>

<script>
import AdminStats from "./AdminStats.vue";
import AdminCard from "./AdminCard.vue";
export default {
  name: "AdminDashboard",
  components: {
    AdminStats,
    AdminCard,
  },
};
</script>
