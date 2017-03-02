# Software-Engineering
NKU-软件工程课程设计2017

一、項目描述：
该项目工程的目标是为私有的中小餐饮企业提供一种自动化业务运行模式。现阶段餐饮人员面临的主要问题有如何：
1)协调不同餐馆中不同角色的工作活动
2）估计并处理高低峰时段顾客拥挤情况
3）尽早发现畅销菜品，增大供应提高利润；同时尽早发现不受欢迎的菜品，减少供应，节约成本。
4）降低人工操作成本，增加效率和利润

落伍的餐馆运行模式：
1、顾客进入餐馆，引导员欢迎、查看黑板是否有空桌、实时更新黑板上信息，带入就坐。
2、顾客就坐，服务员在复写纸上速记点的菜品，送到厨房，厨房准备食材。
3、服务生定时反复查看餐品是否准备好。
4、餐品全送上桌后，点菜单存根统一管理。

落伍的方式：会产生大量的点菜单，浪费很多时间进行管理分析，是非常低效的。在这种模式下，服务生总是拿着小板，配着签字笔等待点菜，同时还需要记录每一桌与之对应的账单。

另一个棘手的问题是：记录管理和存储。在老的系统里，所有信息都记录在纸上，组织、存储和分析这些记录，从中得出有用信息将会耗费巨大的时间和人力开销。

该项目用电脑处理餐厅中的那些操作，所有订单和员工的操作可以很便利地实现共享，并且存储在餐厅的内联网中。引导员也可以通过点击按钮
查看餐桌的状态，服务生可以快捷而高效地记录顾客的点菜单，并通过网络直接传送到厨房。厨房员工（厨师）可以查看点的菜品，在做好菜之后通知正确的服务生。餐厅侍者助手（bus boy）可以实时查看餐厅平面图中显示的餐桌状态，可以及时了解哪些桌子是干净的、肮脏的或者被占用着的。更值得注意的是，所有餐厅信息都被组织和存储在系统数据库中来查看管理和存档的。而对于数据的分析也可以分成每天分析和每小时分析等不同粒度的，主要分析：1）营业利润，每道菜产生的利润所占比重 2）菜品受欢迎程度 3）员工工作效率 4）平均用餐时间 5）每桌菜品的平均准备时间

这种新的系统避免了使用大量的纸张，也减少了处理数据耗费的巨大时间成本。所有的数据都可以被自动地收集和处理，使得在管理能够更专注于对数据的分析而不是数据的计算。

二、粗糙的需求分析
根据问题的说明材料，我们设计的系统应该具有具有一般性，即不是针对每一个特定的餐厅，而是设计一个框架结构，可以适用于餐桌布局、餐品不同的不同餐厅。在设计时，不应该给定死，实现基本的功能要求，并且有一定的适用推广能力
。

1）餐厅员工使用平板点餐。平板上通过给餐桌标识不同的颜色区分其状态，绿色表示可使用，黄色表示正在使用中，红色表示脏桌子。
2）餐厅的雇员角色可分为：引导员、服务生、厨师、侍者助手和经理。具有直接联系的员工有：引导员和服务生、服务生和厨师，侍者助手和引导员。每一类角色在系统中都应该有自己的权限。平板上的信息需要要同时同步更新。
3）经理具有管理对雇员的管理权限：新建和修改雇员信息，跟踪雇员活动、授权被限制的服务生活动（authorize restricted waiter activities）、存货跟踪、销售分析。
4）关于服务员用的计算机终端类型选择：固定的电脑终端和手持终端

5）系统使用用户认证（touch screen,card reader,typical keyboard）

6)餐厅平面图是否可改变，以应用于不同场景

7）系统记录雇员的工作时长，能够快速处理工资单

8）快捷键设置，提高效率

9）实地调研




