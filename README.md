**LuckyCI**
===================

LuckyCI是基于C#开发的，运行在Windows平台上的持续集成工具(CI)。目前可以对SVN版本库上的Android Studio, Apache Cordova, .NET项目进行监控并持续集成（Build）。集成结果可以通过**邮件**或**Slack**自动发送给团队成员，从而时刻确保项目完整性，让开发过程更加高效。

功能简介
-------------

> - LuckyCI提供**Windows应用程序**和**Windows Service**两种运行模式,在**Windows客户**中可以通过GUI界面对运行环境和项目进行配置，测试，并监控服务的运行状态, 在**Windows Service**可以在后台运行CI服务，对项目进行持续集成。
> - LuckyCI提供了实时查看信息功能,用户可以查看操作执行的详细结果,项目运行的日志信息以及**SVN**集成功能执行的日志信息。
> - LuckyCI提供了消息实时推送功能,用户可以主动发送也可以在服务器端配置推送项目实时运行情况 (目前支持**邮件**以及**slack**)。

管理项目
-------------

LuckyCI中已经为用户添加了三个项目样例(.Net , Cordova , AndroidStudio),以便用户参考使用,样本样例无法进行正常SVN操作及项目操作,仅供参考学习。

####<i class="icon-pencil"></i>运行环境的配置

点击<kbd>Option</kbd>进入配置页面,选取本地svn.exe路径,输入检测项目的时间周期,选择是否输出标准信息(若不勾选,成功的日志中则只会显示结果),最后在Windows和Service中二选一进行监控吧。

####<i class="icon-pencil"></i>邮件与Slack的配置

如果用户想及时收到消息的推送以便监控项目的情况,可以配置邮件或Slack。
> - 邮件需要用户修改默认域名,输入相应服务器地址,若不更改用户名LuckyCI将会使用SVN的对应项目提交Author作为默认此时用户无需输入密码。
> - Slack则需要用户在Slack提供的Incoming WebHooks页面找到团队的Webhook URL,同时在页面也可以对消息机器人进行简单配置。同样如果不设置用户名我们将默认使用SVN的Author

#### <i class="icon-pencil"></i> 项目修改

点击<kbd>File</kbd>进入项目监测页面,在当前页用户可以对Service的状态进行查看及操作,查看配置好的项目的历史日志信息,单击(或双击)选中项目列表中的项目进入修改模式,修改完后点击<kbd>Save</kbd>进行保存。

#### <i class="icon-pencil"></i> 帮助文档

点击<kbd>Help</kbd>查看帮助文档,解决一些在AndroidStudio出现的一些常见问题。
