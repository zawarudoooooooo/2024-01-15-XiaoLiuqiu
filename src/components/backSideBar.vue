<script>
export default{
    data(){
        return{

        }
    },
    methods:{
        order(){
            this.$router.push('/BackOrder')
        },
        room(){
            this.$router.push('/BackRoom')
        },
        staff(){
            this.$router.push('/BackStaff')
        }
    }
}
</script>

<template>
    <div class="sideBar">
        <button @click="order()">
            <i class="fa-solid fa-list-check" ></i>訂單管理
        </button>
        <button @click="room()">
            <i class="fa-solid fa-bed"></i>房型管理
        </button>
        <button @click="staff()">
            <i class="fa-solid fa-users"></i>員工管理
        </button>
    </div>    
</template>

<style lang="scss" scoped>
    .sideBar{
        width: 15vw;
        gap: 2vmin;
        display: grid;
        button{
            width: 15vw;
            height: 10vh;
            border: none;
            border-radius: 5px;
            color: #4d4327;
            font-size: 16pt;
            box-shadow: 0.5px 0.5px 0.5px 0.5px rgba(2, 40, 63, 0.2);
            &:hover{
                background-color: #797A7E;
                color: white;
            }
            &:active{
                background-color: #F7F2E7;
                color: #797A7E;
            }
            i{
                margin-right: 1vmin;
            }
        }
    }
</style>