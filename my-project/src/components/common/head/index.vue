<template>
    <div :class="$style.header">
        <ul>
            <li :class="$style.navlist+' '+$style.navfirst">
                <router-link :to="'task'">TDList</router-link>
            </li>
            <li :class="$style.navlist">
                <router-link :to="'task'">task</router-link>
            </li>
            <li :class="$style.navlist">
                <router-link :to="'taskList'">tasklist</router-link>
            </li>
            <li :class="$style.navlist">
                <router-link :to="'willTask'">willTask</router-link>
            </li>
            <li :class="$style.navlistright">
                <router-link :to="'Login'">login</router-link>
            </li>
            <li :class="$style.navlistright">
                <router-link :to="'Resign'">resign</router-link>
            </li>
            <li :class="$style.clear"></li>
        </ul>
    </div>
</template>

<script>

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" module>
    .header{
        width: 100%;
        min-width: 1200px;
        background: #26a69a;
    }
    ul .navlist{
        float: left;
        margin-bottom:-1px;
        height:100%;
    }


    ul .navlistright{
       float: right;
    }
    .navfirst{
        font-weight: bolder;
        font-size: 16px;
    }
    ul .navlist a{
        display: inline-block;
        padding: 12px 20px;
        color:#fefefe;
    }

    ul .navlist:hover{
      border-bottom:2px solid #ffeb3b;
    }
    ul .navfirst:hover{
      border-bottom: none;
    }

    ul .navlistright a{
        display: inline-block;
        padding: 12px 20px;
        color:#fff;
    }

    .clear{
        clear:both;
    }

</style>
