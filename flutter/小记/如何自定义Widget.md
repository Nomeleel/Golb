# 小记

先去用stateless或者stateful去组装 还有一些有委托接口 可以自定义widget 实在不行就手写renderobject 分为box和 sliver 优先考虑box  如果非要sliver尽量 customscrollview 不去使用nestedscrollview 两个controller不利于二次封装 而且复杂不利于理解 还有 一般情况下 可以都可以转化倒customscrollview的 而且sliver丰富 更利于理解

box是笛卡尔坐标系 sliver可以理解为无限布局中的笛卡尔在视窗做偏移 

containerrenderobject类似于box 只是是基于多个子节点的 box的遍历与融合 
可以先从相似的render重写实现自己的功能 
或者proxy封装 可以从很多render上参考和复用 高达的乐趣 灵活度很大 很利于封装

至于分层的好处 也稍微体现出来了 自由度很大 上层和下层 都可以做到复用 而且下层官方常规的都有实现 可以随意参考 重写