format:
	cargo fmt --quiet

lint:
	cargo clippy --quiet
run:
	cargo run 

release:
	cargo lambda build --release 

deploy:
	cargo lambda deploy

invoke:
	cargo lambda invoke --remote \
  		--data-ascii '{"command": "threads"}' \
  		--output-format json \
  		lambdathreads

all: format lint test run