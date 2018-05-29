<template>
    <span>test</span>    
</template>
<script>
    import axios from 'axios';
    export default {
        mounted() {
            this.init();
        },
        methods: {
            init() {
                // http://localhost/
                axios.get('/app.php')
                .then(function (res) {
                    console.log(res);
                })
                .catch(function (err) {
                    console.log(err);
                })
            }
        }
    }
</script>
