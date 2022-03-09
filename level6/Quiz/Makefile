SRCS = first.c second.c third.c
OBJS = $(SRCS:.c=.o)
NAME = libft.a
CC = gcc
CFLAGS = -Wall -Wextra -Werror
RM = rm -f

$(NAME) : $(OBJS)
	ar rcs $@ $?
%.o : %.c
	$(CC) $(CFLAGS) -c $<

all : $(NAME)

clean :
	$(RM) $(OBJS)

fclean : clean
	$(RM) $(NAME)

re : fclean all
