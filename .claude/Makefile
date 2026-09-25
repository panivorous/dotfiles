MAKEFILE_DIR := $(dir $(abspath $(lastword $(MAKEFILE_LIST))))
CLAUDE_HOME := $(HOME)/.claude
FILES := CLAUDE.md settings.json agents

.PHONY: install
# -n: on reinstall, replace the existing link to agents/ instead of creating a link inside it.
install:
	mkdir -p $(CLAUDE_HOME)
	@for f in $(FILES); do \
		ln -sfn $(MAKEFILE_DIR)$$f $(CLAUDE_HOME)/$$f; \
	done
