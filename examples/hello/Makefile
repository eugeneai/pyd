.PHONY: all clean test compile

all: 	test



compile: 
	echo 'import sys; sys.path.append("../../build/lib/");' > tsetup.py
	cat setup.py >> tsetup.py 
	python tsetup.py build

test:	compile
	python test.py
	
clean:
	rm -rf build
	rm -f tsetup.py
