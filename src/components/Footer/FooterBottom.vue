<template>
  <section class="footer-bottom">
      <div class="container">
          <div class="footer-left">
              <button class="btn">Sign-up now!</button>
          </div>
          <div class="footer-right">
              <nav>
                  <ul class="social-links">
                      <li><h3>Follow us</h3></li>
                      <li><a href="#"><img src="../../assets/img/footer-facebook.png" alt=""></a></li>
                      <li><a href="#"><img src="../../assets/img/footer-twitter.png" alt=""></a></li>
                      <li><a href="#"><img src="../../assets/img/footer-youtube.png" alt=""></a></li>
                      <li><a href="#"><img src="../../assets/img/footer-pinterest.png" alt=""></a></li>
                  </ul>
              </nav>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'FooterBottom'
}
</script>

<style lang="scss">
@import '../../assets/style/mixins.scss';
    .footer-bottom{
        background-color: var(--footer-bottom-bg-color);
        padding: 1.25rem 0;

        & .container{
            display: flex;
            justify-content: space-between;
            align-items: center
        }
    }

    .social-links{
        @include listStyle;
        align-items: center;
        gap: 1.25rem;

        & h3{
            text-transform: uppercase;
            color: var(--primary-color);
        }
    }

</style>