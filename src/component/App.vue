<template>
    <!-- The overlay -->
    <div id="myNav" class="overlay">
      <!-- Overlay content -->
      <div class="overlay-modal">
        <div class="modal-contents">
          <label>Hadoop & Eco System</label>
          <div class="modal-list">
            <a href="#"><font size=4rem; color="white">· MIDAS Ambari</font></a>
            <a href="#"><font size=4rem; color="white">· MEDUS Ambari</font></a>
            <a href="#"><font size=4rem; color="white">· MALTHAEL Ambari</font></a>
          </div>
        </div>

        <div class="modal-contents">
          <label>BI</label>
        </div>

        <div class="modal-contents">
          <label>Elastic Search</label>
        </div>

        <div class="modal-contents">
          <label>Kibana</label>
        </div>

        <div class="modal-contents">
          <label>Etc</label>
        </div>

        <!-- Button to close the overlay navigation -->
        <a href="javascript:void(0)" class="closebtn" v-on:click="closeNav()" align="right">&times;</a>
      </div>
    </div>
    <span v-on:click="openNav()"> #전체보기 </span>

    <div id="header_custom">
        <h1 id="header_h1"> Zumvigator </h1>
    </div>
    <input type="text" v-model="input" placeholder="Search..."/>

    <div id="footer_custom">
        Copyright ⓒ Kang Hyunwoo
    </div>
</template>

<script setup>
  import { ref } from "vue";
  let input = ref("");

  function openNav() {
    document.getElementById("myNav").style.width = "100%";
  }

  function closeNav() {
    document.getElementById("myNav").style.width = "0%";
  }
</script>

<style src="../style/custom_style.css" />
