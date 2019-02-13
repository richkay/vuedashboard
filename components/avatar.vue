<template>
    <div class="thumb float-right el-dropdown-link">
        <img 
            :src="imgs" 
            class="rounded-circle">
        <div class="profile">
            <div class="name">{{ bname }}</div>
            <div class="role">{{ brole }}</div>
        </div>
        <div class="clear" />
    </div>
</template>

<script>
export default {
    name: 'avatar',
    props: {
        imgs: {
            type: String,
            required: true
        },
        bname: {
            type: String
        },
        brole: {
            type: String
        }
    }
}
</script>
<style lang="scss" scoped>
.thumb {
    position: relative;
    text-align: left;
    cursor: pointer;
    .profile {
        line-height: 16px;
        margin-top :5px;
        .name {
            color: #ffc247;
            height:16px;
            overflow: hidden;
        }
        .role {
            font-size: 10px;
            height:16px;
            overflow: hidden;
        }
    }
}
.thumb img {
    height: auto;
    max-width: 100%;
    vertical-align: top;
    margin-right: 10px;
    float: left!important;
}
.float-right {
    float: right!important;
}
.thumb {
    top:10px;
    width: 120px;
    height: 44px;
}

.rounded-circle {
    width: 44px;
    border-radius: 50%!important;
}

img, svg {
    vertical-align: middle;
}
img {
    border-style: none;
}
</style>


