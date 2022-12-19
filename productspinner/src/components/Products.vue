<template>
    <div v-if="array.length">
        <div v-for="item in array" :key="item">
    
            <div class="container w-25 mx-auto">
                <div class="row">
                    <div class="card m-5">
                        <img :src="item.image" class="card-img-top" alt="">
                        <div class="card-body">
                            <h4 class="card-title text-black">{{ item.name }}</h4>
                            <p class="card-text text-black">In Stock: {{ item.quantity }}</p>
                            <p class="card-text text-black">Price: {{ item.price }}</p>
                            <button id='addCheckout' class="cart-btn">🛒</button>
                        </div>
                    </div>
                </div>
            </div>
    
        </div>
    </div>

    <div v-else><SpinnerVue></SpinnerVue></div>

<!--  -->
</template>
  
<script>
import SpinnerVue from '../components/Spinner.vue';
export default {
    data() {
        return {
            array: [
                // {
                //     name: "Graphic T",
                //     price: 800,
                //     image: "https://i.postimg.cc/P56qnJ4S/Crew-Neck-1.jpg",
                //     quantity: 1
                // },
                // {
                //     name: " Graphic Sweat-Shirt",
                //     price: 1000,
                //     image: "https://i.postimg.cc/L8tD8d7Y/Graphic-Sweat-Shirt-1.jpg",
                //     quantity: 3
                // },
                // {
                //     name: "Carhartt Bones Jacket",
                //     price: 2200,
                //     image: "https://i.postimg.cc/1XzWTW5C/Carhartt-Bones-1.jpg",
                //     quantity: 2
                // },
                // {
                //     name: "Graphic SW Pants",
                //     price: 1800,
                //     image: "https://i.postimg.cc/cCfd6Mnc/275834450-542228100497493-5314424466359396574-n.jpg",
                //     quantity: 4
                // }
            ]
        };
    },
    components: {
         SpinnerVue,
    }
}
</script>
    
<style scoped>
.cart-btn {
    background-color: white;
    border: none;
    margin-bottom: 10px;
}

.cart-btn:hover {
    background-color: rgb(67, 67, 67);
    border: none;
}
</style>