<template>
  <div id="profile">
    <!-- 导航栏 -->
    <nav-bar class="profile_navbar">
      <template #center>
        我的信息
      </template>
    </nav-bar>
    <!-- 基本信息 -->
    <profile-base-info />
    <!-- 信息列表 -->
    <profile-list />
  </div>
</template>

<script>
import NavBar from "components/common/navbar/NavBar.vue";

import ProfileBaseInfo from "./childComponents/ProfileBaseInfo.vue";
import ProfileList from "./childComponents/ProfileList.vue";

export default {
  name: "Profile",
  components: {
    NavBar,
    ProfileBaseInfo,
    ProfileList
  }
};
</script>

<style>
.profile_navbar {
  background-color: #ff5677;
  color: white;
}
</style>
