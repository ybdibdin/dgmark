<template>
  <div>
    <h2 style="color: #025cc3;position: absolute;margin:-3.5% 0 0 46%" >DGNet</h2>
    <div id="top">
      <div class="nav"><div style="transform: scale(0.6);line-height: 90%;">聚类簇统计</div></div>
      <div class="topcontent">
        <div class="count">
          <div class="title" style="background-color: #d5b100;"><span style="transform: scale(0.6);">总数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">{{clustercount.allsize.allcount||'no data'}}</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.zclustersize.allcount||'no data'}}</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclustersize.allcount||'no data'}}</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclustersize.allcount||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclustersize.allcount||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclusternum.allcount||'no data'}}</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclusternum.allcount||'no data'}}</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclusternum.allcount||'no data'}}</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
        <div class="count">
          <div class="title" style="background-color: #d44144;"><span style="transform: scale(0.6);white-space: nowrap;">重庆产品数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">{{clustercount.allsize.chongqing||'no data'}}</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.zclustersize.chongqing||'no data'}}</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclustersize.chongqing||'no data'}}</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclustersize.chongqing||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclustersize.chongqing||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclusternum.chongqing||'no data'}}</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclusternum.chongqing||'no data'}}</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclusternum.chongqing||'no data'}}</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
        <div class="count">
          <div class="title" style="background-color: #57c269;"><span style="transform: scale(0.6);">人人网数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">{{clustercount.allsize.renren||'no data'}}</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.zclustersize.renren||'no data'}}</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclustersize.renren||'no data'}}</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclustersize.renren||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclustersize.renren||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclusternum.renren||'no data'}}</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclusternum.renren||'no data'}}</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclusternum.renren||'no data'}}</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
        <div class="count">
          <div class="title" style="background-color: #6548ff;"><span style="transform: scale(0.6);white-space: nowrap;">世纪佳缘网数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">{{clustercount.allsize.sjjy||'no data'}}</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.zclustersize.sjjy||'no data'}}</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclustersize.sjjy||'no data'}}</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclustersize.sjjy||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclustersize.sjjy||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclusternum.sjjy||'no data'}}</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclusternum.sjjy||'no data'}}</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclusternum.sjjy||'no data'}}</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
        <div class="count">
          <div class="title" style="background-color: #fe6e00;"><span style="transform: scale(0.6);">badoo数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">{{clustercount.allsize.badoo||'no data'}}</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.zclustersize.badoo||'no data'}}</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclustersize.badoo||'no data'}}</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclustersize.badoo||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclustersize.badoo||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclusternum.badoo||'no data'}}</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclusternum.badoo||'no data'}}</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclusternum.badoo||'no data'}}</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
        <div class="count">
          <div class="title" style="background-color: #13a7d0;"><span style="transform: scale(0.6);white-space: nowrap;">公司内部数据</span></div>
          <div class="data">
            <div class="datadetail">
              <div class="btnum">{{clustercount.allsize.internal||'no data'}}</div>
              <div class="bbpic">总图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.zclustersize.internal||'no data'}}</div>
              <div class="bbpic">0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclustersize.internal||'no data'}}</div>
              <div class="bbpic">非0簇图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclustersize.internal||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数>10图片数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclustersize.internal||'no data'}}</div>
              <div class="bbpic">簇内单簇图片数<10</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.nzclusternum.internal||'no data'}}</div>
              <div class="bbpic">非0簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.bigclusternum.internal||'no data'}}</div>
              <div class="bbpic">簇内图片>10的簇数</div>
            </div>
            <div class="datadetail">
              <div class="btnum">{{clustercount.smallclusternum.internal||'no data'}}</div>
              <div class="bbpic">簇内图片<10的簇数</div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div id="bottom">
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
  </div>
</template>

<script>
  import {TweenLite} from "gsap";
  import icon1 from '../image/titleicon.png'
export default {
  name: 'app',
  data(){
      return {

        clustercount: {
          "allsize": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0
          },
          "bigclusternum": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0
          },
          "bigclustersize": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0
          },
          "nzclusternum": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0
          },
          "nzclustersize": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0
          },
          "smallclusternum": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0
          },
          "smallclustersize": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": 0,
            "internal": 0,
            "renren": 0,
            "sjjy": 0
          },
          "zclustersize": {
            "allcount": 0,
            "badoo": 0,
            "chongqing": null,
            "internal": null,
            "renren": 0,
            "sjjy": null
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
        }
        }
      },
  created(){

        this.$http.get('http://192.168.1.35:5000/api/washedcount').then(response =>{
          console.log(response);
          this.washedcount=response.data;
        }),
        this.$http.get('http://192.168.1.35:5000/api/clustercount').then(response =>{
          console.log(response);
          this.clustercount=response.data;
        }),
        this.$http.get('http://192.168.1.35:5000/api/collectcount').then(response =>{
          console.log(response);
          this.collectcount=response.data;
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

  #bottom{
    height: 57.16vh;
    width: 98.07vw;
    margin:1.62vh 0 0 1.04vw;
    display: flex;
    flex-direction: column;
    justify-content: space-between;

  }
  #left{
    width: 100%;
    height: 27.93vh;
    background-color: #15283f;
  }
  #right{
    display: inline-block;
    width: 100%;
    height: 27.93vh;
    background-color: #15283f;
  }
  #top{
    width: 98.07vw;
    height: 31.59vh;
    margin:6.71vh 0 0 1.04vw;
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
    width: 100%;
    height: 23.71vh;
    margin: 1.11vh 0 0 1.3vw;
    display: flex;
    justify-content: space-between;
  }
  .detail{
    background-color: #13263f;
    height:100%;
    width: 15.52vw;
  }
  .topcontent{
    width: 95.36vw;
    height: 28.3vh;
    margin:0.83vh 0 0 1.33vw;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    background: -webkit-radial-gradient(#173555,#18375c,#163453,#14202f);
  }
  .count{
    background-color: #13263f;
    width: 100%;
    height: 3.89vh;
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
    margin-top:1%;
    height:22%;
    color: #0077fd;
    font-size: 50%;
  }
  .bbpic{
    height: 57.14%;
    display: flex;
    align-items: center;
    font-size: 70%;
    transform: scale(0.6);
    margin-top: 5%;
    white-space: nowrap;
  }
  i{
    transform: scale(0.5);

  }
</style>
