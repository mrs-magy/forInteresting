# src > readme

this is the words to descript what 'src 'contents

## 实现isNan、Number.isNaN

```js
// 基本知识
window.isNaN === isNaN // true
isNaN === Number.isNaN // false
NaN === NaN // false

// 实现1
function diyNaN(val){
	let flag = false
	if (typeof val === 'number') {
		flag = isNaN(val)
	}
	return flag
}
// 实现2
function equalNaN(val){
	let flag = typeof val === 'number'&& val !== val
	return flag
}
```

