
circle-config: SHELL:=/bin/bash
circle-config:
	{ echo "=== Generating circleci config ==="; } 2>/dev/null
	circleci -h >/dev/null 2>&1 || { echo >&2 "Install the circleci cli with brew install"; }
	circleci config pack src > config.yml
	circleci config validate config.yml