# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: gcollet <gcollet@student.42.fr>            +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2021/08/17 19:56:08 by gcollet           #+#    #+#              #
#    Updated: 2021/10/14 10:16:04 by gcollet          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

PROG	= philo

SRCS 	= srcs/main.c srcs/utils.c srcs/init.c srcs/routine.c

OBJS 	= ${SRCS:.c=.o}

HEADER	= -Iinclude

CC 		= gcc
CFLAGS 	= -Wall -Wextra -Werror -g

.c.o:		
					@$(CC) ${CFLAGS} ${HEADER} -c $< -o $(<:.c=.o)

all:	${PROG}

${PROG}:	${OBJS}
					@$(CC) ${OBJS} -o ${PROG} -lpthread
					@echo "\n\033[32m\033[1m  Philosophers Compiled\n\033[0m"

clean:
					@rm -f ${OBJS}

fclean: 	clean
					@rm -f ${PROG}

re:			fclean all

emote:	
					@echo "▒▒▒▒▒▒▒▒▄▄▄▄▄▄▄▄▄▄▒▒▒▒▒▒▒▒"
					@echo "▒▒▒▒▒▄█▀▀░░░░░░░░▀▀█▄▒▒▒▒▒"
					@echo "▒▒▒▄█▀▄██▄░░░░░░░░░░▀█▄▒▒▒"
					@echo "▒▒█▀░▀░░▄▀░░░░░░▄▀▀▀▀░▀█▒▒"
					@echo "▒█▀░░░░███░░░░░░▄█▄░░░░▀█▒"
					@echo "▒█░░░░░░▀░░░░░░░▀█▀░░░░░█▒"
					@echo "▒█░░░░░░░░░░░░░░░░░░░░░░█▒"
					@echo "▒█░░██▄░░▀▀▀▀▄▄░░░░░░░░░█▒"
					@echo "▒▀█░█░█░░░▄▄▄▄▄░░░░░░░░█▀▒"
					@echo "▒▒▀█▀░▀▀▀▀░▄▄▄▀░░░░░░▄█▀▒▒"
					@echo "▒▒▒█░░░░░░▀█░░░░░░░▄█▀▒▒▒▒"
					@echo "▒▒▒█▄░░░░░▀█▄▄▄▄▄█▀▀▒▒▒▒▒▒"
					@echo "▒▒▒▒▀▀▀▀▀▀▀▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒\n"

.PHONY: all clean fclean re