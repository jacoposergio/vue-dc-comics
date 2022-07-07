<template>
   <main>
    <div class="site-menu">
        <ul>
            <li v-for="link, index in menuLinks" :key="index">
                <div class="menu-img">
                    <img :src= "require(`../assets/img/${link.img}`)" :alt="`pic di ${link.text}`">
                </div>
                <div class="menu-text">
                    <p>{{link.text}}</p>
                </div>
            </li>
        </ul>
    </div>
   </main>
</template>

<script>
export default {
    name: 'PageMain',
         data() {
        return {
            menuLinks: [
                {
                    text: 'DIGITAL COMICS',
                    img: 'buy-comics-digital-comics.png',
                    current: false
                },
                {
                    text: 'DC MERCHANDISE',
                    img: 'buy-comics-merchandise.png',
                    current: true
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: 'buy-comics-shop-locator.png',
                    current: false
                },
                {
                    text: 'SUBSCRIPTIONS',
                    img: 'buy-comics-subscriptions.png',
                    current: false
                },
                {
                    text: 'DC POWER VISA',
                    img: 'buy-dc-power-visa.svg',
                    current: false
                }
            ],
        };
     }
}
</script>

<style lang="scss" scoped>
  @import '../style/variables.scss';

  main{
     background-color: $brand_main_color;
  
    
     .site-menu{
          margin: 0 auto;
          width: 70%;
     
        ul{
                display: flex;
                justify-content: space-between;
                align-items: center;
                padding: 2rem 3rem;
            li{
                display: flex;
                align-items: center;
                color: white;
                width: 150px;
                margin-right: 3rem;

                    .menu-img{
                        width: 40px;
                    }

                    .menu-text{
                        width: calc((100%/5)*3);
                        font-size: 0.7rem;
                        margin-left: 1rem;
                    }
              }
        }
     }
  }
</style>
