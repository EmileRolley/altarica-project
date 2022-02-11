SRC = $(wildcard *.dot)

TARGET = $(SRC:.dot=.pdf)

all: $(TARGET)

clean:
	rm -f *~ *.core

cleandir: clean
	rm -f $(TARGET) $(SRC)

.SUFFIXES: .dot .pdf

.dot.pdf: $*.dot
	dot -Tpdf $*.dot -o $*.pdf
