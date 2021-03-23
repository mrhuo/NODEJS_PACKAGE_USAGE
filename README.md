# NODEJS_PACKAGE_USAGE

    用于记录使用过的 nodejs 包使用方法。

---- 
目录（`点击链接直达`）：

## 加密解密

<table>
    <thead>
        <tr>
            <th>名称</th>
            <th>简介</th>
            <th>主页</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="#abab">abab</a>
            </td>
            </td>
            <td>BASE64 加密解密</td>
            <td>
                <a href="https://www.npmjs.com/package/abab" target="_blank">
                    <img src="https://badge.fury.io/js/abab.svg" />
                </a>
                <a href="http://npm-stat.com/charts.html?package=abab" target="_blank">
                    <img src="https://badge.fury.io/js/abab.svg" />
                </a>
            </td>
        </tr>
        <tr>
            <td>
                <a href="#md5">md5</a>
            </td>
            </td>
            <td>md5 字符串/文件加密</td>
            <td>
                <a href="https://www.npmjs.com/package/md5" target="_blank">
                    <img src="https://badge.fury.io/js/md5.svg" />
                </a>
                <a href="http://npm-stat.com/charts.html?package=md5" target="_blank">
                    <img src="https://badge.fury.io/js/md5.svg" />
                </a>
            </td>
        </tr>
    </tbody>
</table>

----
#### **abab** 

> `BASE64` 加密解密


安装方法：

```bash
npm install abab
```

使用方法：

btoa (base64 加密)

```js
const { btoa } = require('abab');
btoa('Hello, world!'); // 'SGVsbG8sIHdvcmxkIQ=='
```

atob (base64 解密)
```js
const { atob } = require('abab');
atob('SGVsbG8sIHdvcmxkIQ=='); // 'Hello, world!'
```

----
#### **md5**

> `MD5` 加密

[![](https://badge.fury.io/js/md5.svg)](https://www.npmjs.com/package/md5)
[![](https://img.shields.io/npm/dt/md5.svg)](http://npm-stat.com/charts.html?package=md5)

安装方法：


```bash
npm install md5
```

使用方法：

```js
var md5 = require('md5');
console.log(md5('message')); // 78e731027d8fd50ed642340b7c9a63b3
```

支持 `buffer` 流，比如文件 `md5`

```js
var fs = require('fs');
var md5 = require('md5');
fs.readFile('example.txt', function(err, buf) {
    console.log(md5(buf));
});
```