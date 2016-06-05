TARGET = slide.pdf
OUT_FORMAT = beamer
IN_FORMAT = markdown
HEADER = header.tex

.PHONY: all clean

all: $(TARGET)

$(TARGET): *.yaml *.md
	pandoc -H $(HEADER) -f $(IN_FORMAT) -t $(OUT_FORMAT) -s -o $(TARGET) $^

clean:
	-@rm -f $(TARGET)
