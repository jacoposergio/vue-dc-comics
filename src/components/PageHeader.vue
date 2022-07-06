<template>
  <header>
    <div class="header-container">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="dc logo">
       </div>
        <nav>
            <ul>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                  <li>
                    <a href="#">CHARACTERS</a>
                </li>
                  <li>
                    <a href="#">CHARACTERS</a>
                </li>
                  <li>
                    <a href="#">CHARACTERS</a>
                </li>
                  <li>
                    <a href="#">CHARACTERS</a>
                </li>
            </ul>
        </nav>    
    </div>
  </header>
</template>

<script>
export default {
    name: 'PageHeader'
}
</script>

<style lang="scss" scoped>
 header {

    .header-container{
        display: flex;
        justify-content: space-between;
        background-color: white;
        border: 1px solid black;

    }
    .logo{
        img{
            width: 50px;
        }
    }
 }
</style>