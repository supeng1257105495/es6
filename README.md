# es6
es6 小结 笔记
## 数组

//json 数组格式
// let json  = {
//    // key:value,//普通的json格式
// }

// let json1  = {
//     '0':'super',
//     '1':'super1',
//     '2':'super2',
//     length:3,
// }
//json 数组格式转换成数组 Array.of()
// 1
// let arr = Array.from(json1)
// console.log(arr)
// Array.of 
// '3,4,5,6';
// let arr = '3,4,5,6';
// let arr1 = '[3,4,5,6];
// let arr1 = Array.of(arr)//以前使用eval  现在可以使用 Array.of()
// console.log(arr1)//转换成了数组

//find() 实例方法
// let arr = [1,2,3,4,5,6,7,8,9];
// let arr = ['super','jspang','supeng']
// console.log(arr.find(function(value,index,arr){//value表示当前查找的值 ， index 表示查找之的索引 ，查找原型
//     // return value >5;//满足条件就不在查找 返回值6
//     // return value >10;//如果没有满足条件的值 返回 undefined
//     return value == 'super';//返回值 supeng 满足条件 返回满足条件的值 未满足时返回 undefined
// }))

// fill()实例方法
// let arr = ['super','jspang','supeng'];
// arr.fill('web',1,2)//填充替换 接受三个值 第一个替换的对象 第二个 替换开始的位置 脚标计算从0开始  第三个 替换结束的位置 脚标计算从1开始
// console.log(arr)

// 数组循环 
// let arr = ['super','jspang','supeng'];
// for(let item of arr){
//     console.log(item);//输出数组的值
   
// }
// for(let item of arr.keys()){
//     console.log(item);//输出数组的下标
   
// }
// for(let [index,value] of arr.entries()){
//     console.log(index+'索引'+value+'下标');//输出数组值和下标    
   
// }

//entries
let arr = ['super','jspang','supeng'];
let list = arr.entries()//手动循环生成条目
console.log(list.next().value)//[0, "super"]
console.log(list.next().value)//[1, "jspang"]
console.log(list.next().value)//[2, "supeng"]
