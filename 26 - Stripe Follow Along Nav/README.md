  .trigger-enter .dropdown {
    display: block;
  }

  .trigger-enter-active .dropdown {
    opacity: 1;
  }


 A 分两步使dropdown做呈现
  1-可获取该div(隐藏未active时)的长宽
  2-添加背景；


B-transform, translate

C-getBoundingClientRect()

D A && B, if a成立，则运行B；
