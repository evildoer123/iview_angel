
<template>
    <div class="layout">
        <Layout>
            <Header>
                <Menu mode="horizontal" theme="dark" active-name="1">
                    <div class="layout-logo"><img src="../static/img/logo.svg" class="logo" alt=""> <span class="logo1">天使办公</span></div>
                    <div class="layout-nav">
                        <MenuItem name="1">
                            <Icon type="ios-navigate"></Icon>
                            Item 1
                        </MenuItem>
                        <MenuItem name="2">
                            <Icon type="ios-keypad"></Icon>
                            Item 2
                        </MenuItem>
                    </div>
                </Menu>
            </Header>
            <Layout>
                <Sider  hide-trigger :style="{background: '#495060'}">
                    <Menu active-name="1-2" theme="dark" width="auto" :open-names="['1']">
                        <Submenu name="1">
                            <template slot="title">
                                <Icon type="ios-navigate"></Icon>
                               科室管理
                            </template>
                            <MenuItem name="1-1">Option 1</MenuItem>
                            <MenuItem name="1-2">Option 2</MenuItem>
                            <MenuItem name="1-3">Option 3</MenuItem>
                        </Submenu>
                        <Submenu name="2">
                            <template slot="title">
                                <Icon type="ios-keypad"></Icon>
                              科室管理
                            </template>
                            <MenuItem name="2-1">Option 1</MenuItem>
                            <MenuItem name="2-2">Option 2</MenuItem>
                        </Submenu>
                        <Submenu name="3">
                            <template slot="title">
                                <Icon type="ios-analytics"></Icon>
                               排班管理
                            </template>
                            <MenuItem name="3-1">Option 1</MenuItem>
                            <MenuItem name="3-2">Option 2</MenuItem>
                        </Submenu>
                    </Menu>
                </Sider>
                <Layout :style="{padding: '0 24px 24px'}">
                    <Breadcrumb :style="{margin: '24px 0'}">
                        <BreadcrumbItem>Home</BreadcrumbItem>
                        <BreadcrumbItem>Components</BreadcrumbItem>
                        <BreadcrumbItem>Layout</BreadcrumbItem>
                    </Breadcrumb>
                    <Content :style="{padding: '24px', minHeight: '800px', background: '#fff'}">
                        Content
                    </Content>
                </Layout>
            </Layout>
        </Layout>
    </div>
</template>
<script>
    export default {

    }
</script>
<style scoped lang="sass">
.layout
    background: #f5f7f9
    position: relative
    overflow: hidden
    vertical-align: middle
    .logo1
        color: #009688
        margin-left: 5px
    .logo
        height: 18px
    .layout-logo
        width: 100px
        height: 30px
        line-height: 30px
        border-radius: 3px
        float: left
        display: flex
        justify-content: center
        align-items: center
        position: relative
        top: 15px
        left: 0
    .layout-nav
        width: 420px
        margin: 0 auto
        margin-right: 20px


</style>
