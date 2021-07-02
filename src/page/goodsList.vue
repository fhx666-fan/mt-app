<template>
    <div class="page-product">
        <el-row class="m-crumbs">
            <crumbs />
        </el-row>
        <el-row>
            <el-col :span="19">
                <el-row>
                    <category />
                </el-row>
                <el-row>
                    <list />
                </el-row>
            </el-col>
            <el-col :span="5">
            </el-col>
        </el-row>
    </div>
</template>

<script>
import crumbs from '@/components/products/crumbs.vue'
import Category from '@/components/products/category.vue'
import List from '@/components/products/list.vue'
export default {
  components: {
    crumbs,
    Category,
    List
  }
}
</script>
<style lang="scss">
    @import '@/assets/css/products/index.scss';
</style>
