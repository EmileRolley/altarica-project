TARGET = tank.alt

SOURCE_ALT = Parameters.alt\
	Valve.alt\
	ValveVirtual.alt\
	Tank.alt\
	System.alt\

DIFF_ALT = 

all: $(TARGET) $(DIFF_ALT)

clean:
	rm -f *~

cleandir : clean
	rm -f $(TARGET) $(DIFF_ALT) test.alt

$(TARGET) :  $(SOURCE_ALT)
	rm -f $(TARGET)
	for d in $(SOURCE_ALT); do \
		cat $$d >> $(TARGET);\
	done

$(DIFF_ALT) : $(SOURCE_ALT)
