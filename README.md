# touchZoomSlide
移动端支持双手放大缩小的slide插件，支持定义选中第几张

# 插件使用方法

      var photo = $('.photo-body').phototAlbum({
          width: $(window).width(),
          height: $(window).height(),
          lazyLoad: true,
          pagination: false,
          callback: function (i) {
              getTitle(i);
          }
      });
      
# 第几张选中

     photo.goto(num) //num是传入打开页面第几张选中
  
 # 上一张，下一张
 
       photo.prev();
       photo.next();
   
# 默认参数

        var defaultParameters = {
          width: 'auto', // 宽度 
          height: 'auto', // 高度 
          loop: true, // 是否循环
          index: 0, // 当前为第几个
          zoomNumber: 1, // 图片缩放倍数
          maxZoomNumber: 3, // 图片最大缩放的倍数
          picturePosition: { // 图片移动位置
            x: 0,
            y: 0
          },
          transformOrigin: { // 图片缩放基于的点
            x: 0,
            y: 0
          },
          lazyLoad: true, // 是否懒加载
          threShold: 30, // 阀值
          pagination: true, // 是否添加分页器
          paginationClass: 'pagination', // 分页器的className
          container: '.container', // 容器选择器
          child: '.items', // 项容器选择器
          callback: null, // 回调函数
          pictureLoadComplete: null // 图片加载完成时的回调
        };


