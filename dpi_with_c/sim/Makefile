
ifneq ($(origin VCS_HOME), environment)
    $(error  "Please set `VCS_HOME`")
endif

CMP_OPTS += -sverilog
CMP_OPTS += -f ../src/filelist

cmp:
	@echo "VCS_HOME is ${VCS_HOME}"
	vcs -full64 ${CMP_OPTS}
run:
	@echo "VCS_HOME is ${VCS_HOME}"
	vcs -full64 ${CMP_OPTS} -R

clean:
	@rm -rf `ls | grep -v Makefile`
