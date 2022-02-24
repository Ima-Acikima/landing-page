<template>
  <div class="sm:w-2/3 mx-auto my-12">
    <div>
        <div class="text-3xl italic font-bold register-primary-color text-left mb-3">
            Register Your Interest
        </div>
        <div class="border rounded-md p-4">
            <div class="grid grid-cols-2 gap-4">
                <input v-model="name" placeholder="Name" class="p-2 border border-gray-300 rounded-md" />
                <select v-model="occupation" placeholder="Occupation" class="appearance-none p-2 border border-gray-300 rounded-md">
                    <option>A</option>
                    <option>A</option>
                    <option>A</option>
                </select>
                <input v-model="email" placeholder="Email" type="email" class="p-2 border border-gray-300 rounded-md" />
                <input v-model="contact" placeholder="Contact No" type="tel" class="p-2 border border-gray-300 rounded-md" />
                <textarea v-model="message" placeholder="Message" class="p-2 border border-gray-300 rounded-md" />

            </div>
            <div class="flex mt-4">
                <button class="inline-flex items-center px-12 py-2 register-primary-bg-color rounded-sm shadow-sm font-bold text-white text-xs self-start uppercase tracking-widest hover:bg-gray-700 active:bg-gray-900 focus:outline-none focus:border-gray-900 focus:shadow-outline-gray transition ease-in-out duration-150">
                    SUBMIT MESSAGE
                </button>
            </div>
        </div>
    </div>
      
  </div>
</template>

<script>
export default {
    data() {
        return {
            name: null,
            occupation:null,
            email: null,
            contact:null,
            message: null
        }
    },

}
</script>

<style scoped>
.register-primary-color {
    color: #00A99D
}

.register-primary-bg-color {
    background-color: #00A99D
}

</style>