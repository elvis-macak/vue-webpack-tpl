export PATH := node_modules/.bin/:$(PATH)
export LC_ALL := en_US.UTF-8

all: serve

install:
	@if [ ! -f node_modules/.bin/npm ]; then npm install npm; fi
	npm install

clean:
	@rm -rf dist

serve:
	npm run dev

lint:
	npm run lint

e2e:
	npm run e2e

deploy: clean
	npm run build
