# Intégration continu - Florys Robin

### Détails de la configuration

1. **Box Debian :**
   - `config.vm.box = "debian/buster64"` : Crée une VM avec la box Debian Buster 64 bits. Vagrant téléchargera cette box depuis Vagrant Cloud si elle n'est pas déjà disponible localement.

2. **Provisionnement :**
   - La section de provisionnement exécute les commandes suivantes lors de la création de la VM :
     - `apt-get update` : Met à jour la liste des paquets pour les mises à jour et les nouvelles installations de paquets.
     - `apt-get install -y git` : Installe Git. L'option `-y` permet d'accepter automatiquement les invites pendant l'installation.

## Utilisation

1. Clonez ce dépôt :
   ```bash
   git clone <URL_DU_DEPOT>
   cd <NOM_DU_REPERTOIRE>
   ```

2. Démarrez la VM avec Vagrant :
   ```bash
   vagrant up
   ```

3. Accédez à la VM :
   ```bash
   vagrant ssh
   ```

4. Git est maintenant installé et prêt à être utilisé !

## Commandes Vagrant utiles

- `vagrant halt` : Arrête la VM.
- `vagrant destroy` : Supprime la VM.
- `vagrant reload` : Redémarre la VM en appliquant les modifications du `Vagrantfile`.

## Aide et Ressources

Pour plus d'informations sur Vagrant, consultez la [documentation officielle](https://www.vagrantup.com/docs).
```

Vous pouvez copier ce texte dans un fichier `README.md` pour documenter votre projet.
