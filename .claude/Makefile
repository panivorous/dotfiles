MAKEFILE_DIR := $(dir $(abspath $(lastword $(MAKEFILE_LIST))))
CLAUDE_HOME := $(HOME)/.claude

.PHONY: install
install:
	mkdir -p $(CLAUDE_HOME)
	@if [ -L $(CLAUDE_HOME)/CLAUDE.md ]; then \
		rm $(CLAUDE_HOME)/CLAUDE.md; \
	elif [ -e $(CLAUDE_HOME)/CLAUDE.md ]; then \
		echo "Refusing to overwrite existing non-symlink $(CLAUDE_HOME)/CLAUDE.md" >&2; \
		exit 1; \
	fi
	ln -s $(MAKEFILE_DIR)CLAUDE.md $(CLAUDE_HOME)/CLAUDE.md
