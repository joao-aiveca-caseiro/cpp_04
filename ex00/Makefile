SRCS		= main.cpp\
				Animal.cpp\
				Cat.cpp\
				Dog.cpp\
				WrongCat.cpp\
				WrongAnimal.cpp
INCS		= Animal.hpp\
				Cat.hpp\
				Dog.hpp\
				WrongCat.hpp\
				WrongAnimal.hpp
OBJS		= ${SRCS:.cpp=.o}
NAME		= test
CXX			= c++
CXXFLAGS		= -Wall -Wextra -Werror -std=c++98 -fsanitize=address

$(NAME):	${OBJS} ${INCS}
			${CXX} ${CXXFLAGS} ${OBJS} -o ${NAME}

all:		$(NAME)

clean:
			${RM} ${OBJS}

fclean:		clean
			${RM} $(NAME)

re:			fclean all