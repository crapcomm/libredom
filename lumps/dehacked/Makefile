CPP=../../scripts/simplecpp

all: ../fdm_deh.lmp ../p1_deh.lmp ../p2_deh.lmp ../demo_deh.lmp

../fdm_deh.lmp: dehacked.txt
	$(CPP) -DFREEDM < $< > $@

../demo_deh.lmp: dehacked.txt
	$(CPP) -DFREEDEMO -DPHASE1 < $< > $@

../p1_deh.lmp: dehacked.txt
	$(CPP) -DPHASE1 < $< > $@

../p2_deh.lmp: dehacked.txt
	$(CPP) -DPHASE2 < $< > $@

clean:
	$(RM) ../fdm_deh.lmp ../p1_deh.lmp ../p2_deh.lmp ../demo_deh.lmp
