<script>
export default {
    data(){
        return {
            HeaderList: [
              {
                  item: 'CHARACTERS',
                  url: '#'
              },
              {
                  item: 'COMIC',
                  url: '#'
              },
              {
                  item: 'MOVIE',
                  url: '#'
              },
              {
                  item: 'TV',
                  url: '#'
              },
              {
                  item: 'GAMES',
                  url: '#'
              },
              {
                  item: 'COLLECTIBLES',
                  url: '#'
              },
              {
                  item: 'VIDEOS',
                  url: '#'
              },
              {
                  item: 'FANS',
                  url: '#'
              },
              {
                  item: 'NEWS',
                  url: '#'
              },
              {
                  item: 'SHOP',
                  url: '#'
              }
            ]

    }
    }
}
</script>
<template lang="">
  <div class="container">
    <img src="/public/img/favicon.ico" alt="">
    <ul>
        <li v-for="(items, index) in HeaderList">
            <a href="">{{ items.item }}</a>
        </li>
    </ul>
  </div>
</template>
<style lang="scss">
  @use '../components/styles/partials/variables';

.container {
    display: flex;
    width: 70%;
    margin: 0 auto;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0px;
    ul {
        display: flex;
        li {
            list-style-type: none;
            a {
                text-decoration: none;
                color: black;
                margin-left: 20px;
                padding-bottom: 30px;
                &:hover{
                    color: variables.$link-text;
                }
            }
        }
    }
}
</style>
