<template>
  <div class="py-12 bg-gray-700">
      <div class="w-2/3 mx-auto grid grid-cols-4 gap-4">

        <div v-for="item in CONTENT.data" :key="item.id">
            <div class="bg-gray-400 h-60 relative">
                <div class="absolute -bottom-6 w-full">
                    <div class="flex justify-center">
                        <div class="p-2 bg-primary text-white font-bold uppercase shadow-sm rounded-md text-sm">{{item.name}}</div>
                    </div>
                </div>
            </div>
            <div class="h-48 flex-col justify-center text-center bg-transparent border border-gray-400 p-8">
                <div class="text-gray-300 border-b border-gray-100">
                    {{item.position}}
                </div>
                <div class="text-white flex items-center">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-14 w-14" viewBox="0 0 20 20" fill="currentColor">
                        <path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z" />
                        <path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z" />
                    </svg>
                    {{item.email}}
                </div>
                <div class="text-white flex items-center">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                        <path d="M2 3a1 1 0 011-1h2.153a1 1 0 01.986.836l.74 4.435a1 1 0 01-.54 1.06l-1.548.773a11.037 11.037 0 006.105 6.105l.774-1.548a1 1 0 011.059-.54l4.435.74a1 1 0 01.836.986V17a1 1 0 01-1 1h-2C7.82 18 2 12.18 2 5V3z" />
                    </svg>
                    {{item.contact}}
                </div>
            </div>
            
        </div>
          
      </div>
      <div class="flex w-2/3 mx-auto">
        <button class="mt-2 bg-primary items-center px-12 py-2 register-primary-bg-color rounded-sm shadow-sm font-bold text-white text-xs self-start uppercase tracking-widest hover:bg-gray-700 active:bg-gray-900 focus:outline-none focus:border-gray-900 focus:shadow-outline-gray transition ease-in-out duration-150">VIEW ALL WORKS</button>
      </div>
  </div>
</template>

<script>
import { CONTENT } from "../constants/data"
export default {
    data() {
        return {
            CONTENT
        }
    },
}
</script>

<style>

</style>