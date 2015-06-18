##系统部署

###部署环境要求

* 操作系统
	>Linux，windows server均可
* 数据库
	>MySql 5.X 
* JAVA运行环境
	> JDK1.6及以上版本
* WEB服务器
	>Tomcat7.X及以上版本

###系统部署

应用程序以`.war`格式发布，请将`.war`文件拷贝至tomcat的webapp目录下即可。启动tomcat时，tomcat会自动将该文件解压，部署成功。

###系统配置
根据实际部署需求，需要对相关的属性进行配置，主要的配置文件有: `webapps/ssctvap/WEB-INF/classes/jfinal.properties`，主要的配置项有：

	######数据库相关
    jdbcUrl，数据库地址
	user，数据库用户名
	password，数据库用户密码
	######邮件相关
	mail.smtp.port，邮箱smtp端口
    mail.smtp.host，邮箱stmp地址
    mail.smtp.username，系统邮箱的用户名
    mail.smtp.password，邮箱密码
    #####web服务相关
	serverip，服务器IP地址
	#####程序数据
	attachmentRoot,审批附件保存地址

