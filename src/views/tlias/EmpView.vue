<template>
    <div>
        <el-container style="height: 700px; border: 1px solid #eee">
            <el-header style="font-size: 40px; background-color: rgb(238,241,246)">tlias</el-header>
            <el-container>
                <el-aside width="200px" style="background-color: rgb(238, 241, 246)">
                    <el-menu :default-openeds="['1', '3']">
                        <el-submenu index="1">
                            <template slot="title"><i class="el-icon-message"></i>Management</template>
                            <el-menu-item-group>
                                <el-menu-item index="1-1">DeptView</el-menu-item>
                                <el-menu-item index="1-2">EmpView</el-menu-item>
                            </el-menu-item-group>
                        </el-submenu>
                    </el-menu>

                </el-aside>
                <el-main>
                    <el-table :data="tableData">
                        <el-table-column prop="date" label="Date" width="140">
                        </el-table-column>
                        <el-table-column prop="name" label="Name" width="120">
                        </el-table-column>
                        <el-table-column prop="address" label="Address">
                        </el-table-column>
                    </el-table>
                </el-main>
            </el-container>
        </el-container>
    </div>
</template>

<script>
export default {

}
</script>

<style></style>