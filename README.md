HTTP：//railsapps.github.io/images/rails-36x36.jpg（Rails应用程序的子域与设计）！ Rails应用程序的子域与设计

Rails的3.2示例应用程序演示如何使用子域名与设计进行验证。

*“设计”：HTTP：//github.com/plataformatec/devise给你现成的认证和用户管理。
* MongoDB是用作与“Mongoid”数据存储：HTTP：//mongoid.org/创业板的快速发展没有模式或迁移。

最重要的是，有一个“详细教程”：HTTP：//railsapps.github.io/tutorial-rails-subdomains.html展示它是​​如何构建的。

你可以建立一个使用“Rails的作曲家”中只有几分钟这个应用程序：http：//railsapps.github.io/rails-composer/工具。

H2。 ！HTTP：//twitter-badges.s3.amazonaws.com/t_logo-a.png（在Twitter）：HTTP：//www.twitter.com/rails_apps在Twitter关注

在Twitter项目：“@rails_apps”：HTTP：//twitter.com/rails_apps。请鸣叫一些好评，如果你喜欢你发现了什么。

H2。教程

一个完整的演练教程可在GitHub上的wiki：

H4。 “查看教程”：HTTP：//railsapps.github.io/tutorial-rails-subdomains.html

教程文件的每一步跟着来创建应用程序。每一步都被记录简明扼要，所以一个完整的初学者也可以创建这个应用程序，无需任何额外的知识。但是，没有解释提供任何步骤，所以如果你是一个初学者，我们建议你找一个引入到别处轨。请参阅“Rails的”推荐资源列表：HTTP：//railsapps.github.io/rails.html。

H2。什么是实现 - ，什么是不

该示例应用程序实现了一个共同使用子域名，通常被称为“在Rails的大本营式的子域。”游客到主站点创建一个托管在一个子域匹配的用户名的用户帐户。每个用户只有一个子域名和登录时，他们所有的活动仅限于自己的子域名。

另一种常见的使用子域名可以被称为“博客风格的子域。”这种方法是熟悉的网站，如wordpress.com的用户，每个用户都可以创建多个博客，每个托管在自己的子域。例如，与电子邮件地址“用户@ example.com @”一个用户可以拥有多个博客，例如，“puppyphotos.wordpress.com”和“kittenphotos.wordpress.com”。而“博客风格的子域”的做法是不是在这个示例应用程序实现的。

H4。 RailsApps示例和教程

这是在一系列的Rails应用程序示例和教程从“RailsApps工程”：HTTP：//railsapps.github.io/。看到额​​外的“Rails的例子，教程和起动应用程序”列表：HTTP：//railsapps.github.io/rails-examples-tutorials.html。

H2。依赖

运行这个程序之前，您需要：

* Ruby语言（1.9.3版或2.0.0）
* Rails的宝石（版本3.2.13）
*“的MongoDB的”工作安装：HTTP：//www.mongodb.org/（1.6.0版或更新版本）

请参阅文章“安装滑轨”：HTTP：//railsapps.github.io/installing-rails.html咨询有关更新Rails和你的开发环境。

H4。 MongoDB的安装

如果您没有安装在计算机上的MongoDB，你需要安装它，将它设置为始终在您的计算机上运行（运行在发射）。在Mac OS X，安装MongoDB的最简单的方法是安装“家酿”：HTTP：//mxcl.github.com/homebrew/，然后运行以下命令：

<前>
BREW MongoDB的安装
</ PRE>

家酿将提供安装后指示，以获得MongoDB的运行。安装输出的最后一行显示了MongoDB的安装位置（例如，*的/ usr /本地/库/ MongoDB的/ 1.8.0-x86_64的*）。你会发现MongoDB的配置文件存在。使用自制软件的安装后，默认的数据目录将成为*的/ usr /本地的/ var / MongoDB的*。

H2。获取应用程序

你有几个选项获取的代码。

H3。叉

如果你想添加的功能（或错误修复），以提高示例应用程序，您可以用叉子叉GitHub的回购和“做拉请求”：HTTP：//help.github.com/send-pull-requests/。你的代码贡献，欢迎！

H3。克隆

如果要复制，并与你自己的项目是唯一有用的变化自定义应用程序，您可以克隆GitHub的回购。你需要搜索和替换整个应用程序的项目名称。你或许应该生成的应用程序，而不是（见下文）。克隆：

<前>
$混帐混帐克隆：//github.com/RailsApps/rails3-subdomains.git
</ PRE>

你需要“混帐”：您的机器上//git-scm.com/：HTTP。请参阅“Rails和混帐”：HTTP：//railsapps.github.io/rails-git.html。

H3。生成

如果你想使用的项目作为启动的应用程序，使用“Rails的作曲家”：HTTP：//railsapps.github.io/rails-composer/工具生成的示例应用程序的新版本。你就可以在生成的应用程序给它自己的项目名称。生成的应用程序为您提供了许多额外的选项。

要构建示例应用程序，运行以下命令：

<前>
$导轨新rails3，子域-m https://raw.github.com/RailsApps/rails-composer/master/composer-Rails3_2.rb -T -O
</ PRE>

使用@ -T -O @标志来跳过测试::单位的文件和活动记录文件。

该@ $ @字符表示shell提示符;不包括它，当你运行该命令。

这将创建一个名为@ rails3-子域名@您的计算机上新的Rails应用程序。

你会看到一个提示：

<前>
问题安装一个示例应用程序？
      1）我想建立自己的应用程序
      2）会员/订阅/萨斯
      3）导轨-发射前，注册
      4）rails3 - 引导 - 色器件，康康舞
      5）rails3-色器件-RSpec的黄瓜
      6）rails3-mongoid-色器件
      7）rails3-mongoid-omniauth
      8）rails3，子域
</ PRE>

选择* rails3-子域*。 Rails的作曲工具，可能会给你其他的选择（其他选择​​可能已添加，因为这些笔记写）。

该应用程序生成的模板将要求您提供额外优惠：

<前>
 问题的Web服务器进行开发？
       1）的WEBrick（默认）
       2）薄
       3）独角兽
       4）彪马
 问题的Web服务器进行生产？
       1）同发展
       2）薄
       3）独角兽
       4）彪马
 问题模板引擎？
       1）ERB
       2）Haml的
       3）超薄
   额外设置robots.txt文件禁止蜘蛛？ （Y / N）
   额外使用或创建一个项目特定RVM宝石？ （Y / N）
   额外创建一个GitHub的库？ （Y / N）
</ PRE>

H4。 Web服务器

使用默认的WEBrick服务器的便利。如果您计划部署到Heroku上，选择“瘦”为您的生产网络服务器。

H4。模板引擎

示例应用程序使用默认的“再培训局”Rails的模板引擎。或者，您可以使用其他的模板引擎，如Haml的或修身。请参阅“Haml的和Rails”指令：HTTP：//railsapps.github.io/rails-haml.html。

H4。其他选择

如果你想保持你的新网站走出谷歌搜索结果中设置robots.txt文件禁止蜘蛛。

这是一个好主意，用“RVM”：HTTPS：//rvm.io/，Ruby的版本管理，并创建一个项目特定RVM宝石（不能在Windows可用）。请参阅“安装滑轨”：HTTP：//railsapps.github.io/installing-rails.html。

如果您选择创建一个GitHub的资源库，生成器会提示你输入一个GitHub上的用户名和密码。

H4。故障排除

如果你得到一个错误“OpenSSL的证书验证失败”或“宝石:: RemoteFetcher :: FetchError：所以SSL_connect”见文章“OpenSSL的错误和Rails”：HTTP：//railsapps.github.io/openssl-certificate-verify-failed html的。

如果你得到一个错误是这样的：

<前>
你的包是完整的！使用`束秀[gemname]`看到安装了捆绑的宝石在哪里。
    作曲家回调“打捆后'运行。
该模板[...]无法加载。
错误：您已经激活了......，但你的Gemfile需要....
使用捆绑EXEC可能会解决这个问题。
</ PRE>

这是由于相互冲突的宝石版本。请参阅文章“Rails的错误：”您已经激活了（......）“”：HTTP：//railsapps.github.io/rails-error-you-have-already-activated.html。

其他的问题？检查“问题”：HTTPS：//github.com/RailsApps/rails3-subdomains/issues。

H3。编辑自述

如果你存储在GitHub的资源库的应用程序，请编辑README文件添加应用程序的描述，您的联系方式。如果你不改变的自述，人们会认为我是你的应用程序版本的作者。

H2。入门

H3。安装所需的宝石

检查的Gemfile看看哪些宝石使用这个应用程序。

如果你使用了“Rails的作曲家”：HTTP：//railsapps.github.io/rails-composer/工具生成的示例应用程序，该应用程序模板脚本已经运行@bundle安装@命令。

如果没有，你应该运行@bundle安装@命令来安装在计算机上的宝石要求：

<前>
$捆绑安装
</ PRE>

您可以检查哪些宝石安装在计算机上：

<前>
$创业板上市
</ PRE>

请您已经在本地安装这些宝石的头脑。当你部署应用程序到另一台服务器，同样的宝石（和版本）必须是可用的。

我建议使用“RVM”：HTTPS：//rvm.io/，Ruby的版本管理，建立项目特定的宝石为应用程序。请参阅文章“安装滑轨”：HTTP：//railsapps.github.io/installing-rails.html。

H3。配置Mongoid

Mongoid提供由轨道上的MongoDB数据库。

您可以使用文件*配置/ mongoid.yml *中的默认配置。

如果你想看看有什么在你的MongoDB数据库，我建议使用“MongoHub”：HTTP：//mongohub.todayclose.com/应用程序（用于Mac OS X）。

H3。配置电子邮件

这个示例应用程序不发送电子邮件。但是，如果你希望你的应用程序发送电子邮件（例如，如果你计划安装设计@：@可确认模块），您必须配置应用程序为您的电子邮件帐户。请参阅文章“发送电子邮件使用Rails”：HTTP：//railsapps.github.io/rails-send-email.html。

H3。配置设计

您可以修改设计配置文件，如果你想使用比默认其他的东西：

*配置/初始化/ devise.rb *

H3。配置文件

该应用程序使用“费加罗宝石”：HTTPS：//github.com/laserlemon/figaro来设置环境变量。凭据为管理员帐户和电子邮件帐户将在*配置/ application.yml *文件中设置。在* *的.gitignore文件，防止被保存在Git仓库，以便您的凭据保密的*配置/ application.yml *文件。请参阅文章“Rails环境变量”：HTTP：//railsapps.github.io/rails-environment-variables.html以获取更多信息。

修改文件*配置/ application.yml *：

<前>
＃在这里添加帐户凭据和API密钥。
＃见http://railsapps.github.io/rails-environment-variables.html
＃这个文件中应列出的.gitignore保持你的设置秘密！
＃每个条目设置一个局部环境变量，将覆盖在Unix shell的环境变量。
＃例如，设置：
＃GMAIL_USERNAME：Your_Gmail_Username
＃使'Your_Gmail_Username“作为ENV [”GMAIL_USERNAME“]
＃添加应用程序配置变量在这里，如下图所示。
＃
GMAIL_USERNAME：Your_Username
GMAIL_PASSWORD：Your_Password
ADMIN_NAME：USER1
ADMIN_EMAIL：user@example.com
ADMIN_PASSWORD：changeme
</ PRE>

如果您计划定制使用Gmail帐户发送电子邮件的应用程序，你可以添加需要发送电子邮件的应用程序的用户名和密码。请参阅文章“发送电子邮件使用Rails”：HTTP：//railsapps.github.io/rails-send-email.html。

如果你愿意，为第一用户的帐户设置你的姓名，电子邮件地址和密码。如果你喜欢，你可以使用默认的登录到应用和部署后编辑的帐户。它始终是一个好主意，将应用程序部署后更改密码。

是在*配置/ application.yml *文件中的所有配置值可在任何地方的应用程序环境变量。例如，@ENV [“GMAIL_USERNAME”] @将返回字符串“Your_Username”。

如果你愿意，你可以删除*配置/ application.yml *文件，并设置每个值作为Unix外壳的环境变量。

H3。建立一个数据库种子文件

在* DB / seeds.rb *文件初始化使用默认值的数据库。保留一些私人数据，巩固配置设置在一个位置，我们使用*配置/ application.yml *文件来设置环境变量，然后在* DB / seeds.rb *文件中使用的环境变量。

<前>
放“默认用户”
用户= User.create！ ：名称=> ENV ['ADMIN_NAME'] DUP，：电子邮件=> ENV ['ADMIN_EMAIL'] DUP，：密码=> ENV ['ADMIN_PASSWORD'] DUP，：password_confirmation => ENV ['ADMIN_PASSWORD']。 DUP
看跌期权“用户：”<< user.name
</ PRE>

您可以更改第一个用户的姓名，电子邮件和密码在此文件，但它是更好地使的变化，*配置/ application.yml *文件，以保持凭据私人。如果您决定包括在* DB / seeds.rb *文件你的私人密码，请务必将文件名添加到您的* *的.gitignore文件，使你的密码不会成为你的公共GitHub的仓库中。

请注意，这不是你需要部署应用程序之前，个性化* DB / seeds.rb *文件。你可以用一个例子用户部署应用程序，然后使用应用程序的“编辑帐户”功能更改姓名，电子邮件地址和密码登录后，使用此功能作为第一个用户登录并修改用户名和密码你自己的。

您可能希望包括额外的样本用户：

<前>
用户2 = User.create！ ：名称=>'用户2'，：电子邮件=>'user2@example.com'，：密码=>'changeme'，：password_confirmation =>'changeme“
看跌期权“用户：”<< user2.name
</ PRE>

这将第二用户添加到数据库。

H3。设置数据库

准备数据库并通过运行命令添加默认用户到数据库中：

<前>
$耙分贝：种子
</ PRE>

使用@rake DB：//补种，如果你想清空和补种的数据库。或者你可以使用@rake分贝：滴@和@rake DB：设置@。与Rails的ActiveRecord的等效任务是@rake DB：复位@这将在Mongoid 4.0。

运行测试设置数据库：

<前>
$耙分贝：测试：准备
</ PRE>

如果你不使用“RVM”：HTTPS：//rvm.io/，Ruby的版本管理，你应该前言每个瑞克命令@bundle EXEC @。你并不需要使用@bundle EXEC @如果您使用的是RVM版本1.11.0或更高版本。

H3。更改应用程序的秘密令牌

如果你使用了Rails的作曲工具生成的应用程序，该应用程序的秘密令牌将是独一无二的，就像与@rails新的@命令所产生的任何Rails应用程序。

但是，如果你直接从GitHub上克隆的应用程序，它是您将应用程序部署在生产模式前更改应用程序的秘密令牌是至关重要的。否则，人们可能会改变他们的会话信息，并可能访问您的网站未经您的许可。你的秘密令牌至少应为30个字符长，完全是随机的。

得到一个唯一的秘密令牌：

<前>
耙秘密
</ PRE>

编辑*配置/初始化/ secret_token.rb *文件中添加的秘密令牌：

<前>
Rails3Subdomains :: Application.config.secret_token ='...一些很长的，随机字符串......“
</ PRE>


H2。测试的应用程序使用子

如果你启动应用程序，它会在运行的“http：//本地主机：3000 /”：HTTP：//本地主机：3000 /或“http://0.0.0.0:3000/":http://0.0。 0.0：3000 /。但是，除非你已经取得了一些配置更改到您的计算机，您将无法解析地址，使用一个子域，如“http：//foo.localhost：3000 /”：HTTP：// foo中。本地主机：3000 /。有几种复杂解决这一问题。你可以建立自己的域名服务器上的本地主机，并创建一个A项捕获所有子域。你可以修改你的* / etc / hosts文件*文件（但它不会满足动态创建的子域）。您可以创建一个“代理自动配置（PAC）”：HTTP：//en.wikipedia.org/wiki/Proxy_auto-config文件，并将它设置为代理服务器在Web浏览器preferences.There的一个非常简单的解决方案，它不需要重新配置您的计算机或网络浏览器的偏好。开发商列维库克注册了域名，“lvh.me”：//lvh.me：3000 /（简称：本地虚拟主机我）解析为本地主机IP地址​​127.0.0.1，支持通配符，（可容纳HTTP动态创建子域）。

要测试应用程序，请访问“http://lvh.me:3000/":http://lvh.me:3000/。你应该可以看到注册用户链接到他们的个人资料页的列表。

尝试“http://user1.lvh.me:3000/":http://user1.lvh.me:3000/。您应该看到个人资料页面默认用户“user1的。”

尝试“http://foo.lvh.me:3000/":http://foo.lvh.me:3000/。您应该看到“用户未找到”的错误消息。

尝试“http://www.lvh.me:3000/":http://www.lvh.me:3000/。您应该被重定向到应用程序主页，在“http://lvh.me:3000/":http://lvh.me:3000/。

要登录为默认的用户，（除非你已经改变了它）使用

*电子邮件：user@example.com
*密码：changeme

您应该删除或更改预配置登录您部署应用程序之前。

H2。部署的Heroku

为了您的方便，这里是“部署你的应用程序的Heroku的说明”：HTTP：//railsapps.github.io/rails-heroku-tutorial.html。 Heroku的提供成本低，易于配置的Rails应用程序托管。

H2。自定义

“设计”：HTTP：//github.com/plataformatec/devise提供了多种功能，实现身份验证。请参阅设计文档的选项。

这个示例应用程序和教程演示了设计和Mongoid合作on Rails的3.添加任何模型，控制器和视图，你需要。

H2。测试

该应用程序设置为RSpec的单元测试和情景黄瓜和步骤。没有测试和场景此版本的示例应用程序的执行。请将作者信息，创建一个问题，或者提交pull请求，如果你能贡献RSpec的或黄瓜测试和情景。

安装应用程序后，运行@rake -T @检查可用于RSpec的黄瓜瑞克任务。

运行@rake规格@运行RSpec的测试。

运行@rake黄瓜@（或者更简单地说，@ @黄瓜）运行黄瓜方案和步骤。

H2。故障排除

存在的问题？检查“问题”：HTTPS：//github.com/RailsApps/rails3-subdomains/issues。

H4。有问题的“证书验证失败”

你得到一个错误“OpenSSL的证书验证失败”当您尝试生成应用程序模板一个新的Rails应用程序？见建议来解决的错误“证书验证失败”：HTTP：//railsapps.github.io/openssl-certificate-verify-failed.html。

H2。文档和技术支持

该“指南”：HTTP：//railsapps.github.io/tutorial-rails-subdomains.html提供补充文件。

对于Mongoid介绍，瑞安贝茨提供了一个“Railscast上Mongoid”：HTTP：//railscasts.com/episodes/238-mongoid。你可以找到文档“Mongoid”：HTTP：//mongoid.org/在“http://mongoid.org/":http://mongoid.org/有一个活跃的”Mongoid邮件列表“：HTTP：/ /groups.google.com/group/mongoid，你可以提交“Mongoid问题”：HTTP：//github.com/durran/mongoid/issues在GitHub上。

对于设计的介绍，瑞安贝茨提供了一个“Railscast上制定”：HTTP：//railscasts.com/episodes/209-introducing-devise。在“http://github.com/plataformatec/devise":http://github.com/plataformatec/devise //github.com/plataformatec/devise：HTTP：您可以为”设计“找到文档。有一个活跃的“设计邮件列表”：HTTP：//groups.google.com/group/plataformatec-devise，你可以提交“设计问题”：HTTP：//github.com/plataformatec/devise/issues在GitHub上。

H4。问题

请创建一个“GitHub上的问题”：HTTP：//github.com/RailsApps/rails3-subdomains/issues如果你发现任何问题或有改进建议。

H4。何处获取帮助

您最好的帮助，问题来源是“堆栈溢出”：HTTP：//stackoverflow.com/questions/tagged/ruby-on-rails-3。你的问题可能已经遇到和别人讨论。

你也可以尝试“的Rails热线”：HTTP：//www.railshotline.com/，一个免费的电话热线的Rails有助于志​​愿者。

H2。特约

如果你把改善这个应用程序，请与别人分享。

发送笔者的消息，创建一个“问题”：HTTP：//github.com/RailsApps/rails3-subdomains/issues，或派生的项目，并提交pull请求。

如果将功能添加到这个应用程序，创建一个替代实现，或者建立一个应用程序类似，请与我联系，我会添加注释自述，以便其他人可以找到你的工作。

H2。积分

感谢您对“布赖恩Cardarella”：HTTP：//bcardarella.com/为“自定义子域的Rails 3”一个有用的博客帖子：HTTP：//bcardarella.com/post/716951242/custom-subdomains-in-rails- 3。

丹尼尔·基欧实现的应用程序，并写了教程。

是应用程序对你有用？在Twitter项目：“@rails_apps”：HTTP：//twitter.com/rails_apps
和鸣叫一定的好评。我很想知道你是帮助了由什么我放在一起。

H2。 MIT许可证

“MIT许可证”：HTTP：//www.opensource.org/licenses/mit-license

版权所有©2012丹尼尔·基欧

H2。相关链接

| _。入门| _。文章| _。教程|
|“学习Rails的”：HTTP：//learn-rails.com/ |“Twitter的引导和Rails”：HTTP：//railsapps.github.io/twitter-bootstrap-rails.html |“Rails和引导”：HTTP： //railsapps.github.io/rails-bootstrap/ |
|“Ruby和Rails”：HTTP：//railsapps.github.io/ruby-and-rails.html |“分析Rails的”：HTTP：//railsapps.github.io/rails-google-analytics.html | |
|“什么是Ruby on Rails的？”：HTTP：//railsapps.github.io/what-is-ruby-rails.html |“Heroku和Rails的”：HTTP：//railsapps.github.io/rails-heroku- tutorial.html |“设计与惨惨和Twitter引导”：HTTPS：//tutorials.railsapps.org/rails3-bootstrap-devise-cancan |
|“Rails的教程”：HTTPS：//tutorials.railsapps.org/rails-tutorial |“的JavaScript和Rails”：HTTP：//railsapps.github.io/rails-javascript-include-external.html |“Rails的会员网站用条纹“：HTTPS：//tutorials.railsapps.org/rails-stripe-membership-saas |
|“安装滑轨”：HTTP：//railsapps.github.io/installing-rails.html |“Rails环境变量”：HTTP：//railsapps.github.io/rails-environment-variables.html |“Rails的订阅网站与Recurly“：HTTPS：//tutorials.railsapps.org/rails-recurly-subscription-saas |
|“Rails更新”：HTTP：//railsapps.github.io/updating-rails.html |“混帐和Rails”：HTTP：//railsapps.github.io/rails-git.html |“启动发射前注册申请” ：HTTP：//railsapps.github.io/tutorial-rails-prelaunch-signup.html |
|“Rails的作曲家”：HTTP：//railsapps.github.io/rails-composer/ |“电子邮件和Rails”：HTTP：//railsapps.github.io/rails-send-email.html |“制定使用RSpec和黄瓜“：HTTP：//railsapps.github.io/tutorial-rails-devise-rspec-cucumber.html |
|“Rails的例子”：HTTP：//railsapps.github.io/ |“Haml的和Rails”：HTTP：//railsapps.github.io/rails-haml.html |“设计与Mongoid”：HTTP：// railsapps .github.io /教程护栏-mongoid-devise.html |
|“Rails的入门应用程序”：HTTP：//railsapps.github.io/rails-examples-tutorials.html |“Rails应用程序布局”：HTTP：//railsapps.github.io/rails-default-application-layout.html |“OmniAuth与Mongoid”：HTTP：//railsapps.github.io/tutorial-rails-mongoid-omniauth.html |
| |“HTML5样板Rails的”：HTTP：//railsapps.github.io/rails-html5-boilerplate.html |“子域与制定”：HTTP：//railsapps.github.io/tutorial-rails-subdomains.html |
| |“示例Gemfiles Rails的”：HTTP：//railsapps.github.io/rails-3-2-example-gemfile.html | |
| |“Rails应用程序模板”：HTTP：//railsapps.github.io/rails-application-templates.html | |

！HTTPS：//cruel-carlota.pagodabox.com/8f9093c277a7a135ad14ae2fb3df4d97（githalytics.com阿尔法）！
