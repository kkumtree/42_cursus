NAME	= libft.a

SRCS	= ./ft_putchar.c \
		  ./ft_putchar_n.c \
		  ./ft_putstr.c \
		  ./ft_putnbr_base.c \
		  ./ft_atoi.c \
		  ./ft_atouni.c \
		  ./get_atouni_width.c \
		  ./get_itoa_width.c \
		  ./get_itoa_base_width.c \
		  ./is_set.c \
		  ./ft_strlen.c \
		  ./ft_strchr.c \
		  ./ft_strstrhr.c \
		  ./ft_strndup.c \
		  ./max.c \
		  ./min.c

OBJS	= $(SRCS:.c=.o)
INCS	= .
RM		= rm -f
LIBC	= ar rc
CC		= gcc
CFLAGS	= -Wall -Wextra -Werror

.c.o :
	$(CC) $(CFLAGS) -c $< -o $(<:.c=.o) -I$(INCS)

$(NAME) : $(OBJS)
	$(LIBC) $(NAME) $(OBJS)

all : $(NAME)

clean :
	$(RM) $(OBJS)

fclean : clean
	$(RM) $(NAME) $(bonus)

re : fclean all
