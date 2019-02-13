<template>
    <div class="header">
        <div class="left">Left</div>
        <div class="right">
            <badge icons="bell" btext="12" bclass="mr-r-15"/>
            <badge icons="envelope" btext="12" bclass="mr-r-20"/>
            <el-dropdown trigger="click">
                <avatar 
                    :imgs="profile.img" 
                    :bname="profile.name" 
                    :brole="profile.role" />
                <el-dropdown-menu slot="dropdown">
                    <el-dropdown-item>
                        <fa :icon="['fas', 'user']" class="mr-r-5"/>
                        My Account
                    </el-dropdown-item>
                    <el-dropdown-item><hr></el-dropdown-item>
                    <el-dropdown-item>
                        <fa :icon="['fas', 'book']" class="mr-r-5"/>
                        Note
                    </el-dropdown-item>
                    <el-dropdown-item>
                        <fa :icon="['fas', 'tasks']" class="mr-r-5"/>
                        Task
                    </el-dropdown-item>
                    <el-dropdown-item>
                        <fa :icon="['fas', 'cogs']" class="mr-r-5"/>
                        Setting
                    </el-dropdown-item>
                    <el-dropdown-item><hr></el-dropdown-item>
                    <el-dropdown-item>
                        <fa :icon="['fas', 'sign-out-alt']" class="mr-r-5"/>
                        Log Out
                    </el-dropdown-item>
                </el-dropdown-menu>
            </el-dropdown>
        </div>
        <div class="clear" />
    </div>
</template>

<script>

import badge from '../badge'
import avatar from '../avatar'

export default {
    name: 'comheader',
    components: {
        badge,
        avatar
    },
    data() {
        return {
            profile: {
                name: 'Amanda sfassf',
                role: 'Administrator',
                img: 'avatar/user.jpg'
            }
        }
    },
}
</script>

<style lang="scss" scoped>
.left {
    min-width: 10%;
    text-align: left;
    float: left;
}
.right {
    text-align: right;
}
</style>


