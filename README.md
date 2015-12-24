# -
    // Objective-C 
    cd LeanStorageDemoObjc
    # 如果提示找不到库，则可去掉 --no-repo-update
    pod install --verbose --no-repo-update 
    open LeanStorageDemo.xcworkspace

    // Swift
    cd LeanStorageDemoSwift
    pod install --verbose --no-repo-update
    open LeanStorageDemoSwift.xcworkspace
    AVOSCloud.framework 静态库支持 iOS6 以上的设备上，Demo 也是使用的静态库， Demo 中设置的默认运行设备是 iOS7 以上，
    如果要在 iOS6 的设备上运行，只需修改 Xcode 里的 Deployment Target 为 iOS6 即可。另外注意，因为动态库只支持 iOS8 以上的设备
    ，如果使用了 AVOSCloud.framework 动态库， Deployment Target 必须为 iOS8 以上 。
    用 账号/密码 (leancloud@163.com/Public123) 登录 https://leancloud.cn ，选择应用 LeanStorage-Demo ，即可查看后台数据。
    强烈建议你边查看后台边运行 Demo。当在 Demo 运行代码来增删改查时，就可以在后台看到相应的数据变化。
    编译警告

代码中有一些人为添加的编译,是为了引起您足够的重视, 如果觉得没问题可以删除掉该行

添加Demo

新建一个继承Demo的类, 文件位置在项目的LeanStorageDemo文件夹
在.m里的@end前加一句MakeSourcePath 用来在编译时生成返回这个文件的方法
加一个demo方法. 方法必须以demo开头, 且必须是严格按照骆驼命名法, 否则方法名显示可能会有问题

原文https://github.com/leancloud/LeanStorageDemo-iOS
