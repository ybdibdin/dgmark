<template>
  <div>
    <h2 style="color: #025cc3;position: absolute;margin:-5.89vh 0 0 1.04vw" >DGNet</h2>
    <div id="top">

      <div id="left">
        <div class="nav"><div style="transform: scale(0.6);line-height: 90%;"><span></span>数据采集源统计</div></div>
        <div class="navcontent">
          <div class="detail">
            <div class="detailnav" style="background-color: #d5b100;"><div class="navfont">总数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{collectcount.today.allcount||'no data'}}</span>
                <span class="littlenum">{{collectcount.weekly.allcount||'no data'}}</span>
                <span class="littlenum">{{collectcount.monthly.allcount||'no data'}}</span>
              </div>
            </div>
          </div>
          <div class="detail">
            <div class="detailnav" style="background-color: #d44144;"><div class="navfont">重庆产品数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{collectcount.today.chongqing||'no data'}}</span>
                <span class="littlenum">{{collectcount.weekly.chongqing||'no data'}}</span>
                <span class="littlenum">{{collectcount.monthly.chongqing||'no data'}}</span>
              </div>
            </div>
          </div>
          <div class="detail">
            <div class="detailnav" style="background-color: #57c269;"><div class="navfont">人人网数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{collectcount.today.renren||'no data'}}</span>
                <span class="littlenum">{{collectcount.weekly.renren||'no data'}}</span>
                <span class="littlenum">{{collectcount.monthly.renren||'no data'}}</span>
              </div>
            </div>
          </div>
          <div class="detail">
            <div class="detailnav" style="background-color: #6648ff;"><div class="navfont">世纪佳缘数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{collectcount.today.sjjy||'no data'}}</span>
                <span class="littlenum">{{collectcount.weekly.sjjy||'no data'}}</span>
                <span class="littlenum">{{collectcount.monthly.sjjy||'no data'}}</span>
              </div>
            </div>
          </div>
          <div class="detail">
            <div class="detailnav" style="background-color: #fe6e00;"><div class="navfont">badoo数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{collectcount.today.badoo||'no data'}}</span>
                <span class="littlenum">{{collectcount.weekly.badoo||'no data'}}</span>
                <span class="littlenum">{{collectcount.monthly.badoo||'no data'}}</span>
              </div>
            </div>
          </div>
          <div class="detail">
            <div class="detailnav" style="background-color: #13a7d0;"><div class="navfont">公司内部数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{collectcount.today.internal||'no data'}}</span>
                <span class="littlenum">{{collectcount.weekly.internal||'no data'}}</span>
                <span class="littlenum">{{collectcount.monthly.internal||'no data'}}</span>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div id="right">
        <div class="nav"><div style="transform: scale(0.6);line-height: 90%;">入库量统计</div></div>
        <div class="navcontent">
          <div class="detail">
            <div class="detailnav" style="background-color: #d5b100;"><div class="navfont">总数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{washedcount.today.allcount||'no data'}}</span>
                <span class="littlenum">{{washedcount.weekly.allcount||'no data'}}</span>
                <span class="littlenum">{{washedcount.monthly.allcount||'no data'}}</span>
              </div>
            </div>
          </div>
          <div class="detail">
            <div class="detailnav" style="background-color: #d44144;"><div class="navfont">重庆产品数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{washedcount.today.chongqing||'no data'}}</span>
                <span class="littlenum">{{washedcount.weekly.chongqing||'no data'}}</span>
                <span class="littlenum">{{washedcount.monthly.chongqing||'no data'}}</span>
              </div>
            </div>
          </div>
          <div class="detail">
            <div class="detailnav" style="background-color: #57c269;"><div class="navfont">人人网数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{washedcount.today.renren||'no data'}}</span>
                <span class="littlenum">{{washedcount.weekly.renren||'no data'}}</span>
                <span class="littlenum">{{washedcount.monthly.renren||'no data'}}</span>
              </div>
            </div>
          </div>
          <div class="detail">
            <div class="detailnav" style="background-color: #6648ff;"><div class="navfont">世纪佳缘数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{washedcount.today.sjjy||'no data'}}</span>
                <span class="littlenum">{{washedcount.weekly.sjjy||'no data'}}</span>
                <span class="littlenum">{{washedcount.monthly.sjjy||'no data'}}</span>
              </div>
            </div>
          </div>
          <div class="detail">
            <div class="detailnav" style="background-color: #fe6e00;"><div class="navfont">badoo数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{washedcount.today.badoo||'no data'}}</span>
                <span class="littlenum">{{washedcount.weekly.badoo||'no data'}}</span>
                <span class="littlenum">{{washedcount.monthly.badoo||'no data'}}</span>
              </div>
            </div>
          </div>
          <div class="detail">
            <div class="detailnav" style="background-color: #13a7d0;"><div class="navfont">公司内部数据</div></div>
            <div class="detailcontent">
              <div class="detailcontentleft">
                <span class="littlefont">本日</span>
                <span class="littlefont">本周</span>
                <span class="littlefont">本月</span>
              </div>
              <div class="detailcontentright">
                <span class="littlenum">{{washedcount.today.internal||'no data'}}</span>
                <span class="littlenum">{{washedcount.weekly.internal||'no data'}}</span>
                <span class="littlenum">{{washedcount.monthly.internal||'no data'}}</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div id="bottom">
      <div class="nav"><div style="transform: scale(0.6);line-height: 90%;margin-left: -23%">聚类簇统计</div></div>
      <div class="bottomcontent">
        <div class="count">
          <div class="title" style="background-color: #d5b100;"><span style="transform: scale(0.65);">总数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">1,234,567,890</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">34567890</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
        <div class="count">
          <div class="title" style="background-color: #d44144;"><span style="transform: scale(0.65);white-space: nowrap;">重庆产品数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">1,234,567,890</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">34567890</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
        <div class="count">
          <div class="title" style="background-color: #57c269;"><span style="transform: scale(0.65);">人人网数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">1,234,567,890</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">34567890</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
        <div class="count">
          <div class="title" style="background-color: #6548ff;"><span style="transform: scale(0.65);white-space: nowrap;">世纪佳缘网数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">1,234,567,890</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">34567890</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
        <div class="count">
          <div class="title" style="background-color: #fe6e00;"><span style="transform: scale(0.65);">badoo数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">1,234,567,890</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">34567890</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
        <div class="count">
          <div class="title" style="background-color: #13a7d0;"><span style="transform: scale(0.65);white-space: nowrap;">公司内部数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">1,234,567,890</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">34567890</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">4567890</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import {TweenLite} from "gsap";
export default {
  name: 'app',
  data(){
      return {
        collectcount :{
          "monthly": {
            "allcount":0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0,
          },
          "today": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0,
          },
          "weekly": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0
          }
        },
        washedcount :{
          "monthly": {
            "allcount":0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0,
          },
          "today": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0,
          },
          "weekly": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0
          }
        },
        }
      },
  created(){
      this.$http.get('http://192.168.1.107:5000/api/washedcount').then(response =>{
          console.log(response);
          this.washedcount=response.data;
      })
  },
  mounted(){
      let i=1;
    let test=setInterval(()=>{
        let gap=100;
        let time=10;
        let count=(gap*i)/time;
        //console.log(Math.round(gap*Math.sin((Math.PI/2)*(i/time))));
        this.washedcount.today.allcount=Math.round(gap*Math.sin((Math.PI/2)*(i++/time)));
        if(i==11){clearInterval(test)}
    },1000)
  }


}
</script>

<style scoped>

  #top{
    height: 18.58vh;
    width: 98.07vw;
    margin:6.86vh 0 0 1.04vw;
    display: flex;
    justify-content: space-between;

  }
  #left{
    width: 48.86vw;
    height: 18.58vh;
    background-color: #15283f;
  }
  #right{
    display: inline-block;
    width: 48.86vw;
    height: 18.58vh;
    background-color: #15283f;
  }
  #bottom{
    width: 98.07vw;
    height: 66.13vh;
    margin:1.99vh 0 0 1.04vw;
    background-color: #15283f;
  }
  .nav{
    height: 1.95vh;
    width: 100%;
    background-color: #0e2c4c;
    display: flex;

  }
  .navcontent{
    background-color: #14202f;
    width: 46.18vw;
    height: 14.5vh;
    margin: 1.11vh 0 0 1.3vw;
    display: flex;
    justify-content: space-between;
  }
  .detail{
    background-color: #13263f;
    height:100%;
    width: 6.98vw;
  }
  .bottomcontent{
    width: 95.36vw;
    height: 59.91vh;
    margin:1.53vh 0 0 1.35vw;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    background: -webkit-radial-gradient(#173555,#18375c,#163453,#14202f);
  }
  .count{
    background-color: #13263f;
    width: 100%;
    height: 7.55vh;
    display: flex;

  }
  .detailnav{
    width: 100%;
    height: 1.76vh;
    display: flex;
    align-items: center;
    justify-content: center;

  }
  .navfont{
    white-space: nowrap;
    transform: scale(0.6);
  }
  .detailcontent{
    margin: 1.67vh 0 0 0.47vw;
    display: flex;
    justify-content: space-between;
  }

  .title{
    width: 6.98vw;
    height:100%;
    display: flex;
    justify-content: center;
    align-items: center;

  }
  .detailcontentleft{
    height: 9.64vh;
    width: 1.05vw;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .littlefont{
    transform: scale(0.6);
    font-size: 80%;
    white-space: nowrap;
  }
  .detailcontentright{
    width: 5.05vw;
    height: 9.62vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .littlenum{
    transform: scale(0.7);
    font-size: 80%;
    white-space: nowrap;
    color: #0172f7;
    display: flex;
    justify-content: center;
  }
  .data{
    height: 100%;
    width: 88.46vw;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .datadetail{
    width: 12.5%;
    height: 4.54vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

  }
  .btnum{
    height:42.86%;
    color: #0077fd;
    font-size: 90%;
  }
  .bbpic{
    height: 57.14%;
    display: flex;
    align-items: center;
    font-size: 80%;
    transform: scale(0.6);
    margin-top: 5%;
    white-space: nowrap;
  }
  i{
    transform: scale(0.5);

  }
</style>
