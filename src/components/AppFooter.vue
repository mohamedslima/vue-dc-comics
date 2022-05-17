<template>
  <footer class="footer">
    <div class="footer__info"></div>
    <div class="footer__links">
      <div class="footer__links_width">
        <div class="footer__links_left">
          <div>
            <h3>DC COMICS</h3>
            <ul>
              <li><a href="">Characters</a></li>
              <li><a href="">Comics</a></li>
              <li><a href="">Movies</a></li>
              <li><a href="">TV</a></li>
              <li><a href="">Games</a></li>
              <li><a href="">Videos</a></li>
              <li><a href="">News</a></li>
            </ul>
            <h3>SHOP</h3>
            <ul>
              <li>
                <a href="">Shop DC </a>
              </li>
              <li>
                <a href="">Shop DC Collectibles </a>
              </li>
            </ul>
          </div>
          <div>
            <h3>DC</h3>
            <ul>
              <li><a href="">Terms Of Use</a></li>
              <li><a href="">Privacy policy (new)</a></li>
              <li><a href="">Ad Choiches</a></li>
              <li><a href="">Advertising</a></li>
              <li><a href="">Jobs</a></li>
              <li><a href="">Subscriptions</a></li>
              <li><a href="">Talent Workshops</a></li>
              <li><a href="">CPSC Certificates</a></li>
              <li><a href="">Ratings</a></li>
              <li><a href="">Shop Help</a></li>
              <li><a href="">Contact Us</a></li>
            </ul>
          </div>
          <div>
            <h3>SITES</h3>
            <ul>
              <li><a href="">DC</a></li>
              <li><a href="">MAD Magazine</a></li>
              <li><a href="">DC Kids</a></li>
              <li><a href="">DC Universe</a></li>
              <li><a href="">DC Power Vita</a></li>
            </ul>
          </div>
        </div>
        <div class="footer__links_right">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.footer {
  &__info {
    height: 150px;
    background-color: blue;
  }
  &__links {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: 100%;
    padding: 1rem 0;
    div.footer__links_width {
      width: $general-width-page;
      margin: $general-center-page;
      display: flex;
      justify-content: space-between;
      div.footer__links_left {
        display: flex;
        h3 {
          color: white;
          margin: 0.8rem 0;
        }
        ul {
          li {
            list-style: none;
            margin: 0.5rem 1rem 0 0;
            a {
              text-decoration: $leave-decoration-text;
              color: gray;
            }
          }
        }
      }
      div.footer__links_right {
        img {
          width: 60%;
        }
      }
    }
  }
}
</style>
