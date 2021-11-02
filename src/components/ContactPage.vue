<template>
  <div>
    <div class="text-gray-600 body-font relative">
      <div class="container px-5 py-24 mx-auto">
        <div class="flex flex-col text-center w-full mb-12">
            <h1 class="sm:text-3xl text-2xl font-medium title-font mb-4 text-gray-900">Contact Us</h1>     
        </div>
        <div class="lg:w-1/2 md:w-2/3 mx-auto">
            <div class="flex flex-wrap -m-2">
                  <div class="p-2 w-1/2">
                    <div class="relative">
                      <label for="name" class="leading-7 text-sm text-gray-600">Name</label>
                      <input 
          
                      class="
                      w-full 
                      bg-gray-100 
                      bg-opacity-50 
                      rounded 
                      border 
                      border-gray-300 
                      focus:border-indigo-500 
                      focus:bg-white 
                      focus:ring-2 
                      focus:ring-indigo-200 
                      text-base 
                      outline-none 
                      text-gray-700 
                      py-1 
                      px-3 
                      leading-8 
                      transition-colors 
                      duration-200 
                      ease-in-out
                      "
                      placeholder="Name"
                      type="text" 
                      @input="nameChange($event.target.value)"
                      id="input-name" 
                      v-model="inputName"
                      />
                    </div>
                  </div>
                  <div class="p-2 w-1/2">
                    <div class="relative">
                      <label for="email" class="leading-7 text-sm text-gray-600">Email</label>
                      <input 
                      class="
                      w-full 
                      bg-gray-100 
                      bg-opacity-50 
                      rounded 
                      border 
                      border-gray-300 
                      focus:border-indigo-500 
                      focus:bg-white 
                      focus:ring-2 
                      focus:ring-indigo-200 
                      text-base 
                      outline-none 
                      text-gray-700 
                      py-1 
                      px-3 
                      leading-8 
                      transition-colors 
                      duration-200 
                      ease-in-out
                      "
                      placeholder="Email"
                      type="email" 
                      @input="emailChange($event.target.value)"

                      id="input-email" 
                      v-model="inputEmail"
                      />
                    </div>
                  </div>
                  <div class="p-2 w-full">
                    <div class="relative">
                      <label for="message" class="leading-7 text-sm text-gray-600">Message</label>
                      <textarea 
                        class="
                          w-full 
                          bg-gray-100 
                          bg-opacity-50 
                          rounded 
                          border 
                          border-gray-300 
                          focus:border-indigo-500 
                          focus:bg-white 
                          focus:ring-2 
                          focus:ring-indigo-200 
                          h-32 
                          text-base 
                          outline-none 
                          text-gray-700 
                          py-1 
                          px-3 
                          resize-none 
                          leading-6 
                          transition-colors 
                          duration-200 
                          ease-in-out
                        "
                        placeholder="Message"
                        @input="messageChange($event.target.value)"
                        id="input-message" 
                        v-model="inputMessage"
                      >
                      </textarea>
                    </div>
                  </div>
                  <div class="p-2 w-full">
                    <button 
                      class="
                        flex 
                        mx-auto 
                        text-white 
                        bg-red-500 
                        font-medium 
                        border-0 
                        py-2 
                        px-11 
                        focus:outline-none 
                        hover:bg-red-600 
                        rounded 
                        text-lg
                      "
                      v-on:click="submitForm"
                    >
                      Submit
                    </button>
                  </div>
                 
            </div>
        </div>
      </div>
    </div>
  </div> 
</template>

<script>


export default {
    name: "ContactForm", 
    data(){
      return{
        form: {
          userName: "", 
          userEmail: "", 
          userMessage: "", 
        },
      };
    },

    methods: {

        nameChange(value){ 
          this.userName = value; 
        },

        emailChange(value){
          this.userEmail = value; 
        }, 

        messageChange(value){
          this.userMessage = value; 
        },

        submitForm() {
          const body = {
            user_name: this.userName, 
            user_email: this.userEmail, 
            user_message: this.userMessage,
          };

          console.log(body);
          console.log(JSON.stringify(body)); 
          fetch(`${process.env.SERVER_URL}/contact-form`, {  //contact-form is just a placeholder doesnt exist rn
            method: "POST", 
            mode: "cors", 
            credentials: "same-origin", 
            headers: {
              "Content-Type": "application/json",
            },
            body: JSON.stringify(body), 
          }).then((res) => {
            if (res.status == 200) {
              window.location.href = "/"; 
            } else { 
              alert("Failed"); 
            }
          });
            
        },
    },
};
</script>
