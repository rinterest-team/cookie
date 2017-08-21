### get( name )

获取 cookie 值。

#### Parameters:	

* name {String} – cookie 的名称

#### Returns:	

{String}

### remove( name, domain, path, secure )

置空 cookie 值，并立刻过期。

#### Parameters:	

* name, {String} – cookie的名称
* domain {String} – 域
* path {String} – 路径
* secure {Boolean} – 安全标志

### set( name, val[, expires, domain, path, secure] )

设置cookie值。

#### Parameters:	

* name {String} – cookie 的名称
* val {String} – cookie 的值
* expires {number|date} – 失效时间. number 类型时单位为天，不设置表示生效时间为本次浏览器进程。
* domain {String} – 域
* path {String} – 路径
* secure {Boolean} – 安全标志

#### Note:

建议前端小心使用 set 接口，一定要与后端童鞋多沟通配合，不要在多个地方各自写 cookie。
