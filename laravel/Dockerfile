FROM php:8.3-fpm

WORKDIR /var/www/html

# Install system dependencies needed for Laravel
RUN apt-get update && apt-get install -y \
      git \
      unzip \
      libpq-dev \
      libzip-dev \
      zip \
    && docker-php-ext-install pdo_pgsql zip

# Copy composer
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

# Copy Laravel application code
COPY . .

# Install dependencies
RUN composer install --no-dev --optimize-autoloader

CMD ["php-fpm"]
