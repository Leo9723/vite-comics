<script>
export default {
    data(){
        return {
            HeaderList: [
              {
                  item: 'CHARACTERS',
                  url: '#',
                  active: false
              },
              {
                  item: 'COMIC',
                  url: '#',
                  active: false
              },
              {
                  item: 'MOVIE',
                  url: '#',
                  active: true
              },
              {
                  item: 'TV',
                  url: '#',
                  active: false
              },
              {
                  item: 'GAMES',
                  url: '#',
                  active: false
              },
              {
                  item: 'COLLECTIBLES',
                  url: '#',
                  active: false
              },
              {
                  item: 'VIDEOS',
                  url: '#',
                  active: false
              },
              {
                  item: 'FANS',
                  url: '#',
                  active: false
              },
              {
                  item: 'NEWS',
                  url: '#',
                  active: false
              },
              {
                  item: 'SHOP',
                  url: '#',
                  active: false
              }
            ],
              methods: {
                ChangeActive() {
                    if(this.items.active == true){
                        this.items.active = false
                    }
                    else{
                        this.items.active = true
                    }
                } 
              },
    }
    }
}
</script>
<template lang="">
  <div class="container">
    <img src="/public/img/favicon.ico" alt="">
    <ul>
        <li v-for="(items, index) in HeaderList">
            <a href="" @click="ChangeActive()" :key="index" :class="items.active ? 'active' : ''">{{ items.item }}</a>
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
                padding-bottom: 24px;
                &.active, &:hover{
                    color: variables.$link-text;
                    border-bottom: 3px solid variables.$link-text;
                }
            }
        }
    }
}
</style>
