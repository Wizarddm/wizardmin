# mst

## 一行代码实现数组去重（ES6）

```javascript
// 方法一
let array = Array.from(new Set([1,1,1,2,3,4,5,4,3]));

// 方法二
let arr = arr.filter((val,index,self) => self.indexOf(val) === index )

```

## 使用js实现一个持续的动画效果

```javascript
 var progress = 0;
    //回调函数
    function render() {
        progress += 1; //修改图像的位置
        console.log(progress)
        if (progress < 100) {
              //在动画没有结束前，递归渲染
              window.requestAnimationFrame(render);
        }
    }
    //第一帧渲染
    window.requestAnimationFrame(render);

```