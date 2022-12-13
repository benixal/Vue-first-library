<template>
    <div>
        <button @click="sayhi">click here {{name}}</button>
    </div>
    <div>{{himsg}}</div>
</template>

<script>
export default {
    name:"SayHi",
    props: {
        name:String
    },
    data:()=> {
        return {
            himsg:'welcome'
        }
    },
    methods: {
        sayhi:function() {
            this.himsg = "Hi "+this.name;
        }
    },
}
</script>