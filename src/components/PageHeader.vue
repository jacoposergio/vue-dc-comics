<template>
  <header>
    <div class="header-container">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="dc logo">
       </div>
        <nav>
            <ul>
                <li v-for="link, index in navLinks" :key="index">
                    <a href="#">{{link.text}}</a>
                </li>
            </ul>
        </nav>    
    </div>
  </header>
</template>

<script>
export default {
    name: 'PageHeader',
        data() {
        return {
            navLinks: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false
                },
                    {
                    text: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false
                }
            ],
        };
    }

}
</script>

<style lang="scss" scoped>
 header {
  background-color: white;

    .header-container{
        width: 70%;
        margin: 0 auto;
        padding: 0.5rem 2rem;
        display: flex;
        justify-content: space-between;
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
                    font-size: 0.8rem;
                }
            }
        }
    }
 }
</style>