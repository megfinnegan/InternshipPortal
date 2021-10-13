<template> 
        <head>
            <link href="https://unpkg.com/tailwindcss@^2/dist/tailwind.min.css" rel="stylesheet">

        </head>

        <body>
            <header class="text-gray-600 body-font">
                <div class="container mx-auto flex flex-wrap p-5 flex-col md:flex-row items-center">
                  <a class="flex title-font font-medium items-center text-gray-900 mb-4 md:mb-0">
                    <!--svg xmlns="http://www.w3.org/2000/svg" fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="w-10 h-10 text-white p-2 bg-indigo-500 rounded-full" viewBox="0 0 24 24">
                      <path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5"></path-->
                        <!-- Commented out tailwind css logo-->
                    </svg>
                    <span class="ml-3 text-xl">Internship Portal</span>
                  </a>
                  <nav class="md:mr-auto md:ml-4 md:py-1 md:pl-4 md:border-l md:border-gray-400	flex flex-wrap items-center text-base justify-center">
                    <a class="mr-5 hover:text-gray-900">Home</a>
                    <a class="mr-5 hover:text-gray-900">Internships</a>
                    <a class="mr-5 hover:text-gray-900">Student</a>
                    <a class="mr-5 hover:text-gray-900">Business</a>
                  </nav>
                  <button class="inline-flex items-center bg-gray-100 border-0 py-1 px-3 focus:outline-none hover:bg-gray-200 rounded text-base mt-4 md:mt-0">Logout
                    <svg fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="w-4 h-4 ml-1" viewBox="0 0 24 24">
                      <path d="M5 12h14M12 5l7 7-7 7"></path>
                    </svg>
                  </button>
                </div>
              </header>


              <!--business info-->

            <section class="text-gray-600 body-font">
            <div class="container px-5 py-24 mx-auto">
            <div class="flex flex-wrap -m-5">
                <div class="container px-5 py-24 mx-auto">
                <div class="absolute top-20 right-20">
                    <div class="p-4 lg:w-1/10">
                        <div class="h-full bg-yellow-100 bg-opacity-100 p-20 rounded-lg overflow-hidden text-center relative">
                            <h1 class="title-font sm:text-2xl text-xl font-bold text-red-700 mb-3">Business Requests</h1>
                            <br>
                  <div class="flex flex-wrap -m-4">
                    <div class="p-4 lg:w-1/10">
                      
                      <button class="bg-red-500 hover:bg-red-600 text-white sm:text-xl text-xl font-bold shadow-lg px-8 pt-16 pb-24 rounded-lg">Pending</button> 
                   
                    </div>
                    <div class="p-4 lg:w-1/8">

                        <button class="bg-red-500 hover:bg-red-600 text-white sm:text-xl text-xl font-bold shadow-lg px-8 pt-16 pb-24 rounded-lg">Accepted</button> 

                    </div>
                    <div class="p-4 lg:w-1/8">

                        <button class="bg-red-500 hover:bg-red-600 text-white sm:text-xl text-xl font-bold shadow-lg px-8 pt-16 pb-24 rounded-lg">Denied</button> 

                    </div>
                   </div>
                  </div>
                </div>
                </div>
                </div>
             

              <!--student info-->
               
                <div class="container px-8 py-20 mx-auto">
                <div class="absolute top-20 left-20">
                <div class="p-4 lg:w-1/8">
                <div class="h-full bg-yellow-100 bg-opacity-100 px-20 py-10 rounded-lg overflow-hidden text-center align-text-top relative">
                            <h1 class="title-font sm:text-2xl text-xl font-bold text-red-700 mb-3">Student Information</h1>
                            <br>
                  <div class="flex flex-wrap -m-4">
                    <div class="h-full space-x-4 bg-yellow-200 bg-opacity-100 p-5 rounded-lg overflow-hidden text-center relative">
                        <h1 class="title-font sm:text-lg text-lg font-bold text-red-700 mb-3">Weekly-Check in</h1>
                    <div class="p-4 lg:w-1/8">
                      
                      <button class="bg-red-500 hover:bg-red-600 text-white sm:text-xl text-xl font-bold shadow-lg px-8 pt-16 pb-20 rounded-lg">Pending</button> 
                   
                    </div>
                    <div class="p-4 lg:w-1/8">

                        <button class="bg-red-500 hover:bg-red-600 text-white sm:text-xl text-xl font-bold shadow-lg px-8 pt-16 pb-20 rounded-lg">Reviewed</button> 

                    </div>
                  </div>
                  <div class="h-full space-x-4 bg-yellow-200 bg-opacity-100 p-5 rounded-lg overflow-hidden text-center relative">
                    <h1 class="title-font sm:text-lg text-lg font-bold text-red-700 mb-3">Internships</h1>
                    <div class="p-4 lg:w-1/8">

                        <button class="bg-red-500 hover:bg-red-600 text-white sm:text-xl text-xl font-bold shadow-lg px-8 pt-16 pb-20 rounded-lg">Pending</button> 

                    </div>
                    <div class="p-4 lg:w-1/8">

                        <button class="bg-red-500 hover:bg-red-600 text-white sm:text-xl text-xl font-bold shadow-lg px-8 pt-16 pb-20 rounded-lg">Reviewed</button> 

                    </div>
                   </div>
                  </div>
                  </div>
                </div>
                </div>
                </div>
            </div>
            </div>
            </section>
        </body>
    </template>

    <script>
        export default {
          name: "AdminDash",
        };
    </script>