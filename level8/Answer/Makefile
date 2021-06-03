NAME := main

SRC_DIR = ./src/
SRC_NAME = main.c \
			first.c \
			second.c \
			third.c
SRC = $(addprefix $(SRC_DIR),$(SRC_NAME))

OBJ_DIR = ./obj/
OBJ_NAME = $(SRC_NAME:.c=.o)
OBJ = $(addprefix $(OBJ_DIR),$(OBJ_NAME))

CC := gcc
CFLAGS := -Wall -Wextra -Werror
INCLUDE := -I./include

all : $(NAME)

clean :
	rm -f $(OBJ)
fclean : clean
	rm -f $(NAME)
re : fclean all

run : all
	./$(NAME)

$(NAME) : $(OBJ)
	$(CC) $(CFLAGS) -o $@ $^
$(LIBFT) : $(LIB_OBJS)
	$(AR) $(ARFLAGS) $@ $?
$(OBJ_DIR)%.o : $(SRC_DIR)%.c
	@mkdir -p $(OBJ_DIR)
	$(CC) $(CFLAGS) $(INCLUDE) -c $< -o $@

.PHONY : all clean fclean
