<template>
    <div class="post-box">
        <span class="post-views">{{ views }}</span>
        <h3 class="post-title">{{ title }}</h3>
        <span class="post-date">{{ date }}</span>
        <p class="post-content">{{ content }}</p>
        <div class="row">
            <div class="col-sm-6">
                <span class="post-author">{{ author }}</span>
            </div>
            <div class="col-sm-6 text-right">
                <span class="post-category">{{ category }}</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: ["views", "title", "date", "content", "author", "category"],
    name: "post"
};
</script>

<style lang="scss" scoped>
.post-box {
    padding: 20px;
    background-color: #fff;
    box-shadow: 0 0 10px #ddd;
    position: relative;
    text-align: left;
    margin-bottom: 20px;
    .post-views {
        position: absolute;
        top: 5px;
        right: 5px;
        background-color: #f00;
        border-radius: 4px;
        padding: 1px 5px;
        text-align: center;
        font-weight: bold;
    }
    .post-date {
        display: block;
        color: #818080;
        padding: 0 0 5px;
        font-size: 14px;
    }
    .post-content {
        line-height: 1.8;
        color: #666;
    }
    .post-author {
        background-color: #607d88;
        padding: 6px 10px;
        border-radius: 4px;
        color: #fff;
    }
    .post-category {
        background-color: #607d88;
        padding: 6px 10px;
        border-radius: 4px;
        color: #fff;
    }
}
</style>
