<template>
  <div class="reg">
    <div
      class="reg-header header-filter clear-filter purple-filter"
      data-parallax="true"
      style="background-image: url('./assets/img/bg2.jpg');"
    >
      <div class="container">
        <div class="card card-nav-tabs role-card">
          <div class="card-header card-header-primary">
            <RoleSelection />
          </div>
          <div class="card-body">
            <Role/>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import RoleSelection from '@/components/Reg/RoleSelection.vue'
import Role from '@/components/Reg/Role.vue'

export default {
  name: 'reg',
  components: {
    Role,
    RoleSelection
  }
}
</script>

<style lang="scss">
.reg-header {
  display: flex;
  align-items: center;
}
#RoleSelection {
  justify-content: center;
}
.role-card{
  margin-top: 200px;
  margin-bottom: 100px;
  .card-header {
  width: fit-content;
  align-self: center;
  }
}

@media only screen and (max-width: 768px) {
  .role-card{
    margin-top: 150px;
  }
}
</style>
