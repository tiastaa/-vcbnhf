<template>
    <div class="card-container">
        <div class="card-button">
            <button ><img src="https://apisproductions.com/wp-content/uploads/2020/02/istockphoto-957096060-170667a.jpg" alt=""></button>
        </div>
        
        <div class="card-image">
            <img :src="imgSrc" />
        </div>
        <div class="card-title">
            {{title}}
        </div>
    </div>
</template>

<script>
export default{
    name:'ProductCard',
    props:{
        imgSrc:{
            type: String,
            default: 'https://www.ukrtour.pro/images/gallery/hostel/22/karpatskie-zori-1.jpg'
        },
        title:{
            type: String,
            default: '. . .'
        }
    }
}
</script>

<style lang='css' scoped>
.card-container {
  width: 150px;
  height: 150px;
  border: 0px solid rgb(0, 0, 0);
  border-radius: 15px;
  margin: 20px;
  padding: 10px;
  background-color: rgb(219, 219, 219);
}

.card-container:hover{
margin-top: 15px;
}
.card-image img {
  margin-bottom: 10px;
  border-radius: 50%;
  width: 80px;
  height: 80px;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.card-button button {
    width: 40px;
    height: 40px;
    background-color: white;
    border: 0px solid black;
    border-radius: 50%;
    display: block;
  margin-left: auto;
    cursor: pointer;
    padding: 2px;
}
.card-button img {
    width: 100%;
    border-radius: 50%;
}
</style>