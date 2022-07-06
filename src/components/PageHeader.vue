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
        padding: 0.5rem 2rem;
        display: flex;
        justify-content: space-between;
        background-color: white;
        align-items: center;

        .logo{
            margin-right: 100px;
            img{
                width: 50px;
             }
        }
        nav{
            ul{
                display: flex;
                li{
                    margin-right: 1rem;
                    font-size: 0.6rem;
                }
            }
        }
    }
 }
</style>