<template>
  <div>
    <b-navbar id="navbar" toggleable="lg" type="dark">
      <b-navbar-brand href="#">
        <img id="logo" src="../assets/img/backupPreview.png" alt="logo">
        Kimchi-Merken
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse" />

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="/index">
            Art
          </b-nav-item>
          <b-nav-item href="#">
            Food
          </b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-form-input
              size="sm"
              class="mr-sm-2"
              placeholder="Busca algo :)"
            />
            <b-button
              id="button"
              size="sm"
              class="my-2 my-sm-0"
              type="submit"
            >
              Buscar
            </b-button>
          </b-nav-form>

          <b-nav-item-dropdown text="Lang" right>
            <b-dropdown-item href="#">
              EN
            </b-dropdown-item>
            <b-dropdown-item href="#">
              ES
            </b-dropdown-item>
            <b-dropdown-item href="#">
              RU
            </b-dropdown-item>
            <b-dropdown-item href="#">
              FA
            </b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template #button-content>
              <em>Usuario</em>
            </template>
            <b-dropdown-item href="#">
              Perfil
            </b-dropdown-item>
            <b-dropdown-item href="#">
              Salir
            </b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/_variables.scss';

#logo {
  background-color: aqua;
  border-radius: 20px;
  width: 50px;
}

#button {
  background-color: #d20056;

}

#navbar{
  background-color: transparent;
}
</style>
