NAME = libft.a
SRCS = first.c second.c third.c
OBJS = $(SRCS:.c=.o)
CC = gcc
CFLAGS = -Wall -Wextra -Werror

$(NAME) : $(OBJS)
	ar rcs $@ $?
%.o : %.c
	$(CC) $(CFLAGS) -c $<
