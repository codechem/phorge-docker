FROM php:7.4-fpm
RUN apt-get update && apt-get install -y \
		libfreetype6-dev \
		libjpeg62-turbo-dev \
		git \
		libpng-dev \
	&& docker-php-ext-configure gd --with-freetype --with-jpeg \
	&& docker-php-ext-install -j$(nproc) gd \
	&& docker-php-ext-configure pcntl \
	&& docker-php-ext-install -j$(nproc) pcntl \
	&& docker-php-ext-configure mysqli \
	&& docker-php-ext-install -j$(nproc) mysqli
