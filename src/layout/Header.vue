<template>
    <header class="header">
        <div class="container">
            <a class="logo">
                <img
                    class="img-logo"
                    src="../assets/header/titleLogo.svg"
                    alt="稀土掘金"
                    srcset=""
                />
                <img
                    class="mobile"
                    src="../assets/header/logo.svg"
                    alt="稀土掘金"
                    srcset=""
                />
            </a>
            <nav class="main-nav">
                <div class="nav-list">
                    <div class="main-nav-list">
                        <ul>
                            <li class="active-li"><a href="">首页</a></li>
                            <li><a href="">沸点</a></li>
                            <li><a href="">课程</a></li>
                            <li><a href="">咨询</a></li>
                            <li><a href="">活动</a></li>
                            <li><a href="">开放社区</a></li>
                        </ul>
                    </div>
                    <div class="right-side-nav">
                        <div class="search-add">
                            <div class="search">
                                <input type="text" />
                            </div>
                            <div class="add">
                                <button>创作者中心</button>
                            </div>
                        </div>
                        <div class="nav-item auth">
                            <button>登陆</button>
                        </div>
                    </div>
                </div>
            </nav>
        </div>
    </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "Header",
    setup() {
        return {};
    },
});
</script>

<style lang="less" scoped>
header {
    width: 100%;
    height: 60px;
    background: #fff;
    color: #909090;
    border-bottom: 1px solid #ccc;
    .container {
        display: flex;
        align-items: center;
        height: 100%;
        margin: 0 2rem;
        .logo {
            .mobile {
                display: none;
            }
        }
        .main-nav {
            flex: 1;
            height: 100%;
            .nav-list {
                display: flex;
                align-items: center;
                justify-content: space-between;
                height: 100%;
                margin: 0;
                ul {
                    display: flex;
                    li {
                        font-size: 15px;
                        color: #252933;
                        cursor: pointer;
                        a {
                            margin: 0 16px;
                        }
                    }
                    .active-li {
                        color: #1e80ff;
                        font-weight: 500;
                    }
                }
            }
        }
        .right-side-nav {
            display: flex;
            align-items: center;
            justify-content: center;
            .search-add {
                display: flex;
            }
        }
    }
}
</style>
