LECS = lecture1.pdf

all: $(LECS)



%.pdf: %.qmd
	quarto render $^

%-6up.pdf: %.pdf
	pdfjam -q --nup 2x3 --suffix '6up'  $<

.PHONY: clean

clean:
	rm -fr 
show:
	echo $(LECS)
