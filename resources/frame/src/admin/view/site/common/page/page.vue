<template>
    <div class="page-box">
      <el-pagination
        @current-change="handleCurrentChange"
        :current-page="currentPags"
        :page-size="pageSize"
        layout="total, prev, pager, next,jumper"
        :total="total">
      </el-pagination>
    </div>
</template>

<script>
import '../../../../scss/site/module/common/page/page.scss';
import pageCon from '../../../../controllers/site/common/page/pageCon';
export default {
    name: "page",
  ...pageCon
}
</script>
