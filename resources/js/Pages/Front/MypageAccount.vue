<script setup lang="ts">
const shippings = [
    {
        'id': 1,
        'name': '妻夫木聡',
        'address': '東京都国立市東',
        'phonenumber': '03-3333-3333'
    },
    {
        'id': 2,
        'name': '木村拓哉',
        'address': '大阪府大阪市',
        'phonenumber': '06-6666-6666'
    },
    {
        'id': 3,
        'name': '綾瀬はるか',
        'address': '大阪府大阪市',
        'phonenumber': '06-6666-6666'
    }
    // '妻夫木聡', 
    // '東京都港区', 
    // '03-3333-3333'
]
</script>

<template>
    <div v-for="shipping in shippings" :key="'id'" class=" flex">
        <div  class="bg-gray-100">
            <div>
                <p>{{ shipping.name }}</p>
                <p>{{ shipping.address }}</p>
                <p>{{ shipping.phonenumber }}</p>
            </div>
            <div class="mr-0 ml-auto mt-10">
                <button class="bg-blue-300 rounded-md mr-3">編集</button>
                <button class="bg-red-300 rounded-md">削除</button>
            </div>
        </div>
    </div>
</template>