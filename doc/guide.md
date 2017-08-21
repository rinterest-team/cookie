### 使用说明

Cookie 是指某些网站为了辨别用户身份而储存在用户本地终端（Client Side）上的数据（通常经过加密）。

KISSY cookie 模块对常用的 cookie 方法进行了封装，可以让你更方便的使用 cookie 的接口。

### 基本使用示例

```javascript
	var cookie = require('cookie');
	// set cookie
	cookie.set('a', 'b');
	// 读取 cookie
	cookie.get('a'); // => b
	// 删除 cookie
	cookie.remove('a');
```

### 一些注意事项

Cookie 被存储在客户端，可能被恶意篡改，所以，当从 cookie 中读取数据后，尽可能的做下 xss 过滤再进行使用或者渲染。
