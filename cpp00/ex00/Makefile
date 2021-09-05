SRCS	= megaphone.cpp

OBJS	= ${SRCS:.cpp=.o}

NAME	= megaphone

COMP	= clang++

RM		= rm -f

COMPFLAGS	= -Wall -Wextra -Werror

.cpp.o:
	${COMP} ${COMPFLAGS} -c $<

$(NAME):	${OBJS}
	${COMP} ${COMPFLAGS} -o ${NAME} ${OBJS}

all:	${NAME}

clean:
	${RM} ${OBJS}

fclean:	clean
	${RM} ${NAME} 

re:	fclean all

.PHONY:	all clean fclean re
