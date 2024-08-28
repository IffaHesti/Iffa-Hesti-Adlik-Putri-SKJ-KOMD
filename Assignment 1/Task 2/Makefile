# 'all' target: Compile the source code
all: multiply.exe

multiply.exe: multiply.cpp
	g++ -o multiply.exe multiply.cpp

# 'dump' target: Disassemble the compiled code
dump: multiply.exe
	objdump -d multiply.exe > multiply.exe.asm

# 'clean' target: Remove all generated files
clean:
	rm -f multiply.exe multiply.exe.asm

# 'run' target: Run the compiled executable
run: multiply.exe
	./multiply.exe
