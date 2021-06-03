NAME := libft.a
SRCS := first.c \
		second.c \
		third.c
OBJS := $(SRCS:.c=.o)
AR := ar
ARFLAGS := -rc
CC := gcc
CFLAGS := -Wall -Wextra -Werror

$(NAME) : $(OBJS)
	$(AR) $(ARFLAGS) $@ $?

%.o : %.c
	$(CC) $(CFLAGS) -c $<
