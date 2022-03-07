OBJS = first.o second.o third.o
NAME = libft.a

$(NAME) : $(OBJS)
	ar rcs $@ $?
%.o : %.c
	cc -c $<