<template>
  <section class="container">
    <h2>Basic List Group</h2>
    <ul class="list-group">
        <!-- this code currently has a problem with vetur :( -->
        <!-- <li v-for= "item in exampleList" >
            {item.name}
        </li> -->
        
    </ul>
  </section>
</template>

<script>

    export default {
        components: {
            AppLogo
        },
        data(){
            return {
                exampleList: [
                    {
                        name: 'Weyden',
                        email: 'weydenherrera@gmail.com'
                    },
                    {
                        name: 'Andy',
                        email: 'andy.dyems@gmail.com'
                    }
                ]
            }
        }
    }

</script>