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

    </div>
  </div>
</template>
<style lang="scss">
  .info {
    background-color: blue;
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
    display: flex;
    justify-content: space-around;
    div {
      width: 40%;
      display: flex;
      flex-direction: column;
      flex-wrap: wrap;
      height: 350px;
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
      background-size: cover;
      height: 350px;
    }
  }
</style>
