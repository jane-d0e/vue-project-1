<template>
    <div class="app">
        <div class="btn-cont">
            <button @click="addLikes" class="btn">Add likes</button>
            <button @click="addDislikes" class="btn">Add dislikes</button>
        </div>

        <p>Count likes - <strong>{{likes}}</strong></p>
        <p>Count dislikes - <strong>{{dislikes}}</strong></p>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                likes: 0,
                dislikes: 0,
            } 
        },
        methods: {
            addLikes() {
                this.likes +=1;
            },
            addDislikes() {
                this.dislikes +=1;
            }
        }
    }
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');
    /* * {
        margin: 0;
        padding: 0;
    } */
    
    body {
        font-family: "Tahoma";
        font-weight: 100;
    }

    .app {
        display: flex;
        min-height: 100vh;
        min-width: 100%;

        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    .btn {
        display: inline-block;
        padding: 15px;
        background: none;
        border: 1px solid teal;
        border-radius: 6px;

        margin: 6px;
    }
</style>