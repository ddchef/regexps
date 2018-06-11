# 日常使用正则（持续更新）
## 网络
1. xxx.xxx.xxx.xxxx 
```js
/^(25[0-5]|2[0-4]\d|1\d{2}|\d{2}|\d)(\.(25[0-5]|2[0-4]\d|1\d{2}|\d{2}|\d)){3}$/
```
2. xxx.xxx.xxx.xxx/xx或xxx.xxx.xxx.xxx/xxx.xxx.xxx.xxx
```js
/^((25[0-5]|2[0-4]\d|1\d{2}|\d{2}|\d)(\.(25[0-5]|2[0-4]\d|1\d{2}|\d{2}|\d)){3}\/\d{1,2})$|^((25[0-5]|2[0-4]\d|1\d{2}|\d{2}|\d)(\.(25[0-5]|2[0-4]\d|1\d{2}|\d{2}|\d)){3}\/(25[0-5]|2[0-4]\d|1\d{2}|\d{2}|\d)(\.(25[0-5]|2[0-4]\d|1\d{2}|\d{2}|\d)){3})$/
```
3. 域名
```js
/^([-a-zA-Z0-9_]+\.)+[-a-zA-Z0-9_]+$/
```
4. 端口
```js
/^6(?:(553[0-5])|(55[0-2]\d)|(5[0-4]\d{2})|([0-4]\d{3}))$|^([1-5]?\d{1,4})$/
```
## 联系方式
1. 手机号码
```js
/^1\d{10}$/
```
2. 多个手机号码 
```js
/^(1\d{10},?)+$/
```
3. 邮箱
```js
/^[-_a-zA-Z0-9\.]+@[-_a-zA-Z0-9]+(\.[-_a-zA-Z0-9]+)+$/
```
4. 多个邮箱
```js
/^([-_a-zA-Z0-9\.]+@[-_a-zA-Z0-9]+(\.[-_a-zA-Z0-9]+)+,?)+$/
```
5. 固定电话、传真
```js
/^((0\d{2,3})-?)(\d{7,8})(-?(\d{0,4}))?$/
```
6. 邮编
```js
/^\d{6}$/
```
## 字符串及数字
1. 自然数
```js
/^[1-9]\d+$|^[0-9]$/
```
2. 大小写英文
```js
/^[a-zA-Z]+$/
```
## 地理位置
1. 经度(精确到小数点后六位)
```js
/^[-+]?(0?\d{1,2}\.\d{1,6}|1[0-7]?\d{1}\.\d{1,6}|180\.0{1,6})$/
```
2. 纬度(精确到小数点后六位)
```js
/^[-+]?([0-8]?\d{1}\.\d{1,6}|90\.0{1,6})$/
```
