<template>
  <div>
    <div class="course-top">
      <a href="">
        <div class="fanhui"></div>
      </a>
      <div class="c1">
        <a href=""><img src="../img/weixin.png" alt=""></a>
        <a href=""><img src="../img/pyq.png" alt=""></a>
        <a href=""><span>. . . </span></a>
      </div>
    </div>
    <div class="cimg">
      <img src="../img/1.jpg" alt="加载中" title="英式奶油司康">
    </div>
    <div class="bo1">
      <div class="tit">
        <span class="titl">
          英式奶油司康
        </span>
      </div>
      <div class="pic">
        <div class="pic-a">
          <div>8.6</div>
          <span>课程评价</span>
        </div>
        <div class="pic-b">
          <div><img src="../img/ic_kabao.png" alt=""></div>
          <span>课程配方</span>
        </div>
      </div>
      <div class="people">
        <img src="../img/people.jpg" alt=""> 
        <div>安芙手作</div>
        <pre>
          小厨说课堂讲师：angel
          Angel做菜的初衷，就是使用最新鲜、单纯的材料
          做出天然又美味的料理，分享给所爱之人
          让做菜是一种生活态度
          我们不需要端出最华丽的那一个，
          但我相信一定是最令人难忘、温暖的那一个

          法国保罗博古斯法式料理、甜点大师课程毕业
          泰国蓝带法式甜点、法式料理、欧式面包第一名毕业
          悉尼蓝带法式甜点、法式料理、厨房管理结业
          美国惠尔通烘焙学院毕业
          英國PME 协会，裱花、翻糖、糖花毕业
          泰国万迪烹饪艺术学院毕业
          厨师 讲师 菜谱设计师：
          台北多间餐厅 甜点师、西餐主厨、面包师
          台东良食计划 小农产品食谱设计师
          花田喜彘 猪肉 推广厨师
          台北家扶中心青少年料理 讲师
          富春手作料理私厨 讲师
          乐料理厨艺教室 讲师
          《天然果酱私房甜点》出版书作者
          《新手入门蛋糕全书》出版书作者
          韩国 KDFCA 豆沙糖花讲师
          韩国 GFDA 专业豆沙裱花讲师
          *每年500堂线下实体课讲师经验
        </pre>
      </div>
      <div>
        <van-button  class="guan"><img src="../img/guanzhu2.png" alt="">&nbsp;&nbsp;关注老师</van-button>
      </div>
      <div>
        <div class="ke">课程简介</div>
        <div>
          <van-swipe :loop="false" :width="350" class="s1">
            <van-swipe-item>
              <img src="../img/sikang.jpg" alt="">
            </van-swipe-item>
            <van-swipe-item>
              <img src="../img/sikang2.jpg" alt="">
            </van-swipe-item>
            <van-swipe-item>
              <img src="../img/sikang3.jpg" alt="">
            </van-swipe-item>
            <van-swipe-item>
              <img src="../img/sikang4.jpg" alt="">
            </van-swipe-item>
          </van-swipe>
        </div>
        <div class="jian">
          一口气轻松的准备好一个丰盛的下午茶，是每一个人都期盼的事情！本套课程就是会教你如何简单高效的完成下午茶点心集合！
        </div>
      </div>
      <div class="yao">
        <div class="ke">课程要点</div>
        <pre>
          1.制作三种不同风味的果酱
          2.如何熬煮焦糖
          3.果酱装瓶技巧以及如何能延长果酱保存期限
          4.基础奶油杯子蛋糕面糊
          5.粉油拌合法
          6.蛋白霜的打发以及混拌面糊的要点
        </pre>
      </div>
      <div class="yao">
        <div class="ke">适用人群</div>
        <pre>美食爱好者、烘焙爱好者、甜品店面、私房实体店主</pre>
      </div>
      <div class="yao">
        <div class="ke">课程难度</div>
        <van-rate v-model="value" disabled />
      </div>
      <div class="yao">
        <div class="ke">小贴士</div>
        <pre>观看过程中，如有疑问可以私信老师哦～</pre>
      </div>
      <div class="yao">
        <div class="ke">该老师的其他课程</div>
        <van-swipe :loop="false" :width="350" class="s1">
            <van-swipe-item>
              <img src="../img/sikang.jpg" alt="">
            </van-swipe-item>
            <van-swipe-item>
              <img src="../img/sikang2.jpg" alt="">
            </van-swipe-item>
            <van-swipe-item>
              <img src="../img/sikang3.jpg" alt="">
            </van-swipe-item>
            <van-swipe-item>
              <img src="../img/sikang4.jpg" alt="">
            </van-swipe-item>
          </van-swipe>
        <div>

        </div>
      </div>
      <div class="bai"></div>
      
    </div>
    <div class="vip">
        <van-button class="vip1">
          <div>购买课程&nbsp;¥18.00</div>
          <span>1800厨币可兑换</span>
        </van-button>
        <van-button class="vip2"  color="linear-gradient(to right,rgb(240, 218, 157),rgb(194, 158, 42))">
          <img src="../img/zuanshi.png" alt="">加入购物车
        </van-button>
      </div>
  </div> 
</template>

<script>
export default {
  data() {
    return {
      value:2,
      product:[],
      eid:1
    }
  },
  methods:{
      myload(){
      this.axios.get("course").then(result=>{
        console.log(result.data);
      })
    }
  }
}
</script>
<style>
  @import "./Course.css";
</style>