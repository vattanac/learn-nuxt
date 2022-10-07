<template>
    <div>
        <input type="text" v-model="productId">
        <button @click="onLoadProduct">Load Product</button>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                productId:''
            }
        },
        methods: {
            onLoadProduct() {
                this.$router.push('/products/' + this.productId)
            }
        }
    }
</script>