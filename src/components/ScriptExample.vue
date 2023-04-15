<template>
    <section>

    </section>
</template>

<script>
    export default {
        data() {
            return {
                tweets: [
                            "Just had the best sushi ever!",
                            "Why does everyone love avocado toast so much?",
                            "I can't believe it's already Friday!",
                            "Another day, another dollar",
                            "Life is short, eat the cake",
                            "Can't wait to travel again soon!",
                            "Nothing beats a good book on a rainy day",
                            
                        ],
                num_friends: 10,
                logged_in: true
                    }
            },
        methods: {
            show_info() 
            {
                document.querySelector(`section`).insertAdjacentHTML(`afterbegin`, `<p>Number of Friends:${this.num_friends}</p>`);
                document.querySelector(`section`).insertAdjacentHTML(`afterbegin`, `<p>Is User Logged In:${this.logged_in}</p>`);
                for(let i = 0; i < this.tweets.length; i++)
                {
                    document.querySelector(`section`).insertAdjacentHTML(`afterbegin`, `<p>${this.tweets[i]}</p>`);
                }
            },


        },
        mounted: function()
        {
            this.show_info();
        }
        }
</script>

<style scoped>

</style>