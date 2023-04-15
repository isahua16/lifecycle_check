<template>
    <div>
        <h1>{{blog_title}}</h1>
        <i>{{likes}}</i>
        <img :src="blog_image_url" alt="">
        <p>{{blog_content}}</p>
        <button @click="like_blog">Like</button>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                blog_content: `Yeah, but your scientists were so preoccupied with whether or not they could, they didn't stop to think if they should. God creates dinosaurs. God destroys dinosaurs. God creates Man. Man destroys God. Man creates Dinosaurs. This thing comes fully loaded. AM/FM radio, reclining bucket seats, and... power windows. 
                
                God help us, we're in the hands of engineers. God help us, we're in the hands of engineers. Forget the fat lady! You're obsessed with the fat lady! Drive us out of here! My dad once told me, laugh and the world laughs with you, Cry, and I'll give you something to cry about you little bastard!`,
                blog_title: `My Blog Post`,
                blog_image_url: `https://images.unsplash.com/photo-1474552226712-ac0f0961a954?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=3542&q=80`,
                likes: 0
            }
        },
        methods: 
        {
            like_blog: function()
            {
                this.likes++;
            }
        }    
    }
</script>

<style scoped>
    img {
        width: 100%;
    }

    p {
        white-space: pre-line;
    }
</style>