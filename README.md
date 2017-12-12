    0. 功能：
	I.   在网页上控制步进动机启动和停止
	II.  在网页上实时显示超声测距数值


    1. 执行：
	在当前目录执行： ./run.sh
	在连接了校园网的其他电脑上登录 http://本机IP:5000
	即可看到结果

    2. 下一步： Linux中，Python和MySQL的连接：
	environment request:
		pip3
		Python3.4
		
	install:
		sudo apt-get install mysql-server
		sudo pip3 install SQLAlchemy
		sudo pip3 install mysqlclient

    3. 项目还需要：
		sudo pip3 install rpi.gpio
		hardware request: 树莓派、超声测距模块（型号：Sonar_V1.00）、步进动机（型号：TB6600盒式步进电机驱动器）

    4. 项目文件：
	config.py:       flask 框架的配置文件
	run.py:          执行文件
	hardware.py:     步进动机和超声测距的程序	具体见文件注释
	templates:       前端HTML文档
	static：         jquery框架等前端框架放置的文件夹
