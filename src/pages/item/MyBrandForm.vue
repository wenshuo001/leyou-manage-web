<v-form v-model="valid">
  <v-text-field v-model="brand.name" label="请输入品牌名称" required />
  <v-text-field v-model="brand.letter" label="请输入品牌首字母" required />
</v-form>
<script>

  export default {
    name: "my-brand-form",
    data() {
      return {
        valid:false, // 表单校验结果标记
        brand:{
          name:'', // 品牌名称
          letter:'', // 品牌首字母
          image:'',// 品牌logo
          categories:[], // 品牌所属的商品分类数组
        }
      }
    }
  }
</script>
