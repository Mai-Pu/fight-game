# fight-game
战斗小游戏-Java实现-设计模式

## 模式及使用场景


1. 构建Stage场景时，用创建者模式✅
2. 创建角色时，使用工厂方法模式(工厂方法模式、抽象工厂模式)✅
3. 将人及各类角色加入场景时，使用原型模式进行clone✅
4. 构建装备合成时，使用组合模式✅
5. 进行文件存储时，使用单例模式✅
   维护一个列表，用于查找系统中的现有角色，以进行挑战，使用单例模式⬆️☑️
6. 背包系统，采用迭代器模式✅
7. 攻击指令可使用解释器模式解释❌
8. 使用状态模式，用以标识目标的状态✅
9. 技能的泛化使用策略模式❌
10. 技能点组合，使用命令模式进行组合，可以撤销❌
11. 在进行伤害整合时，采用外观模式，因为伤害来自于：目标本身的自带伤害、技能伤害、武器造成的伤害、装备的附加伤害✅
12. 在进行战斗时，利用中介者模式，对战斗双方进行中介访问✅
13. 当健康值、能量值等可变值发生改变时，通知作出相应的变化等，采用观察者模式✅
14. 在攻击前或进行操作前，需要检查合法性等，所以使用代理模式，在执行前后加上检查✅
15. 武器可以添加配件，因此可以使用装饰模式✅
16. 在进行伤害计算时，使用适配器模式，将伤害计算接口统一✅
17. 使用备忘录模式，存储当前目标状态信息✅
18. 在构建模型到表模型转换工具的时候，使用享元模式✅
19. 构建模型转换工具时，不同的模型类需要不同的映射文件，使用模板方法模式，动态化子类映射文件获取✅
20. service类的处理，使用桥接模式，以实现业务处理和内部接口实现和抽象的分离✅
21. 由于攻击方式不同，如果通过索引去确定攻击方式，属于硬编码，使用策略模式进行改进🔘



## 可能的需求改变对模式的破坏

问题：当增加角色类型时，计算伤害的方法将需要被修改


