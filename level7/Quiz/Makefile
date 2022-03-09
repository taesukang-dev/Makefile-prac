NAME = main
SRC = main.o
OBJ = $(SRC:.c=.o)
LIBFT = libft.a
LIB_NAME = ft
LIB_SRCS = first.c second.c third.c
LIB_OBJS = $(LIB_SRCS:.c=.o)

CC = gcc
CFLAGS = -Wall -Wextra -Werror

RM = rm -f

all : $(NAME)

clean :
	$(RM) *.o
fclean: clean
	$(RM) $(LIBFT) $(NAME)
re : fclean all

$(NAME) : $(OBJ) $(LIBFT)
	$(CC) $(CFLAGS) -o $@ $^
$(LIBFT) : $(LIB_OBJS)
	ar rcs $@ $?
%.o : %.c
	$(CC) $(CFLAGS) -c $<
