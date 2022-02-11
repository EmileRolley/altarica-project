TARGET = tank.spe

SOURCE_SPE = System.spe

DIFF_SPE = 

all: $(TARGET) $(DIFF_SPE)

clean:
	rm -f *~

cleandir : clean
	rm -f $(TARGET) $(DIFF_SPE) test.spe


$(TARGET) :  $(SOURCE_SPE)
	rm -f $(TARGET)
	for d in $(SOURCE_SPE); do \
		cat $$d >> $(TARGET);\
	done


$(DIFF_SPE) : $(SOURCE_SPE)
