all:
	@mkdir -p /home/nsahinog/data/wordpress
	@mkdir -p /home/nsahinog/data/mariadb
	@docker-compose -f srcs/docker-compose.yml up --build

start:
	@docker-compose -f srcs/docker-compose.yml start

stop:
	@docker-compose -f srcs/docker-compose.yml stop

clean:
	@docker-compose -f srcs/docker-compose.yml down --volumes

fclean: clean
	@docker system prune -af
	@rm -rf /home/nsahinog/data

.PHONY: all start stop clean fclean re