.PHONY: install test lint check

install:
	@$(MAKE) -s -C lab install

test:
	@$(MAKE) -s -C lab test

lint:
	@python3 lint.py

check: install lint test
