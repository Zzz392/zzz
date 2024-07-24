[Uplo<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>zzz</title>
    <style>
      body {
        margin: 0;
        height: 100vh;
        background-color: #eee;
      }
      /* * {  border: 1px solid rgb(0, 0, 0);
      }*/
      .y {
        box-shadow: rgb(0 0 0 / 20%) 0px 2px 1px,
          rgb(0 0 0 / 14%) 0px 1px 1px 0px, rgb(0 0 0 / 12%) 0px 1px 3px 0px;
      }
      .flex {
        display: flex;
      }
      .baiSe {
        background-color: white;
      }
      .flex1 {
        flex: 1;
      }
      .column {
        flex-direction: column;
      }
      .mg8 {
        margin: 8px;
      }
      .mgr8 {
        margin-right: 8px;
      }
      .mat8 {
        margin-top: 8px;
      }
    </style>
  </head>
  <body class="flex">
    <!--侧边栏-->
    <div style="width: 200px; z-index: 2" class="baiSe y">
      <!--头像-->
      <div
        style="
          padding: 10px;
          align-items: center;
          justify-content: center;
          border-bottom: 1px solid #999;
        "
        class="flex"
      >
        <img
          src="https://p1.ssl.qhimgs1.com/sdr/400__/t016fe23f8ee7eb2d01.jpg"
          alt="头像"
          width="40px"
          height="40px"
          style="margin-right: 10px"
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
ading Untitled-1.html…]()
