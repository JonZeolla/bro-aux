
DIAG=diag.log
BTEST=../../btest/btest

all: cleanup btest-verbose

# Showing all tests.
btest-verbose:
	@$(BTEST) -j -f $(DIAG)

brief: cleanup btest-brief

# Brief output showing only failed tests.
btest-brief:
	@$(BTEST) -j -b -f $(DIAG)

cleanup:
	@rm -f $(DIAG)

.PHONY: all btest-verbose brief btest-brief cleanup
