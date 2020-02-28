<template>
  <aside class="main-sidebar sidebar-dark-primary elevation-4">
    <!-- Brand Logo -->
    <a href="/" class="brand-link">
      <img src="/images/logo_admin.png" alt="AdminLTE Logo" class="">
    </a>
    <!-- Sidebar -->
    <div class="sidebar">
      <!-- Sidebar Menu -->
      <nav class="mt-2">
        <ul class="nav nav-pills nav-sidebar flex-column" data-widget="treeview" role="menu"
            data-accordion="false">
          <!-- Add icons to the links using the .nav-icon class
               with font-awesome or any other icon font library -->
          <li class="nav-item has-treeview menu-open">
            <a href="#" class="nav-link ">
              <p>
                予約管理
                <i class="right fas fa-angle-left"></i>
              </p>
            </a>
            <ul class="nav nav-treeview">
              <li class="nav-item">
                <a href="/"
                   class="nav-link ">
                  <p>予約依頼一覧</p>
                </a>
              </li>
              <li class="nav-item">
                <a href="/"
                   class="nav-link ">
                  <p>予約連絡・確定一覧</p>
                </a>
              </li>
              <li class="nav-item">
                <a href="/" class="nav-link">
                  <p>キャンセル一覧</p>
                </a>
              </li>
            </ul>
          </li>
          <li class="nav-item has-treeview menu-open">
            <a href="#" class="nav-link ">
              <p>
                患者管理
                <i class="right fas fa-angle-left"></i>
              </p>
            </a>
            <ul class="nav nav-treeview">
              <li class="nav-item">
                <a href="/"
                   class="nav-link ">
                  <p>患者一覧</p>
                </a>
              </li>
              <li class="nav-item">
                <a href="/"
                   class="nav-link ">
                  <p>患者CSV取り込み</p>
                </a>
              </li>
            </ul>
          </li>
          <li class="nav-item has-treeview menu-open">
            <a href="#" class="nav-link ">
              <p>
                マスタ管理
                <i class="right fas fa-angle-left"></i>
              </p>
            </a>
            <ul class="nav nav-treeview">
              <li class="nav-item">
                <a href="/"
                   class="nav-link ">
                  <p>管理者一覧</p>
                </a>
              </li>
              <li class="nav-item">
                <a href="/"
                   class="nav-link ">
                  <!--<i class="far fa-circle nav-icon"></i>-->
                  <p>症例紹介マスタ</p>
                </a>
              </li>
            </ul>
          </li>
        </ul>
      </nav>
    </div>

  </aside>
</template>

<script>
  export default {
    name: "Sidebar"
  }
</script>

<style scoped>

</style>
