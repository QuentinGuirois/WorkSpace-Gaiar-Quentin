<template>
    
</template>

<script>

import axios from "axios";

export default {
    setup() {
        console.log('script récupéré');

        //Chercher la reponse renvoyée par l'api
        const getPosts = async () => {
            let posts = await axios.get('/api/posts');
            console.log(posts);
        }
    },
}
</script>
