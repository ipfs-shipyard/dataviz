
url="http://localhost:5001/ipfs/"

publish:
	@export hash=$(shell ipfs add -r -q . | tail -n1) && \
		echo $$hash >published-version && \
		open $(url)$$hash/viz

watch:
	coffee --bare --watch --compile app.coffee