# spring-security-demo

TP Spring Security (FSTG) : authentification et autorisation en mémoire avec Spring Boot 3, Thymeleaf et BCrypt.

## Prérequis
- Java 17 ou 21
- Maven 3.9+

## Lancer
```
mvn spring-boot:run
```
Puis ouvrir http://localhost:8080/

## Comptes de démonstration
| Utilisateur | Mot de passe | Rôles |
|---|---|---|
| user | 1111 | USER |
| admin | 1234 | ADMIN, USER |

## Règles d’accès
- `/` et `/css/**` : public
- `/user/**` : rôle USER
- `/admin/**` : rôle ADMIN
- `/login` : page de connexion personnalisée
- `/logout` : POST uniquement (CSRF)

> Projet pédagogique : les utilisateurs en mémoire ne sont pas destinés à la production.
