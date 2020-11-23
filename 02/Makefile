var:=urlcolor=red
variable=--variable $(var)
file=ue2

all: $(file).pdf

$(file).pdf: $(file).md
	pandoc $(file).md -o $(file).pdf $(variable)

view: all
	evince $(file).pdf &

clean:
	rm -r $(file).pdf
