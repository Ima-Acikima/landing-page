<template>
  <div class="bg-primary p-4 text-white">
      <div class="w-2/3 mx-auto">
        <div class="flex justify-center text-center">
            <div class="flex space-x-3 bg-gray-100 shadow-sm border rounded-md text-primary font-bold uppercase p-2 text-sm">
                {{reviews[0].name}} <span class="text-gray-400 ml-3 capitalize italic">- {{reviews[0].position}}</span>
            </div>
            
        </div>
        <div class="mt-3">
            <span class="text-4xl mr-2">"</span> {{reviews[0].review}}<span class="text-4xl ml-2">"</span>
        </div>

      </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            reviews: [
                {
                    name: "Alexis Simpson",
                    position: "CEO & Developer",
                    review: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut blandit porta mauris sit amet elementum. Sed volutpat in metus in ultricies. Vestibulum at nibh at erat placerat sollicitudin. Donec eleifend, ipsum eget lacinia sollicitudin, mi erat bibendum eros, a pharetra."
                },
                {
                    name: "Louisa Farrington",
                    position: "Writer",
                    review: "Donec non neque ut justo suscipit suscipit vel at nulla. Praesent dignissim tortor vel elit pellentesque, non faucibus nulla semper."
                },
                {
                    name: "Primrose Ridley",
                    position: "Lecturer",
                    review: "Vivamus ultricies mattis dolor sed varius. Donec facilisis dictum enim, et sollicitudin urna maximus quis. Cras facilisis augue non lorem."
                },
                {
                    name: "Phillipa Morin",
                    position: "Student",
                    review: "Sed euismod nisi metus, vel hendrerit neque porttitor id. Ut sit amet varius metus. In commodo commodo quam at commodo."
                }
            ]
        }
    },

}
</script>

<style>


</style>