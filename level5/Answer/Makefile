NAME := main
FT := ft
LIB_SRCS := first.c \
		second.c \
		third.c
LIB_OBJS := first.o \
		second.o \
		third.o
MAIN_SRC = main.c
MAIN_OBJ = main.o

AR := ar
ARFLAGS := -rc

$(NAME) : $(OBJS)
	$(AR) $(ARFLAGS) $@ $?
