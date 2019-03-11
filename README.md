# ViewPagerGallery
不懂看博客、不懂看博客、不懂看博客
<p>[博客讲解地址](https://blog.csdn.net/lin857/article/details/84644569)
# 特点功能:
* 支持左右无限滑动轮播/<br>
* 支持3D效果的画廊轮播/<br>
* 支持平面铺满常见轮播/<br>
* 支持平面自定义间距轮播/<br>
* 支持网络缓存图片(使用的Glide)/<br>
* 支持自定义指示器图标(默认指示器个数与url一样)/<br>
* 支持自定义圆角/<br>
* 支持自动切换图片,间隔默认5秒/<br>
# API方法介绍:
* initBanner(urlList, true)//url数组，是否3D画廊效果/<br>
* addPageMargin(10, 50)//page之间的间距,中间item距离边界的间距/<br>
* addPoint(6)//添加指示器之间的间距/<br>
* addPointBottom(7)//指示器底部间距/<br>
* addStartTimer(5)//添加自动切换/<br>
* addRoundCorners(12)//添加圆角/<br>
* finishConfig()//最后加这句/<br>
<h3>效果一:3D画廊效果</h3>
<p><img   src="https://raw.githubusercontent.com/lzjin/ViewPagerGallery/master/imgfile/ic_banner1.png">
<h3>效果二:平面自定义间距效果</h3>
<p><img   src="https://raw.githubusercontent.com/lzjin/ViewPagerGallery/master/imgfile/ic_banner2.png">
<h3>效果三:平面铺满常见效果</h3>
<p><img    src="https://raw.githubusercontent.com/lzjin/ViewPagerGallery/master/imgfile/ic_banner3.png">
<h2>使用步骤</h2>
</br>首先在gradle文件中添加
<h3> implementation 'com.github.lzjin:ViewPagerGallery:1.06' </h3>

<h3>使用参考</h3>
viewPager.initBanner(urlList, true) </br>
         .addPageMargin(10, 60) </br>
         .addPoint(6)           </br>
         .addPointBottom(7)     </br>
         .addStartTimer(5)      </br>
         .addRoundCorners(12)   </br>
         .finishConfig()        </br>
         .addBannerListener(new BannerViewPager.OnClickBannerListener() { </br>
         @Override              </br>
         public void onBannerClick(int i) { </br>
             //点击回调          </br>
         }                      </br>
         });                    </br>
         