<template>
  <div class="card-default movie-detail">
    <header>hahahahha</header>
    <div>
      <img src="" alt="">
      <ul class="detail">
        <li><span>原名：</span>haha</li>
        <li><span>地区：</span>haha</li>
        <li><span>年代：</span>haha</li>
        <li><span>类型：</span>haha</li>
        <li><span>又名：</span>haha</li>
        <li><span>导演：</span>haha</li>
        <li><span>主演：</span>haha</li>
        <li><span>豆瓣链接：</span><a class="link">hahah</a></li>
      </ul>
      <div class="score">
        <div class="number">
          <span>9.6</span>
          <icon-svg icon-class="liuamngxing" class="icon"></icon-svg>
        </div>
        <span>豆瓣评分</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MovieDetail',
  props: ['movie-detail'],
  data () {
    return {}
  }
}
</script>

<style lang="scss" scoped>
.movie-detail{
  width: 695px;
  > header{
    font-size: 26px;
  }
  > div{
    display: flex;
    justify-content: flex-start;
    align-items: stretch;
    > img{
      width: 139px;
      height: 207px;
      display: block;
      background-color: rgb(202, 200, 200);
    }
    .detail{
      font-size: 12px;
      color: #666;
      width: 263px;
      margin-left: 40px;
      > li{
        margin-bottom: 9px;
        &:last-child{
          margin-bottom: 0;
        }
        > span{
          color: #444;
          font-weight: bold;
        }
        .link{
          color: #f32941;
          text-decoration: underline;
          &:hover{
            font-weight: bold;
          }
        }
      }
    }
    .score{
      text-align: center;
      padding-top: 11px;
      flex: 1;
      display: flex;
      flex-direction: column;
      justify-content: flex-start;
      align-items: center;
      .number{
        width: 58px;
        height: 66px;
        position: relative;
        margin-bottom: 16px;
        >span{
          font-size: 24px;
          color: #fbe592;
          position: absolute;
          top: 50%;
          left: 50%;
          transform: translate(-50%, -50%);
        }
        .icon{
          width: 70px;
          height: 70px;
          color: #f43e54;
        }
      }
      >span{
        font-size: 12px;
        color: #444;
      }
    }
  }
}
</style>
