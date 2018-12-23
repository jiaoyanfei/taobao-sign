# taobao-sign
#### 淘宝系部分api sign参数的破解
#### 淘宝系的部分api会加sign参数校验有效性
#### 加密方法参见sign.js
#### 用于加密的参数一般形式如下
#### var token = getToken(document.cookie);
#### var signParams = token + "&" + time + "&" + appKey + "&" + JSON.stringify(data);
#### var sign = makeSign(signParams);
#### 其中document.cookie就是淘宝系（*.taobao.com）网站的cookie
#### 其中appKey 可在相关api中查到，一般是对应app的key，是个固定值
#### 其中data就是此http(s)请求的相关核心参数，具体依不同的api而不同
#### getToken 和 makeSign 详见本项目sign.js
![avatar](/images/demo.png)

# License(/LICENSE)
