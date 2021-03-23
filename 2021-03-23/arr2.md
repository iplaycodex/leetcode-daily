# 附加题

> 今日份的附加题还是一道跟数组有关系的算法题,其实也很简单.按照难度讲应该是 easy 类型的

# 题目

给定一个数组,假设该数组中有一个元素跟其他元素不一样,找出这个不一样的元素并返回.eg:

```javascript
let arr = [1, 2, 1, 1, 1, 1, 1]; //返回2
```

# 题解

> 这个题目其实很简答,几行代码就搞定了.如下所示:

```javascript
function findDiff(arr) {
    if (!Array.isArray(arr) || arr.length === 0) return arr;
    /**
     * 假设第一个元素是与其他元素不同的那个元素,利用数组的 find api 即可一行代码实现这个算法
     * 这个算法还是比较简单的,属于 easy 难度
     */
    let a = arr[0];
    return arr.find((item) => item !== a);
}
```
