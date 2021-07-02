<template>
    <div class="page-changeCity">
        <el-row>
            <province />
        </el-row>
        <el-row>
            <hot title="热门城市：" :list="hotList" />
        </el-row>
        <el-row>
            <hot title="最近访问：" :list="recentList" />
        </el-row>
        <el-row>
            <category />
        </el-row>
    </div>
</template>

<script>
import Province from '@/components/changeCity/province.vue'
import hot from '@/components/changeCity/hot.vue'
import Category from '@/components/changeCity/category.vue'
export default {
  data () {
    return {
      hotList: ['北京', '上海', '广州', '深圳'],
      recentList: ['北京', '上海', '广州', '深圳', '太原']
    }
  },
  components: {
    Province,
    hot,
    Category
  }
}
</script>
