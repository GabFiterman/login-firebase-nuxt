<template>
  <div id="login">
    <h2>Login</h2>
    <form @sobmit.prevent="pressed">
        <div class="login">
            <input type="exit" placeholder="login" v-model="login" />
        </div>

        <div class="password">
            <input type="password" placeholder="password" v-model="password" />
        </div>

        <div class="submit">
            <button>Submit</button>
        </div>

        <div class="error" v-if="error">{{error.message}}</div>

    </form>
  </div>
</template>

<script>
export default {
    name: 'login',
    data(){
        return{
            email: '',
            password: '',
            error: ''
        }
    },
    methods:{
        pressed(){
            alert('pressed');
        }
    }
}
</script>

<style scoped>
#login{
    color: white;
    display: flex;
    flex-flow: column;
    align-items: center;
    justify-content: center;
}

#login h2{
    margin: 1.5rem 0;
}

#login input, #login button{
    color: white;
    background-color: rgba(255,255,255,0.25);
    margin: 0.5rem;
    border: none;
    border-radius: 2rem;
    padding: 1rem 2rem;
    min-width: 25vw;
}

#login button{
    background-color: #D2691E;
    font-weight: bold;
    transition: all 0.45s;
}

#login button:hover{
    filter: brightness(0.75);
}
</style>