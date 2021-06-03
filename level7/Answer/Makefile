NAME := main

SRC = main.c
OBJ = $(SRC:.c=.o)

LIBFT := libft.a
LIB_NAME := ft
LIB_SRCS := first.c \
		second.c \
		third.c
LIB_OBJS := $(LIB_SRCS:.c=.o)

AR := ar
ARFLAGS := -rc
CC := gcc
CFLAGS := -Wall -Wextra -Werror

all : $(NAME)

clean :
	rm -f *.o
fclean : clean
	rm -f $(LIBFT) $(NAME)
re : fclean all


$(NAME) : $(OBJ) $(LIBFT)
	$(CC) $(CFLAGS) -o $@ $^
$(LIBFT) : $(LIB_OBJS)
	$(AR) $(ARFLAGS) $@ $?
%.o : %.c
	$(CC) $(CFLAGS) -c $<

.PHONY : all clean fclean
