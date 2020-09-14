<template>
  <div class="about">
    <h1>{{msg}}</h1>
  </div>
</template>

<script>
export default {
    data(){
        return {
            msg: 'Vue生命周期'
        }
    },
    beforeCreate(){
        console.group('-------beforeCreated创建前状态-------');
        console.log("%c%s", "coler:red", "el    :" + this.$el);
        console.log("%c%s", "coler:red", "data  :" + this.$data);
        console.log("%c%s", "coler:red", "msg   :" + this.msg);
    },
    created(){
        console.group('-------Created创建完毕状态-------');
        console.log("%c%s", "coler:red", "el    :" + this.$el);
        console.log("%c%s", "coler:red", "data  :" + this.$data);
        console.log("%c%s", "coler:red", "msg   :" + this.msg);
    },
    beforeMount(){
        console.group('-------beforeMount挂载前状态-------');
        console.log("%c%s", "coler:red", "el    :" + this.$el);
        console.log(this.$el);
        console.log("%c%s", "coler:red", "data  :" + this.$data);
        console.log("%c%s", "coler:red", "msg   :" + this.msg);
    },
    mounted(){
        console.group('-------mount挂载结束状态-------');
        console.log("%c%s", "coler:red", "el    :" + this.$el);
        console.log(this.$el);
        console.log("%c%s", "coler:red", "data  :" + this.$data);
        console.log("%c%s", "coler:red", "msg   :" + this.msg);
    },
    beforeUpdate(){
        console.group('-------beforeUpdate更新前状态-------');
        console.log("%c%s", "coler:red", "el    :" + this.$el);
        console.log(this.$el);
        console.log("%c%s", "coler:red", "data  :" + this.$data);
        console.log("%c%s", "coler:red", "msg   :" + this.msg);
    },
    updated(){
        console.group('-------updated更新完成状态-------');
        console.log("%c%s", "coler:red", "el    :" + this.$el);
        console.log(this.$el);
        console.log("%c%s", "coler:red", "data  :" + this.$data);
        console.log("%c%s", "coler:red", "msg   :" + this.msg);
    },
    beforeDestroy(){
        console.group('-------beforeDestroy销毁前状态-------');
        console.log("%c%s", "coler:red", "el    :" + this.$el);
        console.log(this.$el);
        console.log("%c%s", "coler:red", "data  :" + this.$data);
        console.log("%c%s", "coler:red", "msg   :" + this.msg);
    },
    destroyed(){
        console.group('-------destroyed销毁完成状态-------');
        console.log("%c%s", "coler:red", "el    :" + this.$el);
        console.log(this.$el);
        console.log("%c%s", "coler:red", "data  :" + this.$data);
        console.log("%c%s", "coler:red", "msg   :" + this.msg);
    }
}
</script>