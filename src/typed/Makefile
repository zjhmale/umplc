opts=-use-ocamlfind \
	-syntax camlp4o \
	-pkg core \
	-pkg pa_ounit.syntax \
	-tag thread \
	-tag debug \
	-tag bin_annot \
	-tag short_paths \
	-cflags "-w A-4-33-40-41-42-43-34-44-27"  \
	-cflags -strict-sequence

all:
	ocamlbuild $(opts) Main.d.byte

clean:
	ocamlbuild -clean

test: all
	./Main.d.byte inline-test-runner dummy
