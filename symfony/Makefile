.PHONY: start stop stan test before-push
stop:
	docker-compose stop

install:
	composer install

start:
	docker-compose up -d


stan:
	./bin/phpstan analyze -c phpstan.neon

cs:
	./bin/php-cs-fixer fix --diff --dry-run

test:
	./bin/phpunit

before-push: cs stan test
	echo 'OK'