<template>
  <div>
    <product-list :product-list-data="listData"/>
  </div>
</template>

<script >
import ProductList from '@/components'

export default {
  name: 'App',
 
  components: {
    ProductList,
  },

  data() {
    return {
      listData: [
        {
          id: 1,
          imgSrc:
            "https://img.freepik.com/free-vector/instagram-icon_1057-2227.jpg?w=2000",
          title: 'Instagram',
          
        },
        {
          id: 2,
          imgSrc:
            'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ8dN00swetq7b8RZ0lPAmKyr94Op-a83czCQ5ljWkBL_4WjnreJWbrjd0T-5pfLj6wuwE&usqp=CAU',
          title: 'Telegram',
          
        },
        {
          id: 3,
          imgSrc:
            'https://t3.ftcdn.net/jpg/04/74/05/94/360_F_474059464_qldYuzxaUWEwNTtYBJ44VN89ARuFktHW.jpg',
          title: 'YouTube',
          
        },
        {
          id: 4,
          imgSrc:
            "https://img.freepik.com/free-vector/instagram-icon_1057-2227.jpg?w=2000",
          title: 'Instagram',
          
        },
      ],
    }
  },
}
</script>

<style >
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>