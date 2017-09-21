<template>
<ul id="demo">
  <item
    class="item"
    :model="treeData">
  </item>
  <p>您好，仅供个人测试，无真实内容，勿随意传播</p>
</ul>
</template>

<script>
/* eslint-disable */

import item from '@/components/Item';

export default {
    name: 'index',
    data() {
        return {
            treeData: {
                name: '学生统一平台',
                children: [
                    { name: '报考四六级' },
                    { name: '本科生考试' },
                    {
                        name: '期末成绩',
                        children: [{
                                name: '本学期成绩',
                                children: [
                                    { name: '重修' },
                                    { name: '补考通知' }
                                ]
                            },
                            { name: '学分绩点' },
                            { name: '培养计划' },
                            {
                                name: '你的大学进度',
                                children: [
                                    { name: '已完成' },
                                    { name: '未完成' }
                                ]
                            }
                        ]
                    }
                ]
            }
        };
    },
    components: { item },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
