
url="http://localhost:5001/ipfs/"

publish: build
	@export hash=$(shell ipfs add -r -q . | tail -n1) && \
		echo $$hash >>all-versions && \
		echo $$hash >latest-version && \
		open $(url)$$hash/viz

build: app.coffee
	coffee --bare --compile $^

watch:
	coffee --bare --watch --compile app.coffee
