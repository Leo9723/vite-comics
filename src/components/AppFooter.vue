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
</style>
