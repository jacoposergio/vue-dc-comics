<template>
  <footer>
    <div class="footer-container">
        <div class="top-footer">
            <div class="footer-links">
                <ul>
                    <li></li>
                </ul>
            </div>
            <div class="footer-logo">
                <img src="../assets/img/dc-logo-bg.png" alt="dc-logo">
            </div>
        </div>
        <div class="bottom-footer">
            bottom
        </div>
    </div>
  </footer>
</template>

<script>
export default {
     name: 'PageFooter',

}

</script>

<style lang="scss" scoped>
  @import '../style/variables.scss';
 @import '../style/common.scss';

  footer{
    .footer-container{
        background-image: url(../assets/img/footer-bg.jpg);

        .top-footer{
          display: flex;    
          height: 300px;
          margin: 0 auto;
          width: 70%;
             
             .footer-links{
                 margin: 0 auto;
                 width: 70%;
                 width: 50%;
                 color: white;
             }
            .footer-logo{
               height: 100%;

                img{
                    height: 100%;
                }
            }
        }
    }
  }


</style>