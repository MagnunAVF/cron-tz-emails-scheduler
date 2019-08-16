help:
	@echo 'Makefile for cron-tz-emails-scheduler                                 '
	@echo '                                                                      '
	@echo 'Usage:                                                                '
	@echo '   build-jar                           Build app with Maven           '
	@echo '   build-docker                        Build docker image             '
	@echo '   run                                 Run app with docker            '

build-jar:
	@mvn clean install -DskipTests

build-docker:
	@docker build -f Dockerfile -t cron-tz-emails-scheduler .

run:
	@docker run -t --name cron-tz-emails-scheduler-container -p 8087:8080 cron-tz-emails-scheduler

.PHONY: help, build-jar, build-docker, run