MAKEFILE_DIR := $(dir $(abspath $(lastword $(MAKEFILE_LIST))))
CLAUDE_HOME := $(HOME)/.claude
FILES := CLAUDE.md settings.json

.PHONY: install
install:
	mkdir -p $(CLAUDE_HOME)
	@for f in $(FILES); do \
		ln -sf $(MAKEFILE_DIR)$$f $(CLAUDE_HOME)/$$f; \
	done
