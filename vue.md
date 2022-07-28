# hello Vue

![image-20211019100701804](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019100701804.png)

![image-20211019101836230](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019101836230.png)

![image-20211019101954463](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019101954463.png)

![image-20211019103119763](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019103119763.png)

![image-20211019103533635](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019103533635.png)

# 指令语法V-bind

![image-20211019104159093](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019104159093.png)

![image-20211019104244288](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019104244288.png)

## V-bind的简写

![image-20211019104332200](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019104332200.png)

![image-20211019104506112](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019104506112.png)

![image-20211019104759949](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019104759949.png)

# 数据绑定

v-bind是单向绑定

v-modle双向绑定

![image-20211019105242427](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019105242427.png)

简写方式

![image-20211019105448579](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019105448579.png)

# el和data的两种语法

![image-20211019105943273](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019105943273.png)

这种方式比较灵活

![image-20211019110158855](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019110158855.png)

简写方式

![image-20211019110331870](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019110331870.png)

组件都用这种方式

## 箭头函数没有自己的this

![image-20211019110410632](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019110410632.png)

![image-20211019110814694](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019110814694.png)

![image-20211019110822781](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019110822781.png)

# 理解MVVM模型

![image-20211019111608293](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019111608293.png)

原型上有的东西可以直接在模板上使用

# 数据代理

![image-20211019112034438](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019112034438.png)

![image-20211019112423204](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019112423204.png)

![image-20211019112604270](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019112604270.png)

![image-20211019113107869](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019113107869.png)

![image-20211019113435778](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019113435778.png)

![image-20211019113543908](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019113543908.png)

![image-20211019141625692](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019141625692.png)

这里的_data=上面的data，而数据代理就是做了一个操作：将 _data中的数据给了vm，vm就代理了其中的name和address

# 事件处理

![image-20211019142418664](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019142418664.png)

简写方式

![image-20211019142737882](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019142737882.png)

![image-20211019143311628](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019143311628.png)

![image-20211019143432578](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019143432578.png)

上面这种方式会导致event丢失

![image-20211019143657325](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019143657325.png)

![image-20211019143916051](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019143916051.png)

![image-20211019144146778](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019144146778.png)

![image-20211019144233731](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019144233731.png)

![image-20211019144254480](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019144254480.png)

![image-20211019145001547](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019145001547.png)

## 键盘事件

![image-20211019150127538](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019150127538.png)

![image-20211019150138903](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019150138903.png)

![image-20211019150530255](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019150530255.png)

![image-20211019150737727](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019150737727.png)

![image-20211019150805029](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019150805029.png)

![image-20211019151124515](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019151124515.png)

![image-20211019152523274](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019152523274.png)

![image-20211019152654337](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019152654337.png)

# 计算属性

![image-20211019153059348](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019153059348.png)

![image-20211019153723135](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019153723135.png)

![image-20211019161231137](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019161231137.png)

![image-20211019161419435](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019161419435.png)

![image-20211019161808035](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019161808035.png)

![image-20211019162900301](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019162900301.png)

**简写形式调用时括号不用**

# 监视属性

![image-20211019163427180](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019163427180.png)

![image-20211019164244199](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019164244199.png)

![image-20211019164336103](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019164336103.png)

![image-20211019164636430](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019164636430.png)

以上这个是监视的另一种写法

## 深度监视

![image-20211019165743953](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019165743953.png)

![image-20211019170442408](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019170442408.png)

![image-20211019170537077](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019170537077.png)

## 简写

![image-20211019191920067](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019191920067.png)

# 计算属性和监视属性的对比

![image-20211019192448670](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019192448670.png)

![image-20211019192911879](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019192911879.png)

![image-20211019193121760](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019193121760.png)

# 样式绑定

![image-20211019193645900](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019193645900.png)

![image-20211019193820674](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019193820674.png)

![image-20211019194235530](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019194235530.png)

![image-20211019194601661](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019194601661.png)

![image-20211019195018775](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211019195018775.png)

# 条件渲染

![image-20211020225527638](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020225527638.png)

![image-20211020225645763](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020225645763.png)

![image-20211020225716790](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020225716790.png)

![image-20211020225907566](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020225907566.png)

![image-20211020230323985](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020230323985.png)

![image-20211020230616615](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020230616615.png)

![image-20211020230732699](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020230732699.png)

# 列表渲染

![image-20211020231145577](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020231145577.png)

![image-20211020231707082](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020231707082.png)

![image-20211020231848312](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020231848312.png)

![image-20211020231944550](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020231944550.png)

![image-20211020232116380](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020232116380.png)

## key的原理



![image-20211020233924689](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020233924689.png)

![image-20211020234205629](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020234205629.png)

![image-20211020234307913](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020234307913.png)

![image-20211020234453169](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211020234453169.png)

## 列表过滤

![image-20211021000045349](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021000045349.png)

![image-20211021000333912](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021000333912.png)

## 解决不可折叠问题

![image-20211021000613555](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021000613555.png)

![image-20211021001123470](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021001123470.png)

## 列表排序

![image-20211021002156206](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021002156206.png)

![image-20211021002220521](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021002220521.png)

![image-20211021002449790](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021002449790.png)

![image-20211021002556621](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021002556621.png)

![image-20211021002721626](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021002721626.png)

# 数据检测对象原理

![image-20211021005319116](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021005319116.png)

![](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021014034498.png)

![image-20211021014600236](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021014600236.png)

![image-20211021014923572](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021014923572.png)

![image-20211021015044673](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021015044673.png)

![image-20211021015646401](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021015646401.png)

![image-20211021020545450](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021020545450.png)

# 收集表单数据

![image-20211021021232088](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021021232088.png)

![image-20211021022009101](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021022009101.png)

![image-20211021022039932](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021022039932.png)

![image-20211021022350853](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021022350853.png)

![image-20211021022446048](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021022446048.png)

![image-20211021022646092](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021022646092.png)

![image-20211021022816713](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021022816713.png)

![image-20211021022918095](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021022918095.png)

![image-20211021022944144](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021022944144.png)

# 过滤器

![image-20211021023753114](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021023753114.png)

![image-20211021024012842](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021024012842.png)

![image-20211021024438088](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021024438088.png)	

![image-20211021024455983](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021024455983.png)

![image-20211021024609246](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021024609246.png)

# 内置指令

## V-text

![image-20211021024851084](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021024851084.png)

## V-Html

![image-20211021030300457](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021030300457.png)

## V-cloak：

作用：在网速过慢的情况下防止未经解析的元素跑到页面上去

![image-20211021123234189](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021123234189.png)

![image-20211021123425298](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021123425298.png)

## V-once

![image-20211021123639730](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021123639730.png)

## V-pre

![image-20211021123819304](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021123819304.png)

# 自定义指令

![image-20211021124836192](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021124836192.png)

![image-20211021125137417](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021125137417.png)

![image-20211021130216167](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021130216167.png)

![image-20211021130357131](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021130357131.png)

## 总结

![image-20211021130909980](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021130909980.png)

## 自定义指令里面的this是window

![image-20211021131232116](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021131232116.png)

![image-20211021131326315](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021131326315.png)

![image-20211021131551981](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021131551981.png)

# 生命周期

![image-20211021131739422](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021131739422.png)

![image-20211021132508571](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021132508571.png)

![image-20211021132541312](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021132541312.png)

![image-20211021132842385](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021132842385.png)	

![image-20211021133052592](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021133052592.png)

![image-20211021133211765](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021133211765.png)

![image-20211021133818482](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021133818482.png)

![image-20211021134611056](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021134611056.png)

![image-20211021134925393](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021134925393.png)

![image-20211021135326901](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021135326901.png)

![image-20211021154132610](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021154132610.png)

![image-20211021154520405](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021154520405.png)

![image-20211021154958251](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021154958251.png)

![image-20211021155025466](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021155025466.png)

# 组件化编程

![image-20211021155858970](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021155858970.png)

![image-20211021162555071](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021162555071.png)

![image-20211021162851650](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021162851650.png)

![image-20211021162922238](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021162922238.png)

![image-20211021163142525](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021163142525.png)

![image-20211021163600535](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021163600535.png)

![image-20211021163751488](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021163751488.png)

![image-20211021164202493](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021164202493.png)

![image-20211021164628065](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021164628065.png)

![image-20211021183221091](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021184202332.png)

![image-20211021190000452](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021190000452.png)

# vue与VueComponent

![image-20211021190851783](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021190851783.png)

# 单文件组件

![image-20211021192337612](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021192337612.png)

![image-20211021192607331](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021192607331.png)

![image-20211021192756575](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021192756575.png)

![image-20211021192805431](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021192805431.png)

![image-20211021193008960](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021193008960.png)

![image-20211021193024995](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021193024995.png

![image-20211021193151582](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021193151582.png)

![image-20211021193227660](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021193227660.png)

![image-20211021201223329](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021201223329.png)

![image-20211021202248511](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021202248511.png)

![image-20211021203531074](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021203531074.png)

![image-20211021204512837](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021204512837.png)

![image-20211021205536479](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021205536479.png)

# ref属性

![image-20211021210850585](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021210850585.png)

![image-20211021211048625](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021211048625.png)

# Props属性

![image-20211021211624221](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021211624221.png)

![image-20211021211657877](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021211657877.png)

![image-20211021212026155](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021212026155.png)

![image-20211021212125791](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021212125791.png)

![image-20211021212343168](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021212343168.png)

![image-20211021212550836](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021212550836.png)

# mixin混入

两个组件共享一个配置

![image-20211021212957817](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021212957817.png)

![image-20211021213014806](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021213014806.png)

![image-20211021213412202](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021213412202.png)

# 插件

![image-20211021213819277](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021213819277.png)

![image-20211021213900252](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021213900252.png)

![image-20211021214251895](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021214251895.png)

![image-20211021222924274](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021222924274.png)

# localStorage

![image-20211021223803760](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021223803760.png)

![image-20211021224035876](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021224035876.png)

# 组件的自定义事件

![image-20211021225326789](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021225326789.png)

![image-20211021225529056](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021225529056.png)

# 全局事件总线

# ![image-20211021231001376](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021231001376.png)	消息订阅与发布

![image-20211021231245835](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021231245835.png)

![image-20211021231401073](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021231401073.png)

![image-20211021231547285](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021231547285.png)

![image-20211021231739250](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021231739250.png)

# nextTick

![image-20211021232105323](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021232105323.png)

# 动画效果

![image-20211021232352090](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021232352090.png)

![image-20211021232414529](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021232414529.png)

# 配置代理方法一

![image-20211021232756288](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021232756288.png)

![image-20211021232936765](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021232936765.png)

![image-20211021233857377](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021233857377.png)

![image-20211021234114932](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021234114932.png)

# 配置代理方法二

![image-20211021234631234](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021234631234.png)

![image-20211021234734297](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021234734297.png)

# 总结代理方法

![image-20211021234823329](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021234823329.png)

![image-20211021234833805](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021234833805.png)

![image-20211021234919949](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211021234919949.png)

![image-20211022000643718](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022000643718.png)

# vuex

![image-20211022001536942](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022001536942.png) 	![image-20211022001805512](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022001805512.png)

![image-20211022001958388](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022001958388.png)

![image-20211022003309497](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022003309497.png)   	

![image-20211022003926993](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022003926993.png

![image-20211022003952859](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022003952859.png)

![image-20211022005708001](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022005708001.png)

![image-20211022010430264](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022010430264.png)

# 路由

![image-20211022011613859](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022011613859.png)

![image-20211022011754937](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022011754937.png)

![image-20211022011820426](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022011820426.png)

# vue UI组件库

![image-20211022014847886](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211022014847886.png)

# dockfile

![image-20211116100828693](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116100828693.png)

![image-20211116100927682](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116100927682.png)

## RUN rm -f /usr/share/nginx/html/index.html

![image-20211116101041185](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116101041185.png)

## ADD nginx.conf /etc/nginx/

![image-20211116101221061](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116101221061.png)

## ![image-20211116101546523](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116101546523.png)copy

## 资源访问地址：https://www.cnblogs.com/panwenbin-logs/p/8007348.html

# nginx.conf文件

######Nginx配置文件nginx.conf中文详解#####

#定义Nginx运行的用户和用户组
user www www;

#nginx进程数，建议设置为等于CPU总核心数。
worker_processes 8;

#全局错误日志定义类型，[ debug | info | notice | warn | error | crit ]
error_log /usr/local/nginx/logs/error.log info;

#进程pid文件
pid /usr/local/nginx/logs/nginx.pid;

#指定进程可以打开的最大描述符：数目
#工作模式与连接数上限
#这个指令是指当一个nginx进程打开的最多文件描述符数目，理论值应该是最多打开文件数（ulimit -n）与nginx进程数相除，但是nginx分配请求并不是那么均匀，所以最好与ulimit -n 的值保持一致。
#现在在linux 2.6内核下开启文件打开数为65535，worker_rlimit_nofile就相应应该填写65535。
#这是因为nginx调度时分配请求到进程并不是那么的均衡，所以假如填写10240，总并发量达到3-4万时就有进程可能超过10240了，这时会返回502错误。
worker_rlimit_nofile 65535;

events
{
    #参考事件模型，use [ kqueue | rtsig | epoll | /dev/poll | select | poll ]; epoll模型
    #是Linux 2.6以上版本内核中的高性能网络I/O模型，linux建议epoll，如果跑在FreeBSD上面，就用kqueue模型。
    #补充说明：
    #与apache相类，nginx针对不同的操作系统，有不同的事件模型
    #A）标准事件模型
    #Select、poll属于标准事件模型，如果当前系统不存在更有效的方法，nginx会选择select或poll
    #B）高效事件模型
    #Kqueue：使用于FreeBSD 4.1+, OpenBSD 2.9+, NetBSD 2.0 和 MacOS X.使用双处理器的MacOS X系统使用kqueue可能会造成内核崩溃。
    #Epoll：使用于Linux内核2.6版本及以后的系统。
    #/dev/poll：使用于Solaris 7 11/99+，HP/UX 11.22+ (eventport)，IRIX 6.5.15+ 和 Tru64 UNIX 5.1A+。
    #Eventport：使用于Solaris 10。 为了防止出现内核崩溃的问题， 有必要安装安全补丁。
    use epoll;

```
#单个进程最大连接数（最大连接数=连接数*进程数）
#根据硬件调整，和前面工作进程配合起来用，尽量大，但是别把cpu跑到100%就行。每个进程允许的最多连接数，理论上每台nginx服务器的最大连接数为。
worker_connections 65535;

#keepalive超时时间。
keepalive_timeout 60;

#客户端请求头部的缓冲区大小。这个可以根据你的系统分页大小来设置，一般一个请求头的大小不会超过1k，不过由于一般系统分页都要大于1k，所以这里设置为分页大小。
#分页大小可以用命令getconf PAGESIZE 取得。
#[root@web001 ~]# getconf PAGESIZE
#4096
#但也有client_header_buffer_size超过4k的情况，但是client_header_buffer_size该值必须设置为“系统分页大小”的整倍数。
client_header_buffer_size 4k;

#这个将为打开文件指定缓存，默认是没有启用的，max指定缓存数量，建议和打开文件数一致，inactive是指经过多长时间文件没被请求后删除缓存。
open_file_cache max=65535 inactive=60s;

#这个是指多长时间检查一次缓存的有效信息。
#语法:open_file_cache_valid time 默认值:open_file_cache_valid 60 使用字段:http, server, location 这个指令指定了何时需要检查open_file_cache中缓存项目的有效信息.
open_file_cache_valid 80s;

#open_file_cache指令中的inactive参数时间内文件的最少使用次数，如果超过这个数字，文件描述符一直是在缓存中打开的，如上例，如果有一个文件在inactive时间内一次没被使用，它将被移除。
#语法:open_file_cache_min_uses number 默认值:open_file_cache_min_uses 1 使用字段:http, server, location  这个指令指定了在open_file_cache指令无效的参数中一定的时间范围内可以使用的最小文件数,如果使用更大的值,文件描述符在cache中总是打开状态.
open_file_cache_min_uses 1;

#语法:open_file_cache_errors on | off 默认值:open_file_cache_errors off 使用字段:http, server, location 这个指令指定是否在搜索一个文件是记录cache错误.
open_file_cache_errors on;
```

}

 

#设定http服务器，利用它的反向代理功能提供负载均衡支持
http
{
    #文件扩展名与文件类型映射表
    include mime.types;

```
#默认文件类型
default_type application/octet-stream;

#默认编码
#charset utf-8;

#服务器名字的hash表大小
#保存服务器名字的hash表是由指令server_names_hash_max_size 和server_names_hash_bucket_size所控制的。参数hash bucket size总是等于hash表的大小，并且是一路处理器缓存大小的倍数。在减少了在内存中的存取次数后，使在处理器中加速查找hash表键值成为可能。如果hash bucket size等于一路处理器缓存的大小，那么在查找键的时候，最坏的情况下在内存中查找的次数为2。第一次是确定存储单元的地址，第二次是在存储单元中查找键 值。因此，如果Nginx给出需要增大hash max size 或 hash bucket size的提示，那么首要的是增大前一个参数的大小.
server_names_hash_bucket_size 128;

#客户端请求头部的缓冲区大小。这个可以根据你的系统分页大小来设置，一般一个请求的头部大小不会超过1k，不过由于一般系统分页都要大于1k，所以这里设置为分页大小。分页大小可以用命令getconf PAGESIZE取得。
client_header_buffer_size 32k;

#客户请求头缓冲大小。nginx默认会用client_header_buffer_size这个buffer来读取header值，如果header过大，它会使用large_client_header_buffers来读取。
large_client_header_buffers 4 64k;

#设定通过nginx上传文件的大小
client_max_body_size 8m;

#开启高效文件传输模式，sendfile指令指定nginx是否调用sendfile函数来输出文件，对于普通应用设为 on，如果用来进行下载等应用磁盘IO重负载应用，可设置为off，以平衡磁盘与网络I/O处理速度，降低系统的负载。注意：如果图片显示不正常把这个改成off。
#sendfile指令指定 nginx 是否调用sendfile 函数（zero copy 方式）来输出文件，对于普通应用，必须设为on。如果用来进行下载等应用磁盘IO重负载应用，可设置为off，以平衡磁盘与网络IO处理速度，降低系统uptime。
sendfile on;

#开启目录列表访问，合适下载服务器，默认关闭。
autoindex on;

#此选项允许或禁止使用socke的TCP_CORK的选项，此选项仅在使用sendfile的时候使用
tcp_nopush on;
 
tcp_nodelay on;

#长连接超时时间，单位是秒
keepalive_timeout 120;

#FastCGI相关参数是为了改善网站的性能：减少资源占用，提高访问速度。下面参数看字面意思都能理解。
fastcgi_connect_timeout 300;
fastcgi_send_timeout 300;
fastcgi_read_timeout 300;
fastcgi_buffer_size 64k;
fastcgi_buffers 4 64k;
fastcgi_busy_buffers_size 128k;
fastcgi_temp_file_write_size 128k;

#gzip模块设置
gzip on; #开启gzip压缩输出
gzip_min_length 1k;    #最小压缩文件大小
gzip_buffers 4 16k;    #压缩缓冲区
gzip_http_version 1.0;    #压缩版本（默认1.1，前端如果是squid2.5请使用1.0）
gzip_comp_level 2;    #压缩等级
gzip_types text/plain application/x-javascript text/css application/xml;    #压缩类型，默认就已经包含textml，所以下面就不用再写了，写上去也不会有问题，但是会有一个warn。
gzip_vary on;

#开启限制IP连接数的时候需要使用
#limit_zone crawler $binary_remote_addr 10m;
```



```
#负载均衡配置
upstream jh.w3cschool.cn {
 
    #upstream的负载均衡，weight是权重，可以根据机器配置定义权重。weigth参数表示权值，权值越高被分配到的几率越大。
    server 192.168.80.121:80 weight=3;
    server 192.168.80.122:80 weight=2;
    server 192.168.80.123:80 weight=3;

    #nginx的upstream目前支持4种方式的分配
    #1、轮询（默认）
    #每个请求按时间顺序逐一分配到不同的后端服务器，如果后端服务器down掉，能自动剔除。
    #2、weight
    #指定轮询几率，weight和访问比率成正比，用于后端服务器性能不均的情况。
    #例如：
    #upstream bakend {
    #    server 192.168.0.14 weight=10;
    #    server 192.168.0.15 weight=10;
    #}
    #2、ip_hash
    #每个请求按访问ip的hash结果分配，这样每个访客固定访问一个后端服务器，可以解决session的问题。
    #例如：
    #upstream bakend {
    #    ip_hash;
    #    server 192.168.0.14:88;
    #    server 192.168.0.15:80;
    #}
    #3、fair（第三方）
    #按后端服务器的响应时间来分配请求，响应时间短的优先分配。
    #upstream backend {
    #    server server1;
    #    server server2;
    #    fair;
    #}
    #4、url_hash（第三方）
    #按访问url的hash结果来分配请求，使每个url定向到同一个后端服务器，后端服务器为缓存时比较有效。
    #例：在upstream中加入hash语句，server语句中不能写入weight等其他的参数，hash_method是使用的hash算法
    #upstream backend {
    #    server squid1:3128;
    #    server squid2:3128;
    #    hash $request_uri;
    #    hash_method crc32;
    #}

    #tips:
    #upstream bakend{#定义负载均衡设备的Ip及设备状态}{
    #    ip_hash;
    #    server 127.0.0.1:9090 down;
    #    server 127.0.0.1:8080 weight=2;
    #    server 127.0.0.1:6060;
    #    server 127.0.0.1:7070 backup;
    #}
    #在需要使用负载均衡的server中增加 proxy_pass http://bakend/;

    #每个设备的状态设置为:
    #1.down表示单前的server暂时不参与负载
    #2.weight为weight越大，负载的权重就越大。
    #3.max_fails：允许请求失败的次数默认为1.当超过最大次数时，返回proxy_next_upstream模块定义的错误
    #4.fail_timeout:max_fails次失败后，暂停的时间。
    #5.backup： 其它所有的非backup机器down或者忙的时候，请求backup机器。所以这台机器压力会最轻。

    #nginx支持同时设置多组的负载均衡，用来给不用的server来使用。
    #client_body_in_file_only设置为On 可以讲client post过来的数据记录到文件中用来做debug
    #client_body_temp_path设置记录文件的目录 可以设置最多3层目录
    #location对URL进行匹配.可以进行重定向或者进行新的代理 负载均衡
}
```

​     
​     
​    #虚拟主机的配置
​    server
​    {
​        #监听端口
​        listen 80;
​    
​        #域名可以有多个，用空格隔开
​        server_name www.w3cschool.cn w3cschool.cn;
​        index index.html index.htm index.php;
​        root /data/www/w3cschool;
​    
​        #对******进行负载均衡
​        location ~ .*.(php|php5)?$
​        {
​            fastcgi_pass 127.0.0.1:9000;
​            fastcgi_index index.php;
​            include fastcgi.conf;
​        }
​         

```
    #图片缓存时间设置
    location ~ .*.(gif|jpg|jpeg|png|bmp|swf)$
    {
        expires 10d;
    }
     
    #JS和CSS缓存时间设置
    location ~ .*.(js|css)?$
    {
        expires 1h;
    }
     
    #日志格式设定
    #$remote_addr与$http_x_forwarded_for用以记录客户端的ip地址；
    #$remote_user：用来记录客户端用户名称；
    #$time_local： 用来记录访问时间与时区；
    #$request： 用来记录请求的url与http协议；
    #$status： 用来记录请求状态；成功是200，
    #$body_bytes_sent ：记录发送给客户端文件主体内容大小；
    #$http_referer：用来记录从那个页面链接访问过来的；
    #$http_user_agent：记录客户浏览器的相关信息；
    #通常web服务器放在反向代理的后面，这样就不能获取到客户的IP地址了，通过$remote_add拿到的IP地址是反向代理服务器的iP地址。反向代理服务器在转发请求的http头信息中，可以增加x_forwarded_for信息，用以记录原有客户端的IP地址和原来客户端的请求的服务器地址。
    log_format access '$remote_addr - $remote_user [$time_local] "$request" '
    '$status $body_bytes_sent "$http_referer" '
    '"$http_user_agent" $http_x_forwarded_for';
     
    #定义本虚拟主机的访问日志
    access_log  /usr/local/nginx/logs/host.access.log  main;
    access_log  /usr/local/nginx/logs/host.access.404.log  log404;
     
    #对 "/" 启用反向代理
    location / {
        proxy_pass http://127.0.0.1:88;
        proxy_redirect off;
        proxy_set_header X-Real-IP $remote_addr;
         
        #后端的Web服务器可以通过X-Forwarded-For获取用户真实IP
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
         
        #以下是一些反向代理的配置，可选。
        proxy_set_header Host $host;

        #允许客户端请求的最大单文件字节数
        client_max_body_size 10m;

        #缓冲区代理缓冲用户端请求的最大字节数，
        #如果把它设置为比较大的数值，例如256k，那么，无论使用firefox还是IE浏览器，来提交任意小于256k的图片，都很正常。如果注释该指令，使用默认的client_body_buffer_size设置，也就是操作系统页面大小的两倍，8k或者16k，问题就出现了。
        #无论使用firefox4.0还是IE8.0，提交一个比较大，200k左右的图片，都返回500 Internal Server Error错误
        client_body_buffer_size 128k;

        #表示使nginx阻止HTTP应答代码为400或者更高的应答。
        proxy_intercept_errors on;

        #后端服务器连接的超时时间_发起握手等候响应超时时间
        #nginx跟后端服务器连接超时时间(代理连接超时)
        proxy_connect_timeout 90;

        #后端服务器数据回传时间(代理发送超时)
        #后端服务器数据回传时间_就是在规定时间之内后端服务器必须传完所有的数据
        proxy_send_timeout 90;

        #连接成功后，后端服务器响应时间(代理接收超时)
        #连接成功后_等候后端服务器响应时间_其实已经进入后端的排队之中等候处理（也可以说是后端服务器处理请求的时间）
        proxy_read_timeout 90;

        #设置代理服务器（nginx）保存用户头信息的缓冲区大小
        #设置从被代理服务器读取的第一部分应答的缓冲区大小，通常情况下这部分应答中包含一个小的应答头，默认情况下这个值的大小为指令proxy_buffers中指定的一个缓冲区的大小，不过可以将其设置为更小
        proxy_buffer_size 4k;

        #proxy_buffers缓冲区，网页平均在32k以下的设置
        #设置用于读取应答（来自被代理服务器）的缓冲区数目和大小，默认情况也为分页大小，根据操作系统的不同可能是4k或者8k
        proxy_buffers 4 32k;

        #高负荷下缓冲大小（proxy_buffers*2）
        proxy_busy_buffers_size 64k;

        #设置在写入proxy_temp_path时数据的大小，预防一个工作进程在传递文件时阻塞太长
        #设定缓存文件夹大小，大于这个值，将从upstream服务器传
        proxy_temp_file_write_size 64k;
    }
```

​         
​        #设定查看Nginx状态的地址
​        location /NginxStatus {
​            stub_status on;
​            access_log on;
​            auth_basic "NginxStatus";
​            auth_basic_user_file confpasswd;
​            #htpasswd文件的内容可以用apache提供的htpasswd工具来产生。
​        }
​         
​        #本地动静分离反向代理配置
​        #所有jsp的页面均交由tomcat或resin处理
​        location ~ .(jsp|jspx|do)?$ {
​            proxy_set_header Host $host;
​            proxy_set_header X-Real-IP $remote_addr;
​            proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
​            proxy_pass http://127.0.0.1:8080;
​        }
​         
​        #所有静态文件由nginx直接读取不经过tomcat或resin
​        location ~ .*.(htm|html|gif|jpg|jpeg|png|bmp|swf|ioc|rar|zip|txt|flv|mid|doc|ppt|
​        pdf|xls|mp3|wma)$
​        {
​            expires 15d; 
​        }
​         

```
    location ~ .*.(js|css)?$
    {
        expires 1h;
    }
}
```

}
######Nginx配置文件nginx.conf中文详解#####

# CreateEdgeInteractor.js

我们通过 ht.Default.def 自定义了 CreateEdgeInteractor 类，然后通过 graphView.setInteractors([ new CreateEdgeInteractor(graphView, 'points')]) 这种方式来添加 graphView 拓扑图中的交互器，可以实现创建连线的交互功能。

在 CreateEdgeInteractor 类中通过监听 touchend 放手后事件向 graphView 拓扑图中添加一个 edge 连线，可以通过在 CreateEdgeInteractor 函数中传参来绘制不同的连线类型，比如 “ortho” 则为折线类型：

```javascript
var CreateEdgeInteractor = function (graphView, type) {
    CreateEdgeInteractor.superClass.constructor.call(this, graphView);   
    this._type = type;
};
ht.Default.def(CreateEdgeInteractor, DNDInteractor, {//自定义类，继承 DNDInteractor，此交互器有一些基本的交互功能
    handleWindowTouchEnd: function (e) {
        this.redraw();
        var isPoints = false;
        if(this._target){
            var edge = new ht.Edge(this._source, this._target);//创建一条连线，传入起始点和终点
            edge.s({
                'edge.type': this._type//设置连线类型 为传入的参数 type 类型 参考 HT for Web 连线类型
            });
            isPoints = this._type === 'points';//如果没有设置则默认为 points 连线方式
            if(isPoints){
                edge.s({
                    'edge.points': [{//设置连线的点
                         x: (this._source.p().x + this._target.p().x)/2,
                         y: (this._source.p().y + this._target.p().y)/2
                    }]
                });                
            }
            edge.setParent(this._graphView.getCurrentSubGraph());//设置连线的父亲节点为当前子网
            this._graphView.getDataModel().add(edge); //将连线添加到拓扑图的数据容器中
            this._graphView.getSelectionModel().setSelection(edge);//设置选中该节点                        
        }
        this._graphView.removeTopPainter(this);//删除顶层Painter
        if(isPoints){
            resetDefault();//重置toolbar导航栏的状态
        }        
    }            
});
```



# CreateNodeInteracto节点原生遍历

# HT

你好，刚好昨天看到一篇博客，是讲这个东西。“ht是基于[HTML5](https://link.zhihu.com/?target=http%3A//dev.w3.org/html5/spec/)标准的企业应用图形界面一站式解决方案， 其包含通用组件、拓扑组件和3D渲染引擎等丰富的图形界面开发类库，提供了完全基于`HTML5`的矢量编辑器、拓扑编辑器及 3D场景编辑器等多套可视化设计工具，和完善的类库开发手册、工具使用手册、及针对`HTML5`技术如何进行大规模团队开发的客户深度培训手册。”摘自它的官网，本来想照着博客的样子也做一个类似的东西，不过后面发现这个东西并不开源，如果需要使用的话，需要（请发送邮件至 [service@hightopo.com](mailto:service@hightopo.com?subject=申请试用)(为了避免被当作垃圾邮件，请将邮件标题指定为：申请试用)，注明您的称呼、公司名称、联系方式(邮箱及电话)等，我们会尽快联系您



作者：疯一般的小猪仔
链接：https://www.zhihu.com/question/265185156/answer/343719496
来源：知乎
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

![image-20211116105459551](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116105459551.png)

# hover

![image-20211116141303883](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116141303883.png)

# mixin

两个文件公用一个配置，提高代码的复用性

## 注意：如果被混合的地方有数据或者其他东西，那么混合的时候不会替换只会合并，如果你有的则不会破坏你的。

![image-20211116144722550](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116144722550.png)

![image-20211116144731100](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116144731100.png)

![image-20211116145306116](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116145306116.png)

![image-20211116145331998](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116145331998.png)

# 插件Vue.use(install)

![image-20211116150423681](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116150423681.png)

![image-20211116150516792](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116150516792.png)

# 组件的简写方式

![image-20211116152942798](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116152942798.png)

![image-20211116153453187](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116153453187.png)

vue组件的本质是一个vuecomponent构造函数。

![image-20211116155459763](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116155459763.png)

![image-20211116155916886](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116155916886.png)

# render函数

使用render函数的原因是因为在脚手架中是不完整版的没有模板解析器需要使用render函数代替模板解析器。

![image-20211116185144706](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116185144706.png)

# ref

id的替代者，可以给组件打标识

# props

![image-20211116191050081](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116191050081.png)

在组件传值的时候加冒号后传的值是引号里面的表达式

![image-20211116191242448](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116191242448.png)

对传入的值进行限制

# scoped

所有组件的样式到最后都会汇总到一起

![image-20211116193611968](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116193611968.png)

# 路由

# ![image-20211116200815096](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116200815096.png)路由传值

![image-20211116211432519](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116211432519.png)

第二种写法

![image-20211116211607755](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116211607755.png)

![image-20211116211717923](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116211717923.png)

# 命名路由

![image-20211116211929115](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116211929115.png)

![image-20211116212030802](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116212030802.png)

![image-20211116212129563](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116212129563.png)

![image-20211116212341129](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116212341129.png)

# params参数

![image-20211116212520651](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116212520651.png)

![image-20211116212622500](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116212622500.png)

![image-20211116213057483](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116213057483.png)

![image-20211116213107639](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116213107639.png)

![image-20211116213118854](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116213118854.png)

# 路由的props

![image-20211116213606905](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116213606905.png)

![image-20211116213909640](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116213909640.png)

![image-20211116213954266](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116213954266.png)

![image-20211116214024768](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116214024768.png)

# router-link的replace属性

![image-20211116214402305](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116214402305.png)

![image-20211116214457911](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116214457911.png)

# 编程式路由导航

![image-20211116214943423](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116214943423.png)

![image-20211116215037779](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116215037779.png)

![image-20211116215706248](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116215706248.png)

![image-20211116215905455](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116215905455.png)

# 缓存路由组件

![image-20211116220328323](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116220328323.png)

其中News是组件名

![image-20211116220523825](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116220523825.png)

![image-20211116220641667](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116220641667.png)

# 路由专有的生命周期钩子

![image-20211116220950168](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116220950168.png)

![image-20211116221227775](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116221227775.png)

# 路由守卫

![image-20211116221921231](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116221921231.png)

# meta 路由元信息，程序员自定义的信息

![image-20211116223020915](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116223020915.png)

# 后置路由守卫

![image-20211116223344423](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116223344423.png)

# 独享路由守卫

![image-20211116224050788](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116224050788.png)

独享路由守卫只有前置，没有后置

# 组件内路由守卫

![image-20211116224454063](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116224454063.png)

# history模式与hash模式

![image-20211116224917109](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116224917109.png)

hash值不会随着http请求发给服务器、

hash有#，history没有#号

# this.$router.go()、back、push、replace

this.$router.go(-1)
原页面表单中的内容会丢失；
向前或者向后跳转n个页面，n可为正整数或负整数

this.$router.go(-1)：后退+刷新

this.$router.go(0)：刷新；

this.$router.go(1) ：前进

this.$router.back()
原页表表单中的内容会保留

this.$router.back():后退 ；

this.$router.back(0) 刷新；

this.$router.back(1)：前进

this.$router.push
跳转到指定url路径，并想history栈中添加一个记录，点击后退会返回到上一个页面

1. 不带参数

this.$router.push(’/home’)
this.$router.push({name:‘home’})
this.$router.push({path:’/home’})
2. query传参

this.$router.push({name:‘home’,query: {id:‘1’}})
this.$router.push({path:’/home’,query: {id:‘1’}})
html 取参 $route.query.id
script 取参 this.$route.query.id
3. params传参

this.$router.push({name:‘home’,params: {id:‘1’}}) // 只能用 name
路由配置 path: “/home/:id” 或者 path: “/home:id” ,
不配置path ,第一次可请求,刷新页面id会消失
配置path,刷新页面id会保留
html 取参 $route.params.id
script 取参 this.$route.params.id
4. query和params区别

query类似 get, 跳转之后页面 url后面会拼接参数,类似?id=1, 非重要性的可以这样传,
params类似 post, 跳转之后页面 url后面不会拼接参数 , 但是刷新页面id 会消失,密码之类还是用params刷新页面
this.$router.replace
跳转到指定url路径，但是history栈中不会有记录，点击返回会跳转到上上个页面 (就是直接替换了当前页面)【A----->B----->C 结果B被C替换 A----->C)】
————————————————
版权声明：本文为CSDN博主「半生过往」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/estrusKing/article/details/123675632

# $nextTick

![image-20211116232518485](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211116232518485.png)

# 全局事件通讯

任意组件之间通信

![image-20211117104425365](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117104425365.png)

# 登录验证码login.js

![image-20211117112038251](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117112038251.png)

![image-20211117112309129](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117112309129.png)

![image-20211117112435861](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117112435861.png)

# 登录页面布局

![image-20211117141109365](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117141109365.png)

![image-20211117141235670](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117141235670.png)

git checkout -b login 创建字分支

# 路由中的懒加载

![image-20211117142911030](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117142911030.png)

require: 运行时调用，理论上可以运用在代码的任何地方，
import：编译时调用，必须放在文件开头

懒加载：component: resolve => require(['@/view/index.vue'], resolve)
用require这种方式引入的时候，会将你的component分别打包成不同的js，加载的时候也是按需加载，只用访问这个路由网址时才会加载这个js

非懒加载：component: index
如果用import引入的话，当项目打包时路由里的所有component都会打包在一个js中，造成进入首页时，需要加载的内容过多，时间相对比较长

vue的路由配置文件(routers.js)，一般使用import引入的写法，当项目打包时路由里的所有component都会打包在一个js中，在项目刚进入首页的时候，就会加载所有的组件，所以导致首页加载较慢，

而用require会将component分别打包成不同的js，按需加载，访问此路由时才会加载这个js，所以就避免进入首页时加载内容过多。
————————————————
版权声明：本文为CSDN博主「余_小凡」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/weixin_37380784/article/details/99671933

# 路由重定向

![image-20211117143237040](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117143237040.png)

![image-20211117143721036](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117143721036.png)

CSS伪元素

/*定义滚动条高宽及背景 高宽分别对应横竖滚动条的尺寸*/
::-webkit-scrollbar
{
	width: 16px;
	height: 16px;
	background-color: #F5F5F5;
}

/*定义滚动条轨道 内阴影+圆角*/
::-webkit-scrollbar-track
{
	-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
	border-radius: 10px;
	background-color: #F5F5F5;
}

/*定义滑块 内阴影+圆角*/
::-webkit-scrollbar-thumb
{
	border-radius: 10px;
	-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,.3);
	background-color: #555;
}

# Scss/Scass

Scss是一种兼容CSS并且比CSS功能更强大的一种样式

Sacss中引入了变量，变量用$来标识，这样使得样式属性可以被复用。

在scss中重复写样式是特别烦恼的事情

如下

```
#content article h1 { color: #333 }
#content article p { margin-bottom: 1.4em }
#content aside { background-color: #EEE }
```

```
面这种是SCSS采用的嵌套CSS方法来使得CSS样式中除去了冗余的部分
#content {
  article {
    h1 { color: #333 }
    p { margin-bottom: 1.4em }
  }
  aside { background-color: #EEE }
}
```

父选择器的标识符&

```
article a {
  color: blue;
  &:hover { color: red }
}

```

用了&后被解析为

```
article a { color: blue }
article a:hover { color: red }

```



群组选择器的嵌套

```
.container h1, .container h2, .container h3 { margin-bottom: .8em }

```

```
.container {
  h1, h2, h3 {margin-bottom: .8em}
}

```

子组合选择器和同层组合选择器：>、+和~;

嵌套属性

```
nav {
  border: {
  style: solid;
  width: 1px;
  color: #ccc;
  }
}

```



```
nav {
  border: 1px solid #ccc {
  left: 0px;
  right: 0px;
  }
}

```

@import

![image-20211117192953694](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117192953694.png)

`css`有一个特别不常用的特性，即`@import`规则，它允许在一个`css`文件中导入其他`css`文件。然而，后果是只有执行到`@import`时，浏览器才会去下载其他`css`文件，这导致页面加载起来特别慢。

`sass`也有一个`@import`规则，但不同的是，`sass`的`@import`规则在生成`css`文件时就把相关文件导入进来。这意味着所有相关的样式被归纳到了同一个`css`文件中，而无需发起额外的下载请求。另外，所有在被导入文件中定义的变量和混合器（参见2.5节）均可在导入文件中使用。

@mixin

如果你的整个网站中有几处小小的样式类似（例如一致的颜色和字体），那么使用变量来统一处理这种情况是非常不错的选择。但是当你的样式变得越来越复杂，你需要大段大段的重用样式的代码，独立的变量就没办法应付这种情况了。你可以通过`sass`的混合器实现大段样式的重用。

混合器使用`@mixin`标识符定义。看上去很像其他的`CSS @`标识符，比如说`@media`或者`@font-face`。这个标识符给一大段样式赋予一个名字，这样你就可以轻易地通过引用这个名字重用这段样式。下边的这段`sass`代码，定义了一个非常简单的混合器，目的是添加跨浏览器的圆角边框。

```
@mixin rounded-corners {
  -moz-border-radius: 5px;
  -webkit-border-radius: 5px;
  border-radius: 5px;
}

```

```
notice {
  background-color: green;
  border: 2px solid #00aa00;
  @include rounded-corners;
}

```

```
.notice {
  background-color: green;
  border: 2px solid #00aa00;
  -moz-border-radius: 5px;
  -webkit-border-radius: 5px;
  border-radius: 5px;
}

```

混入器中的CSS规则

```
@mixin no-bullets {
  list-style: none;
  li {
    list-style-image: none;
    list-style-type: none;
    margin-left: 0px;
  }
}

```

```
ul.plain {
  color: #444;
  @include no-bullets;
}

```

```
ul.plain {
  color: #444;
  list-style: none;
}
ul.plain li {
  list-style-image: none;
  list-style-type: none;
  margin-left: 0px;
}

```

给混合器传参

混合器并不一定总得生成相同的样式。可以通过在`@include`混合器时给混合器传参，来定制混合器生成的精确样式。当`@include`混合器时，参数其实就是可以赋值给`css`属性值的变量。如果你写过`JavaScript`，这种方式跟`JavaScript`的`function`很像：

```
@mixin link-colors($normal, $hover, $visited) {
  color: $normal;
  &:hover { color: $hover; }
  &:visited { color: $visited; }
}

```

```
a {
  @include link-colors(blue, red, green);
}

//Sass最终生成的是：

a { color: blue; }
a:hover { color: red; }
a:visited { color: green; }

```

当你@include混合器时，有时候可能会很难区分每个参数是什么意思，参数之间是一个什么样的顺序。为了解决这个问题，`sass`允许通过语法`$name: value`的形式指定每个参数的值。这种形式的传参，参数顺序就不必再在乎了，只需要保证没有漏掉参数即可：

```
a {
    @include link-colors(
      $normal: blue,
      $visited: green,
      $hover: red
  );
}

```

# before/after选择器

![](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20211117194546710.png)

# this.$set(1,2,3)

 ```xml
1、对象
2、向对象中添加某个字段属性或向或个字段设置值
3、对应2字段的值
 ```



# vue关闭当前路由返回上一页

```xml
back() {
      this.$store.state.tagsView.visitedViews.splice(this.$store.state.tagsView.visitedViews.findIndex(item => item.path === this.$route.path), 1)
      this.$router.push(this.$store.state.tagsView.visitedViews[this.$store.state.tagsView.visitedViews.length - 1].path)
    }
```

# Vue中导出到Excel时显示为科学计数法怎么解决

```xml
   '二维码编码': {
          field: 'qrcode',
          callback: value => {
            return '&nbsp;' + value
          }
        },
```

# Z-Index

```xml
菜鸟上路有点区分不了z-index和！important的区别，所以就研究了一下：
z-index的用法就是：

                          样式中有position属性值为absolute、relative或baifixed导致了页面重叠把想显示的页面给遮住了，这个是后就可以设置z-index值（想显示在上面的值要设置比被遮盖的页面z-index值大）就可以解决了。

!important的用法是： 

                            提高指定样式的优先级，有的时候你的样式是会被其他的样式给遮盖，这是因为你的样式权重不够，那这个时候有两个解决方法，

                           一：是通过选择器来添加权重，不过这个太过于麻烦，代码太长了。

                           二：可以在你想要的显示的样式后面加 ！important  ，这样代码少简单方便
————————————————
版权声明：本文为CSDN博主「干净洁」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/ganjingjie/article/details/106709256
```

# 嵌套按钮

```xml
   <el-dropdown trigger="click" placement>
          <el-button class="filter-item" type="primary" size="mini" icon="el-icon-download" @click="editEquipment">
            导出
            <i class="el-icon-arrow-down el-icon--right" />
          </el-button>
          <el-dropdown-menu slot="dropdown" style="margin-left:30px">
            <el-dropdown-item>
              <el-button
                v-if="operationType !== 'view'"
                id="portPanelViewBtn"
                :disabled="viewPortFlag"
                :loading="loading"
                class="filter-item"
                size="mini"
                type="primary"
                icon="el-icon-download"
                @click="viewPort($event)"
              >
                导出光缆
              </el-button>
              <el-dropdown-item>
                <el-button
                  v-if="operationType !== 'view'"
                  id="portPanelViewBtn"
                  :disabled="viewPortFlag"
                  :loading="loading"
                  class="filter-item"
                  size="mini"
                  type="primary"
                  icon="el-icon-download"
                  @click="viewPort($event)"
                >
                  导出电缆
                </el-button>
              </el-dropdown-item></el-dropdown-item></el-dropdown-menu>
        </el-dropdown>
```

1. **0**:

2. 1. **CODE**: "XSQ.081/GJ082060/PXG00015"
   2. **CREATE_DATE**: "2016-05-31 15:57:19"
   3. **ID**: "531000000000002277998661"
   4. **MODIFY_DATE**: "2016-05-31 15:57:19"
   5. **NAME**: "081/GJ082060/PXG00015"
   6. **ORDER_NUM**: "100"
   7. **RELATIONS**: {CREATE_DATE: '2022-04-23 03:09:12', CODE: '', MODIFY_DATE: '2022-04-23 03:09:12', SPEC_ID: '1210111210000', ID: '531000100000006589882923', …}
   8. **R_ID**: "531000100000006589882923"
   9. **SPEC_ID**: "1211200002"
   10. **SPEC_ID_NAME**: "光缆"
   11. **TIME_STAMP**: "2022-04-23 02:42:51.52515"
   12. **USING_STATE_ID**: "100723"
   13. **USING_STATE_ID_CODE**: "3"
   14. **USING_STATE_ID_ID**: "100723"
   15. **USING_STATE_ID_NAME**: "占用"
   16. **USING_STATE_ID_OBJECT**: {USING_STATE_ID-code: '3', USING_STATE_ID-name: '占用', USING_STATE_ID-id: '100723'}
   17. [[Prototype]]: Object

# el-tree默认展开第一级

![1652075867207](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\1652075867207.png)

# JS中对对象数组

```
const removeDuplicateObj = (arr) => {
              const obj = {}
              arr = arr.reduce((newArr, next) => {
                obj[next.entityId] ? '' : (obj[next.entityId] = true && newArr.push(next))
                return newArr
              }, [])
              return arr
            }
            console.log('过滤后的数据', removeDuplicateObj(wellInfo))
```

# JS中的排序函数

```xml
 data.sort(this.sortBy('start_port'))
```

