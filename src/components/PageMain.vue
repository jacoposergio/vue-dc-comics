<template>
   <main>
    <div class="content-go-here">
        <h2>Content goes here</h2>
    </div>
    <div class="site-menu">
        <ul>
            <li>
                <div class="menu-img">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                </div>
                <div class="menu-text">
                    <h3>DIGITAL COMICS</h3>
                </div>
            </li>
        </ul>
    </div>
   </main>
</template>

<script>
export default {
    name: 'PageMain'
}
</script>

<style lang="scss" scoped>
  @import '../style/variables.scss';

  main{
        .content-go-here{
            padding: 3rem;
            background-color: black;
            color: white;
            font-size: 0.8rem;
        }
        
        ul{
            background-color: $brand_main_color;
            li{
                display: flex;
                align-items: center;
            }
        }
  }
</style>
