

## --- Rent My Ride ---

*Votre mission, à supposer que vous l'acceptiez, consiste à réaliser un nouveau site internet pour notre client “Rent My Ride”.

De par votre grande expertise désormais en la matière, vous travaillerez comme un pro afin de réaliser un site internet pour le grand public. Grâce à un design et une expérience utilisateur hors pair, il sera possible de rechercher un véhicule que l’on souhaiterait louer pour une journée, une semaine, ou plus…

Notre client souhaitant avoir la main sur tout son contenu, vous aurez à réaliser un dashboard lui permettant d’administrer ses différents types de véhicules, sa flotte de véhicules, et bien sûr, ses demandes de réservation.

Nous avons en amont réalisé un modèle conceptuel de données, vous permettant de mener à bien cette mission.

Bonne chance, et bon courage!*

# Réalisation du dashboard  
  

**Gestion des catégories**  
  
**1 -** Vous allez créer le modèle “Category.php” et créer tous les setters et getters correspondants, ainsi qu’une méthode construct permettant d’hydrater un objet.  
  
**2 -** Créer le nouveau fichier “/controllers/dashboard/categories/add-ctrl.php”  dans votre design pattern MVC. Ce fichier devra permettre l’ajout d’une nouvelle catégorie de véhicule. Vous penserez à créer la vue correspondante: “/views/dashboard/categories/add.php”. Vous ajouterez au modèle, une méthode “insert” permettant d’effectuer l’ajout d’une catégorie en base de données grâce à la classe PDO.

  
**3 -** Créer le fichier “/controllers/dashboard/categories/list-ctrl.php”  permettant de lister toutes les catégories existantes. Vous penserez à créer la vue correspondante: “/views/dashboard/categories/list.php”. Dans le modèle “Category.php” une méthode “getAll” permettra de retourner toutes les données de la base.

  
**4 -** Créer le fichier “update-ctrl.php”  permettant d’éditer une catégorie depuis la liste précédente. Créez la vue correspondante ainsi que la méthode ”update” permettant la modification de la catégorie concernée.  
  
**5 -** Depuis la liste, permettre la suppression d’une catégorie grâce au controller “delete-ctrl.php” et la méthode “delete”.  
  
**6 -** Créer une méthode “isExist” permettant de savoir si une catégorie existe en base de données. Cette méthode sera appelée depuis le controller d’ajout et générera un message d’erreur selon le cas.

  

**Gestion des véhicules**  
  
*Vous utiliserez le même principe que pour la gestion des catégories, mais avec le sous-dossier “vehicles”.*

  
**1 -** Créer une page contenant un formulaire permettant de créer un nouveau véhicule, et de l’affecter à une catégorie.

  
**2 -** Créer une page listant tous les véhicules classés par catégorie, par marque et par modèle.

  
**3 -** Depuis la liste précédente, créer une page permettant la modification d’un véhicule.

  
**4 -** Depuis la liste, permettre la suppression d’un véhicule.

  
**5 -** Ajouter un visuel facultatif pour illustrer le véhicule. Ce visuel sera stocké dans “/public/uploads/vehicles/” et portera un nom unique! Il sera supprimé en cas de suppression du véhicule.

#   

# Réalisation de la partie publique

**Listing**  
Depuis la page d’accueil du site, permettre aux internautes de visualiser tous les véhicules disponibles à la location sous forme de “cards”, toutes catégories confondues.

**Pagination**  
Sur la page d’accueil, ajouter une pagination dans le cas ou plus de 10 véhicules s’affichent.

**Filtrer par catégorie**  
Sur la page d’accueil, ajouter la possibilité pour l'utilisateur de filtrer selon une catégorie donnée.

**Recherche**  
Sur la page d’accueil, ajouter un champ de recherche permettant de trouver le véhicule souhaité.

**Détail d’un véhicule**  
Créer une page permettant d’afficher toutes les informations d’un véhicule choisi par l’utilisateur.

# Pour aller plus loin

**Réservation**  
Sur la partie publique, créer une page contenant un formulaire permettant aux utilisateurs de réserver un véhicule choisi. L’enregistrement du client et de sa réservation doivent se faire de manière coordonnée. L'échec de l’un, entraînant l’annulation de l’autre.

**Ville et code postal**  
Améliorer l‘expérience utilisateur lors de la réservation en interrogeant un micro-service pour le choix de la ville en fonction du code postal renseigné.

**Gestion des réservations**  
Dans le dashboard, créer une page permettant de lister toutes les réservations à venir. Sur la liste, donner la possibilité à l’administrateur d’envoyer un mail de confirmation de réservation à l’utilisateur.