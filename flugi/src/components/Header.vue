<template>
  <div class="container">
    <div class="main-header">
      <div class="main-header__items">
        <h1>flugi.</h1>
        <ul>
          <li>Pacotes</li>
          <li>Promoções</li>
        </ul>
      </div>
      <div class="main-header__login">
        <img src="../assets/user-circle-black.svg" alt="User Icon Black">
        <a href="#">Entrar</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style lang="less" scoped>
@import "../assets/variables.less";

.container {
  margin-left: @margin-body-desktop;
  margin-right: @margin-body-desktop;
  
  .main-header {
    height: @height-menu-desktop;
    display: flex;
    align-items: center;
    justify-content: space-between;

    &__items {
      display: flex;
      flex-direction: row;
      align-items: center;
      flex-wrap: wrap;

      h1 {
        font-weight: bold;
        font-size: 32px;
        color: @orange;
        margin-right: 40px;
      }

      ul {
        display: flex;

        li {
          font-weight: bold;
          margin-right: 35px;
          color: @black;
        }
      }
    }

    &__login {
      display: flex;
      flex-direction: row;
      align-items: center;

      img {
        margin-right: 15px;
      }

      a {
        font-weight: bold;
        margin-right: 35px;
        color: @black;
      }
    }
  }

  @media (max-width: 768px) {
    margin-left: @margin-body-mobile;
    margin-right: @margin-body-mobile;

    .main-header {
      height: @height-menu-mobile;

      &__login {
        img {
          margin-right: unset;
        }

        a {
        display: none;
        }
      }
    }
  }

  @media (max-width: 376px) {
    .main-header {
      &__items {
        ul {
          margin-top: 18px;
        }
      }
    
      &__login {
        img {
          margin-bottom: 30px;
        }
      }
    }
  }
}
</style>