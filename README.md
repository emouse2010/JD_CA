## 京东评论抓取
输入京东详情页的商品ID，如：
shop_id = '47831955013' 
自动抓取并保存对应的京东评价信息到excel表格中。

> *  由于京东评论页面经常改版，不一定一直有效。
> * 京东评价最多只能抓取1000条。  

安装依赖  
> pip install -r requirements.txt    

打包成单个程序  
> pyinstaller -F JDCA.py  
> 在 Windows 下该选项的格式为 --add-data="源地址;目标地址" ，可多次重复使用。
其他系统的命令格式需要把地址分隔符从分号 ; 改成冒号 : ，详见官方手册。

## 新增  
售卖详情页用户咨询及回答抓取，对应抓取京东详情页的用户问答栏目，用于了解用户关注情况，抓取完成后在对应excel文件的“用户咨询” sheet中。