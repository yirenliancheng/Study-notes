# Diff算法

Diff算法分为3层：

* tree diff

​      新旧两棵DOM树，逐层对比的过程，就是Tree Diff；当整棵DOM逐层对比完毕，则所有需要被更新的元素，必然能找到。

* component diff

​      在进行Tree diff的时候，每一层中，组件急别的对比，叫做Component Diff:

​      如果类型相同，则暂时认为该组件不需要被更新；

​      如果类型不同，则需要移除旧组件，创建新组件，并追加到页面上。

* element diff

​      在进行组件对比的时候，如果两个组件类型相同，则需要进行元素级别的对比，叫做Element Diff。

![image-20200711191652298](C:\Users\76110\AppData\Roaming\Typora\typora-user-images\image-20200711191652298.png)











