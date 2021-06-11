.PHONY: all clean
# Это комментарий, который говорит, что переменная CC указывает компилятор, используемый для сборки
CC=gcc
#Это еще один комментарий. Он поясняет, что в переменной CFLAGS лежат флаги, которые передаются компилятору
CFLAGS=-L. -llibrary

all : server client


server:
	$(CC) -lpthread server.c library.c -o ./server $(CFLAG)

client:
	$(CC) -lpthread client.c library.c -o ./client $(CFLAG)

server.o:
	$(CC) -lpthread server.c -o server.o $(CFLAG)

client.o:
	$(CC) -lpthread client.c -o client.o $(CFLAG)






# server : server.c liblibrary.so
# 	$(CC) -pthread -o server server.c $(CFLAGS)

# client : client.c liblibrary.so
# 	$(CC) -o client client.c $(CFLAGS)

# liblibrary.so : library.o
# 	$(CC) -shared -o liblibrary.so library.o

# library.o : library.c
# 	$(CC) -fPIC -c library.c

# Цель clean. Она традиционно используется для быстрой очистки всех результатов сборки проекта.
# Очистка запускается так: make -f makefile clean
clean :
	rm server client library.o liblibrary.so