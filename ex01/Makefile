CPPS = main.cpp

OBJS = ${CPPS:.cpp=.o}

NAME = ex01
CXX = c++
CXXFLAGS = -Wall -Wextra -Werror -std=c++98
%.o: %.cpp
	$(CXX) $(CXXFLAGS) -c $< -o $@

$(NAME): $(OBJS)
	$(CXX) $(CXXFLAGS) $(OBJS) -o $(NAME)

.PHONY: all clean fclean re
all: $(NAME);

clean: 
	rm -rf $(OBJS)

fclean: clean
	rm -rf $(NAME)

re: fclean all;
