# AndroidUtilsLibrary

	Android开发辅助工具类Library，用于快速开发，以便减少做重复的工作，提高开发效率。

# Gradle

AndroidUtilsLibrary/utilslibrary 为 Android Library，添加下面依赖即可使用：

	compile project(':utilslibrary')

# 各个包下的工具类

## 1.utilslibrary.system

	1.AppUtils
		获取应用程序名称
		获取应用程序版本名称信息
		
	2.CameraUtils
		判断摄像头是否可用
	
	3.ConvertUtils 类型转换类
		十六进制字符串转换为byte数组
		byte数组转换为十六进制字符串
		int转换为byte数组
		byte数组转换为int
		保留几位小数

	4.DateUtils
		获取日期
		使指定日期向前走一天，变成“明天”的日期
		使日期倒一天
		判断平年闰年
		计算某月的天数
		获取当天凌晨的秒数
		获取第二天凌晨的秒数
		判断某两天是不是同一天

	5.DensityUtils
		根据手机的分辨率从 dip 的单位 转成为 px(像素)
		根据手机的分辨率从 px(像素) 的单位 转成为 dp
		
	6.FileUtils
		检查是否存在SD卡
		创建目录
		删除文件（若为目录，则递归删除子目录和文件）
		获取文件大小，单位为byte（若为目录，则包括所有子目录和文件）
		保存Bitmap到指定目录
		判断某目录下文件是否存在
	
	7.KeyBoardUtils
		切换软键盘的状态，如当前为收起变为弹出,若当前为弹出变为收起
		强制隐藏输入法键盘
		强制显示输入法键盘
		输入法是否显示
	
	8.LogUtils
		调试打印Log
	
	9.ScreenUtils
		获得屏幕高度
		获得屏幕宽度
		获得状态栏的高度
		获取当前屏幕截图，包含状态栏
		获取当前屏幕截图，不包含状态栏
	
	10.SDCardUtils
		判断SDCard是否可用
		获取SD卡路径
		获取SD卡的剩余容量(byte)
		获取指定路径所在空间的剩余可用容量字节数(byte)
		获取系统存储路径
	
	11.SPUtils
		保存数据的方法（put方法），根据类型调用不同的保存方法
		保存图片到SharedPreferences
		获取数据的方法（get方法），根据默认值得到数据的类型，然后调用对应方法获取值
		从SharedPreferences读取图片
		移除某个key对应的值
		清除所有数据
		查询某个key是否已经存在
		返回所有的键值对

	12.StringUtils
		Unicode转中文
		
	13.ToastUtils
		短时间显示Toast
		长时间显示Toast
	
	14.ViewUtils
		把自身从父View中移除
		判断触点是否落在该View上

## 2.utilslibrary.keygen

	1.MD5Util（Message Digest，消息摘要算法）
		MD5加密 不可逆
		
	2.SHAUtil
		SHA（Secure Hash Algorithm，安全散列算法）
		SHA-1 加密 不可逆
	
	3.DESUtils
		DES（Data Encryption Standard，数据加密标准，对称加密算法）
		生成密钥
		DES加密
		DES解密
	
	4.TripleDESUtils
		3DES（Triple DES、DESede，进行了三重DES加密的算法，对称加密算法）
		生成密钥
		3DES加密（对称加密）
		3DES解密
	
	5.AESUtils
		AES（Advanced Encryption Standard，高级数据加密标准，AES算法可以有效抵制针对DES的攻击算法，对称加密算法）
		生成密钥
		AES加密（对称加密）
		AES解密

## 3.utilslibrary.net

	1.HttpUtils（HttpURLConnection）
		异步的Get请求
		异步的Post请求
		
	2.NetUtils
		判断网络是否连接
		是否有网络，需要加上访问网络状态的权限
		判断是否是WiFi网络
		打开网络设置界面

# License
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
    http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
