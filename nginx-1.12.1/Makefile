
default:	build

clean:
	rm -rf Makefile objs

build:
	$(MAKE) -f objs/Makefile

install:
	$(MAKE) -f objs/Makefile install

modules:
	$(MAKE) -f objs/Makefile modules

upgrade:
	/home/yg397/Software/nginx/sbin/nginx -t

	kill -USR2 `cat /home/yg397/Software/nginx/logs/nginx.pid`
	sleep 1
	test -f /home/yg397/Software/nginx/logs/nginx.pid.oldbin

	kill -QUIT `cat /home/yg397/Software/nginx/logs/nginx.pid.oldbin`
