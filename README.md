### Chez Nestor - Test Technique

-----

Le but de l'exercice est de créer les pages suivantes pour le backoffice de Chez Nestor :

- 🏠 Une liste des appartements
- 🏠 Une page de création d'un appartement
- 🏠 Une page de détails d'un appartement avec ses chambres
- 🛏️ Une liste de chambres par appartement
- 🛏️ Une page de création d'une chambre d'un appartement
- 👤 Une liste de clients
- 👤 Une page de création de client
- 👤 Une page de détails de client
- 🏠 Une liste de réservations
- 🏠 Une page d'ajout d'une réservation
- 🏠 Une page de détails d'une réservation

Une petite API te permet de récupérer les différentes données :
L'accès à l'application de booking : https://app-booking-christ.herokuapp.com/  

### Liste des routes:

#### Apartment
* api/apartment (GET)
* api/apartment/:id (GET)
* api/apartment (POST)  
**format attendu de requête à envoyer**
```metadata json
{
    "number": "...",
    "name": "...",
    "rooms": [
        {
            "number":"...",
            "area": "...",
            "price": "..."
        },
        {
            "number":"...",
            "area": "...",
            "price": "..."
        }
    ]
}
```

#### Client
* api/client (GET)
* api/client/:id (GET)
* api/client (POST)  
**format de requête à envoyer**
```metadata json
{
    "firstName": "...",
    "lastName": "...",
    "email": "...",
    "phone": "...",
    "nationality": "...",
    "birthDate": "..."
}
```

#### Room
* api/room (GET)
* api/room/:id (DELETE)
* api/room (POST)  
**format de requête à envoyer**
```metadata json
{
    "number":"...",
    "area": "...",
    "price": "...",
    "apartmentId": "..."
}
```
#### Booking
* api/booking (GET)
* api/booking/:id (GET)
* api/booking (POST)  
**format de requête à envoyer**
```metadata json
{
    "clientId": "...",
    "roomId" : "..."
}
```

De plus, vous veillerez à respecter les règles suivantes :
- Un appartement contient au moins 1 chambre.
- Un client ne peut pas réserver plusieurs chambres en même temps.
- Lorsqu'une chambre a été réservée par un client, elle ne peut plus être réservée.

**Technologie** : le langage, le framework et plus généralement les outils sont Vue Js ou React Js, utilisez ce que vous connaissez le mieux ! :)

Le sujet est volontairement extrêmement large.

Quelques pistes de choses qui nous intéressent :

- ✨ Propreté de code : découpage, gestion d'erreurs, nommage des variables / fonctions, etc.
- 📚 Utilisation de librairies / frameworks
- 🎨 Réflexion UI / UX
- ⚙️ Tests
- ☁️ Déploiement sur un hébergeur (Netlify, Heroku ou autre)
- 📦 Consommation d'API

Si tu penses que tu as fait quelque chose qui mérite notre attention, n'hésite pas à nous le signaler ! :) 
