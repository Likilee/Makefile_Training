NAME := main
LIB_FILE := libft.a
LIB_NAME := ft
LIB_SRCS := first.c \
		second.c \
		third.c
LIB_OBJS := first.o \
		second.o \
		third.o
MAIN_SRC = main.c
MAIN_OBJ = main.o

CC := gcc
CFLAGS := -Wall -Wextra -Werror
AR := ar
ARFLAGS := -rc

$(NAME) : $(LIB_FILE) $(MAIN_OBJ)
	$(CC) $(CFLAGS) -o $@ $^
$(LIB_FILE) : $(LIB_OBJS)
	$(AR) $(ARFLAGS) $@ $?
%.o : %.c
	$(CC) $(CFLAGS) -c $<
