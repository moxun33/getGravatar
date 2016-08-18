# getGravatar
一、Gravatar头像加载地址：
头像服务器/avatar/邮箱的md5值?s=头像尺寸&d=默认头像&r=头像等级
如果需要强制显示默认头像，在最后加上参数&f=y

二、可选“头像服务器”：
http://www.gravatar.com
http://0.gravatar.com
http://1.gravatar.com
http://2.gravatar.com
http://3.gravatar.com
http://s.gravatar.com
http://en.gravatar.com
https://secure.gravatar.com (由于中国的网络环境，推荐这个)

三、“邮箱的md5值”获取方法：

md5(strtolower(trim("MyEmailAddress@example.com"))); //去掉首尾空格、全部转换成小写字母
四、“头像尺寸”可选范围：
Gravatar头像尺寸的可选范围是1~512(1px到512px)

五、“默认头像”参数：
留空 显示gravatar官方图形
404 直接返回404错误状态
mm 神秘人(一个灰白头像)
identicon 抽象几何图形
monsterid 小怪物
wavatar 用不同面孔和背景组合生成的头像
retro 八位像素复古头像
也可以是一个经过urlencode处理的真实图片地址，用如下代码处理：

urlencode('http://example.com/images/avatar.jpg');
六、“头像等级”参数：
g 适合任何年龄的访客查看，一般都用这个
pg 可能有争议的头像，只适合13岁以上读者查看
r 成人级，只适合17岁以上成人查看
x 最高等级，不适合大多数人查看


