<script>
export default {
  data() {
    return {
      FooterInfo: [
        {
          logo: '/public/img/buy-comics-digital-comics.png',
          name: 'DIGITAL COMICS',
          url: ''
        },
        {
          logo: '/public/img/buy-comics-merchandise.png',
          name: 'DC MERCHANDISE',
          url: ''
        },
        {
          logo: '/public/img/buy-comics-subscriptions.png',
          name: 'SUBSCRIPTION',
          url: ''
        },
        {
          logo: '/public/img/buy-comics-shop-locator.png',
          name: 'COMIC SHOP LOCATOR',
          url: ''
        },
        {
          logo: '/public/img/buy-dc-power-visa.svg',
          name: 'DC POWER VISA',
          url: ''
        }
      ],
      FooterList: [
        {
          title: 'DC COMICS',
          Item: [
            'Characters',
            'Comics',
            'Movies',
            'TV',
            'Games',
            'Videos',
            'News'
          ]
        },
        {
          title: 'SHOP',
          Item: [
            'Shop DC',
            'Shop DC Collectibles'
          ]
        },
        {
          title: 'DC',
          Item: [
            'Terms Of Use',
            'Privacy policy (New)',
            'Ad Choices',
            'Advertising',
            'Jobs',
            'Subscriptions',
            'Talent Workshop',
            'CPSC Certificates',
            'Rating',
            'Shop Help',
            'Contact Us'
          ]
        },
        {
          title: 'SITES',
          Item: [
            'DC',
            'MAD Magazine',
            'DC Kids',
            'DC Universe',
            'DC Power Visa'
          ]
        }
      ]
    }
  }
}
</script>
<template lang="">
  <div>
    <div class="info">
      <ul>
        <li v-for="(items, index) in FooterInfo">
          <img :src="items.logo" alt="">
          <a href="">{{ items.name }}</a>
        </li>
      </ul>
    </div>
    <div class="links">
      <div>
      <ul v-for="(list, index) in FooterList">
        <span>{{ list.title }}</span>
        <li v-for="(itemlist, num) in FooterList[index].Item">
          {{ itemlist }}
        </li>
      </ul>
      </div>
      <div class="logo">
      </div>
    </div>
    <div class="media">
      <div class="mediacontainer">
      <div class="sign-up">
        <button>SIGN-UP</button>
      </div>
      <div class="socials">
        <div>
          FOLLOW US
        </div>
        <div>
          <img src="../../public/img/footer-facebook.png" alt="">
        </div>
        <div>
          <img src="../../public/img/footer-twitter.png" alt="">
        </div>
        <div>
          <img src="../../public/img/footer-youtube.png" alt="">
        </div>
        <div>
          <img src="../../public/img/footer-pinterest.png" alt="">
        </div>
        <div>
          <img src="../../public/img/footer-periscope.png" alt="">
        </div>
      </div>
      </div>
    </div>
  </div>
</template>
<style lang="scss">
  @use '../components/styles/partials/variables';

  .info {
    background-color: variables.$link-text;
    ul {
      display: flex;
      width: 70%;
      margin: 0 auto;
      justify-content: space-between;
      padding: 20px 0px;
      li {
        list-style-type: none;
        display: flex;
        align-items: center;
        img {
          height: 50px;
        }
        a {
          color: white;
          text-decoration: none;
          font-size: 15px;
          margin-left: 15px;
        }
      }
    }
  }
  .links {
    color: white;
    background-image: url(../../public/img/footer-bg.jpg);
    background-size: cover;
    display: flex;
    justify-content: space-around;
    div {
      width: 40%;
      display: flex;
      flex-direction: column;
      flex-wrap: wrap;
      height: 450px;
      padding: 30px;
      ul {
        margin-top: 20px;
        span {
          font-weight: bold;
        }
        li {
          list-style-type: none;
          font-size: small;
          margin: 5px 0px;
        }
      }
    }
    .logo {
      width: 30%;
      background-image: url(../../public/img/dc-logo-bg.png);
      background-position: right center;
      background-repeat: no-repeat;
      height: 450px;
    }
  }
  .media {
    background-color: rgb(55, 55, 55);
    padding: 30px 0px;
    .mediacontainer{
      width: 80%;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      .sign-up{
        align-self: center;
        margin-left: 20px;
        button {
          border: 2px solid variables.$link-text;
          padding: 10px 20px;
          background: none;
          color: white;
        }
      }
      .socials{
        display: flex;
        align-items: center;
        div {
          margin-right: 20px;
          color: variables.$link-text;
          font-size: 20px;
        }
      }
    }
  }
</style>
