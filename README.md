<!DOCTYPE html>
<>lang="en"
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>zzz</title>
    <style>
      body {
        margin: 0;
        height: 100vh;
        background-color: #eee;
      }
      /* * { 边框：1px 实线 rgb(0, 0, 0);
      */
      .y {
        盒子阴影：rgb （0  0  0 / 20 ％） 0像素 2像素 1像素，
          rgb （0  0  0 / 14 ％） 0 px  1 px  1 px  0 px，rgb （0  0  0 / 12 ％） 0 px  1 px  3 px  0 px；
      }
      。柔性{
        显示：弹性；
      }
      .白色{
        背景颜色：白色；
      }
      .flex1 {
        弹性：1；
      }
      。柱子{
        弹性方向：列；
      }
      .mg8 {
        边距：8px；​
      }
      .mgr8 {
        右边距：8px；
      }
      .mat8 {
        上边距：8px；
      }
    </样式>
  </头>
  <主体类= “flex” >
    <!--侧边栏-->
    < div style = " width : 200 px ; z-index : 2 "  class = "baiSe y" >
      <!--头像-->
      < div
        风格= “
          填充：10像素；
          对齐项目：居中；
          对齐内容：居中；
          底部边框：1 px 实线#999;
        “
        类= “flex”
      >
        <图片
          来源= “https://p1.ssl.qhimgs1.com/sdr/400__/t016fe23f8ee7eb2d01.jpg”
          alt = "头像"
          宽度= “40px”
          高度= "40px"
          样式= “右边距：10像素”
        />
        <div>zzz</div>
      </div>
      <!--导航-->
      <div></div>
    </div>
    <!--主区域-->
    <div class="flex flex1 column">
      <!--头部栏-->
      <div style="height: 60px; z-index: 1" class="baiSe y"></div>
      <!--内容栏-->
      <div style="overflow: auto" class="flex1 flex">
        <!--左-->
        <div style="flex: 3" class="flex column mg8">
          <!--数据区-->
          <div class="flex">
            <!--数据块-->
            <div style="height: 100px" class="flex1 y baiSe mgr8"></div>
            <div style="height: 100px" class="flex1 y baiSe mgr8"></div>
            <div style="height: 100px" class="flex1 y baiSe mgr8"></div>
            <div style="height: 100px" class="flex1 y baiSe"></div>
          </div>
          <!--列表区-->
          <div class="flex column">
            <!--列表项-->
            <div style="height: 160px" class="y baiSe mat8"></div>
            <div style="height: 160px" class="y baiSe mat8"></div>
            <div style="height: 160px" class="y baiSe mat8"></div>
            <div style="height: 160px" class="y baiSe mat8"></div>
            <div style="height: 160px" class="y baiSe mat8"></div>
            <div style="height: 160px" class="y baiSe mat8"></div>
          </div>
        </div>
        <!--右-->
        <div style="flex: 1" class="flex column mgr8 mat8">
          <!--提示区-->
          <div style="height: 150px" class="y baiSe"></div>
          <!--消息区-->
          <div style="height: 300px" class="y baiSe mat8"></div>
        </div>
      </div>
    </div>
  </body>
</html>

