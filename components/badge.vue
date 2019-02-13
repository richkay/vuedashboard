<template>
    <span class="notif" :class="bclass">
        <fa :icon="['fas', icons]" class="cl-gray pointer" />
        <span class="text">{{ btext }}</span>
    </span>
</template>
<script>
export default {
    name:'badge',
    props: {
        icons: {
            type: String,
            required: false,
        },
        bclass: {
            type: String,
            required: false,
        },
        btext: {
            type: String,
            required: false,
        }
    }
}
</script>
<style lang="scss" scoped>
.svg-inline--fa {
    color:gray;
}
.notif {
   font-size: 18px;
   line-height: 18px;
   color:#fff;
   .text {
        font-size: 10px;
        background:rgb(245,93,93);
        border-radius: 50%;
        line-height: 10px;
        width: 20px;
        height: 20px;
        padding: 3px;
        top: -12px;
        right:5px;
        position: relative;
   }
}
</style>

