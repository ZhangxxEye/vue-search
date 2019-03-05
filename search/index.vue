<template>
    <div class="search-field flex-box">
        <i class="search-icon"></i>
        <div class="search-input">
            <input type="search" @input="$emit('input', $event.target.value)"  :placeholder="placeholder" class="input-field"/>
        </div>
    </div>
</template>
<script>
    export default {
        props: {
            placeholder: {
                default: '请输入查询信息',
                type: String
            },
            value: {}
        }
    };
</script>
<style lang="less" scoped>
    .flex-box {
        display: flex;
    }

    .search-field {
        width: 100%;
        background: rgba(242, 242, 242, 1);
        border-radius: 34px;
        padding: 4px 8px;
        box-sizing: border-box;

        .search-icon {
            display: inline-block;
            width: 24px;
            height: 24px;
            background: url("./img/search.png") no-repeat;
            background-size: 100% 100%;
        }
        .search-input{
            flex: 1;
        }

        .input-field {
            width: 100%;
            font-size: 14px;
            font-weight: 400;
            color: rgba(153, 153, 153, 1);
            border: 0;
            background: transparent;
            box-sizing: border-box;
        }
    }
</style>
