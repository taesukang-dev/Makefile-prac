NAME = main

SRC_DIR = ./src/
SRC_NAME = fourth.c main.c
SRC = $(addprefix $(SRC_DIR), $(SRC_NAME))

OBJ_DIR = ./obj/
OBJ_NAME = $(SRC_NAME:.c=.o)
OBJ = $(addprefix $(OBJ_DIR), $(OBJ_NAME))

LIB_DIR = ./lib/
LIB = $(LIB_DIR)lib$(LIB_NAME).a

CC = gcc
CFLAGS = -Wall -Wextra -Werror
INCLUDE = -I./include -I./lib

$(NAME) : $(OBJ) $(LIB)
	$(CC) $(CFLAGS) -o $@ $^
$(LIB) :
	make -C $(LIB_DIR) all
$(OBJ_DIR)%.o : $(SRC_DIR)%.c
	@mkdir -p $(OBJ_DIR)
	$(CC) $(CFLAGS) $(INCLUDE) -c $< -o $@
