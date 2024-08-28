# 'all' target: Compile the source code
all: add_numbers.exe

add_numbers.exe: add_numbers.cpp
	g++ -o add_numbers.exe add_numbers.cpp

# 'dump' target: Disassemble the compiled code
dump: add_numbers.exe
	objdump -d add_numbers.exe > add_numbers.exe.asm

# 'clean' target: Remove all generated files
clean:
	rm -f add_numbers.exe add_numbers.exe.asm

# 'run' target: Run the compiled executable
run: add_numbers.exe
	./add_numbers.exe
