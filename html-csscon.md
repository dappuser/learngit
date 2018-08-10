###css技巧汇总
文本横向居中 text-align:center;

文本限制宽度并不溢出：  word-wrap:break-word;

文本保持水平不竖直（禁止换行）：    white-space: nowrap;
（自动换行）：
word-wrap: break-word;
word-break: normal;
（强制换行）：word-break:break-all;
禁止选中文本：user-select: none

相对与同级的位置：postion：relative  相对于上一级的位置：postion：absolute

位置固定：postion：fixed

调整图片：img {
height:auto;
width:500px;
}

获得焦点后表单设置：input:focus { border: 2px solid green; } 

颜色透明：opacity: 0.5;或者  background-color: rgba(14,14,14,0.8);

伪元素显示顺序
   未触发 a:link
    触发后 a:visited
    放在上面 a:hover
    点击 a:active

盒子状排列：.box2{ display:flex; justify-content:center; align-items:center; text-align:center; }

.box-sizing 让元素的宽度、高度包含border和padding：box-sizing: border-box;

让元素能叠在另一个上方 z-index：1 （数字大在上方）

输入框有颜色解决方法（设置显示延迟）：-webkit-autofill {
  -webkit-text-fill-color: #fff !important;
  transition: background-color 5000s ease-in-out 0s;
}
