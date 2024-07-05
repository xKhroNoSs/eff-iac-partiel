# eff-iac-partiel

Le terraform crée une vm, une ip publique, une règle firewall pour autoriser ssh
J'ai push les tfvars pour plus de lisibilité lors de la correction.

La partie ansible crée un user, clone le repo via git, crée un venv avec les deps, ajoute un service systemd pour l'exec avec le user. Il y a également un nginx qui est configuré pour rediriger les requêtes du port 80 vers le port 8000.