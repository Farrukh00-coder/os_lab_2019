# Makefile for revert string(static lib)

# binary: main.o librevert.a
# 	gcc -o binary main.o -L. -lrevert

# main.o: main.c
# 	gcc -c main.c

# librevert.a: revert_string.o
# 	ar cr librevert.a revert_string.o

# revert_string.o: revert_string.c
# 	gcc -c revert_string.c

# clean:
# 	rm -f *.o *.a binary



# Makefile for dinamic lib 

binary: main.o librevert.so
	gcc -o binary main.o -L. -lrevert -Wl,-rpath,.

main.o: main.c
	gcc -c main.c

librevert.so: revert_string.o
	gcc -shared -o librevert.so revert_string.o

revert_string.o: revert_string.c
	gcc -c -fPIC revert_string.c

clean:
	rm -f *.o *.so binary