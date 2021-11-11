CC=gcc
CFLAGS=-Wall -Werror -I include/
LDFLAGS=
EXEC=audiocorp

SRC=	$(shell echo src/*.c)
OB=		$(SRC:.c=.o)

.PHONY: clean fclean re all

all: $(EXEC)

audiocorp: $(OB)
			gcc -o $(EXEC) $(OB)  -lm -lsoundio

clean:
	rm -rf src/*.o

fclean: clean
	rm $(EXEC)

re: fclean all
