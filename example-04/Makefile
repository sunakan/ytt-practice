YTT_COMMAND := ../ytt
################################################################################
# 実行
# $ make run
################################################################################
.PHONY: run
run: default dev stg prd

.PHONY: dev
dev:
	$(YTT_COMMAND) --file ./config --file ./env/development.yml

.PHONY: stg
stg:
	$(YTT_COMMAND) --file ./config --file ./env/staging.yml

.PHONY: prd
prd:
	$(YTT_COMMAND) --file ./config --file ./env/production.yml

.PHONY: default
default:
	$(YTT_COMMAND) --file ./config
