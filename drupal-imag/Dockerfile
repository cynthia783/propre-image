# Utilisez l'image officielle de Drupal comme base
FROM drupal:latest

# Copiez les fichiers personnalisés de votre projet Drupal (optionnel)
# Vous pouvez ajouter votre propre code source ou thèmes, modules, etc.
COPY . /var/www/html

# Assurez-vous que le répertoire est accessible en écriture par le serveur web
RUN chown -R www-data:www-data /var/www/html

# Exposez le port sur lequel Drupal écoute par défaut
EXPOSE 80

# Commande par défaut pour exécuter le serveur web Apache
CMD ["apache2-foreground"]
